
<!DOCTYPE html>
<html>

<head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <title>ArcGIS Business Analyst</title>
    <script>if("ActiveXObject" in window) location.assign("unsupported.html");</script>
    <meta http-equiv="Pragma" content="no-cache">
    <meta http-equiv="Expires" content="-1">
    <meta http-equiv="CACHE-CONTROL" content="NO-CACHE">
    <link rel="shortcut icon" href="../esriAnalyst/themes/common/images/favicon.ico" type="image/x-icon">
    <link rel="stylesheet" href="themes/bao.css">
    <link rel="stylesheet" href="../esriAnalystCore/main.css" id="main-stylesheet">
</head>

<body data-env="qa" class="claro esriMaps esriMapsAnalyst esriBAO customTheme">
    <script src="../telemetry/telemetry.js"></script>
    <script src="../esriAnalyst/config.js"></script>
    <script src="../baUtil/filterLocale.js"></script>
    <script src="../dojo/dojo.js"></script>
    <script>
    require([
        "esriAnalystX/services/AppConfig",
        "esriBAO/config/StaticAppConfig",
        "esriBAO/config/AppConfig",
        "esriAnalystX/services/ThemeConfig",
        "esriBAO/config/ThemeConfig"
    ], function (AppConfig, StaticAppConfig, SpecialConfig, ThemeConfig, SpecialThemeConfig) {
        AppConfig.assign(StaticAppConfig, SpecialConfig);
        
        require(["esriAnalyst/themes/utils/ApplyThemeUtil"], function(ApplyThemeUtil) {
            ApplyThemeUtil.startup(ThemeConfig, SpecialThemeConfig);
            setTimeout(() => {
                require(["esriAnalyst/widgets/LoadingAnimation/LoadingAnimation", "esriAnalyst"]);
            }, 100);
        });
    });
    </script>

    <div id="splashScreen" class="esriMapsAnalystSplashScreen"></div>
    <div id="layoutNode"></div>
</body>

</html>
