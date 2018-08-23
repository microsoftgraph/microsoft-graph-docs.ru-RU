# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Тип перечисления deviceManagementExchangeAccessStateReason

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Причина состояния доступа к Еxchange для устройства
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|отсутствует|0|Причина состояния доступа к Exchange не определено|
|unknown|1|Неизвестная причина состояния доступа|
|exchangeGlobalRule|2|Состояние доступа, определяемое глобальным правилом Exchange|
|exchangeIndividualRule|3|Состояние доступа, определяемое индивидуальным правилом Exchange|
|exchangeDeviceRule|4|Состояние доступа, определяемое правилом устройства Exchange|
|exchangeUpgrade|5|Состояние доступа из-за обновления Exchange|
|exchangeMailboxPolicy|6|Состояние доступа, определяемое политикой почтового ящика Exchange|
|other|7|Состояние доступа определяется Exchange|
|compliant|8|Состояние доступа, предоставленное в связи с проблемами соответствия требованиям|
|notCompliant|9|Состояние доступа, отозванное в связи с проблемами соответствия требованиям|
|notEnrolled|10|Состояние доступа отозвано в связи с проблемами управления|
|unknownLocation|12|Состояние доступа из-за неизвестного местоположения|
|mfaRequired|13|Состояние доступа из-за проблемы c MFA|
|azureADBlockDueToAccessPolicy|14|Состояние доступа отозвано политикой доступа AAD|
|compromisedPassword|15|Состояние доступа отозвано из-за компрометации пароля|
|deviceNotKnownWithManagedApp|16|Состояние доступа отозвано из-за проблемы с управляемым приложением|



