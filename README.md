extension-kizzyrpc-imp
=======

A extension that uses Lime JNI to work that add's support for discord rpc to android.

Installation instructions
=======

Step 1. Install the Library through haxelib

```
haxelib git extension-kizzyrpc https://github.com/yNeoNova/extension-kizzyrpc.git
```

Or, you could pick [Haxe Module Manager](https://lib.haxe.org/p/hmm/), aka HMM:
```json
{
  "dependencies": [
    {
      "name": "extension-kizzyrpc-imp",
      "type": "git",
      "url": "https://github.com/yNeoNova/extension-kizzyrpc-imp",
      "ref": "main",
      "dir": null
    }
  ]
}
```

Step 2. Add this in `Project.xml`.

```xml
<haxelib name="extension-kizzyrpc-imp" if="android" />
```

Step 3. Done, this is a little example for how to use it.

```haxe
import android.kizzy.KizzyClient;

var kizzyClient:KizzyClient = new KizzyClient();

kizzyClient.setApplicationID('378534231036395521');
kizzyClient.setName('Kizzy RPC Client Android');
kizzyClient.setDetails('When RPC is sus');
kizzyClient.setLargeImage('attachments/973256105515974676/983674644823412798/unknown.png');
kizzyClient.setSmallImage('attachments/948828217312178227/948840504542498826/Kizzy.png');
kizzyClient.setStartTimeStamps(0, true);
kizzyClient.setButton1('YouTube', 'https://youtube.com/@m.a.jigsaw7297');
kizzyClient.setType(0);
kizzyClient.setState('State');
kizzyClient.setStatus('idle');
kizzyClient.closeOnDestroy(true);
kizzyClient.rebuildClient();
```
Use the [Kizzy](https://kizzy.dead8309.xyz/) for seeing more about types and setting up RPC image, or, copy the image link from your discord client.

# License
Read [License](https://github.com/yNeoNova/extension-kizzyrpc-imp/blob/main/LICENSE) to see what you can and can't do with this repo.

# CREDITS:
• Thanks to MAjigsaw77 for the original library

• Thanks to Fearester2008 for the repository
