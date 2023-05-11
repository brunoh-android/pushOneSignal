# push_one_signal

Recebendo mensagens via Push, OneSignal


# Configurar na main

void main() {<br>
  WidgetsFlutterBinding.ensureInitialized();<br>
  OneSignal.shared.setLogLevel(OSLogLevel.verbose, OSLogLevel.none);<br>
  OneSignal.shared.setAppId("sua chave do oneSignal");<br>
  OneSignal.shared.promptUserForPushNotificationPermission().then((accept){<br>
    print("Accept permission: $accept");<br>
    });<br>
  runApp(const MyApp());<br>
}

## Short Video

https://github.com/brunoh-android/pushOneSignal/assets/67665152/dd1de1f3-b56b-49b0-809b-66b351348b46

