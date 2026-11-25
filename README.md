# Remote-Workstation-SDK PHP SDK

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
