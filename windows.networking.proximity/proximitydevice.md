---
-api-id: T:Windows.Networking.Proximity.ProximityDevice
-api-type: winrt class
-api-device-family-note: xbox
---

<!-- Class syntax.
public class ProximityDevice : Windows.Networking.Proximity.IProximityDevice
-->

# Windows.Networking.Proximity.ProximityDevice

## -description
Enables you to publish messages to proximate devices or subscribe to messages from proximate devices.

## -remarks
The [ProximityDevice](proximitydevice.md) class enables applications to communicate with running applications on devices, typically within a range of 3 centimeters to 4 centimeters.

You can create an instance of [ProximityDevice](proximitydevice.md) by using the [GetDefault](proximitydevice_getdefault.md) or [FromId](proximitydevice_fromid.md) static method.

The [ProximityDevice](proximitydevice.md) class uses publish/subscribe semantics and is useful for advertising and receiving small blocks of data. For larger amounts of data, or for persistent communications, use the [PeerFinder](peerfinder.md) and [StreamSocket](../windows.networking.sockets/streamsocket_streamsocket.md) classes. For Windows Store app, publications and subscriptions are active only if the calling app is in the foreground.



> [!IMPORTANT]
> The proximity APIs do not provide authentication, encryption, or message integrity. Do not use proximity to exchange user sensitive information such as passwords, financial data, text messages, email, photographs, or government id numbers.

## -examples


[!code-csharp[ArriveDepart](../windows.networking.proximity/code/ProximityReferenceSample/csharp/MainPage.xaml.cs#SnippetArriveDepart)]

[!code-js[ArriveDepart](../windows.networking.proximity/code/ProximityReferenceSample/js/default.js#SnippetArriveDepart)]

[!code-vb[ArriveDepart](../windows.networking.proximity/code/ProximityReferenceSample/vbnet/MainPage.xaml.vb#SnippetArriveDepart)]

## -see-also
[Proximity and Tapping (JavaScript)](http://msdn.microsoft.com/library/84a30dcf-ef14-4a93-9e7c-7a3de867d46b), [Proximity and Tapping (C#/VB/C++)](http://msdn.microsoft.com/library/f25bb1df-1cfd-45cd-8c67-04eec73ebfbd), [Proximity sample](http://go.microsoft.com/fwlink/p/?linkid=245082)

## -capabilities
proximity
ID_CAP_PROXIMITY [Windows Phone], ID_CAP_PROXIMITY [Windows Phone]
