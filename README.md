# Remote-Workstation-SDK PHP SDK

<!-- simple-start:start -->
Use Remote-Workstation-SDK from a PHP app.

**Start here.** Run `composer require titancsa/remote-workstation-sdk`, then try the short example below. Install the matching Windows driver separately.
<!-- simple-start:end -->

> [!IMPORTANT]
> **Contact TitanCSA**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about commercial licensing, integration or support for this project.

`composer require titancsa/remote-workstation-sdk`

Windows x64 PHP8.2+; enable FFI extension and `ffi.enable=true`.

```php
require "vendor/autoload.php";
$client=new \TitanCSA\Products\RemoteWorkstationSDK\Client();
try {print_r($client->call("host_status"));} finally {$client->close();}
```

[API and operation schema](docs/API.md). Matching driver installed separately.
