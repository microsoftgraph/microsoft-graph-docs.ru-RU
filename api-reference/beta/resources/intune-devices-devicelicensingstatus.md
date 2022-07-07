---
title: Тип перечисления deviceLicensingStatus
description: Указывает состояние лицензирования устройств после включения подписки на устройства с Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c0ff1ff53acd502fc6c92923b0a80a99e039d280
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66672036"
---
# <a name="devicelicensingstatus-enum-type"></a>Тип перечисления deviceLicensingStatus

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает состояние лицензирования устройств после включения подписки на устройства с Windows.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|licenseRefreshStarted|0|Это состояние задается при запуске обновления лицензии.|
|licenseRefreshPending|1|Это состояние задается, когда ожидается обновление лицензии.|
|deviceIsNotAzureActiveDirectoryJoined|2|Это состояние задается, если устройство не присоединено к Azure Active Directory.|
|verifyingMicrosoftDeviceIdentity|3|Это состояние задается при проверке удостоверения устройства Майкрософт.|
|deviceIdentityVerificationFailed|4|Это состояние задается при сбое проверки удостоверения устройства Майкрософт.|
|verifyingMirosoftAccountIdentity|5|Это состояние задается при проверке удостоверения учетной записи Майкрософт.|
|mirosoftAccountVerificationFailed|6 |Это состояние задается при сбое проверки удостоверения учетной записи Майкрософт.|
|acquiringDeviceLicense|7 |Это состояние задается при получении лицензии на устройство.|
|refreshingDeviceLicense|8 |Это состояние задается при обновлении лицензии устройства.|
|deviceLicenseRefreshSucceed|9 |Это состояние задается при успешном обновлении лицензии устройства.|
|deviceLicenseRefreshFailed|10|Это состояние задается при сбое обновления лицензии устройства.|
|removingDeviceLicense|11|Это состояние задается при удалении лицензии устройства.|
|deviceLicenseRemoveSucceed|12 |Это состояние задается при успешном удалении лицензии устройства.|
|deviceLicenseRemoveFailed|13|Это состояние задается при сбое удаления лицензии устройства.|
|unknownFutureValue|14|Он помещается здесь в качестве заполнителя для будущего расширения.|
|unknown|–1|Значение, используемое по умолчанию. Задайте значение unknown, если не удается определить состояние.|




