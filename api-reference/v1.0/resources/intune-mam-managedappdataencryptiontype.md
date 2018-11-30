---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027237"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Тип перечисления managedAppDataEncryptionType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет уровень, на который приложение шифрование для управляемых приложений
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|useDeviceSettings|0|Приложение шифрование на основе параметров по умолчанию на устройстве.|
|afterDeviceRestart|1|Приложение шифрование при перезапуске устройства.|
|whenDeviceLockedExceptOpenFiles|2|Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых|
|whenDeviceLocked|3|Данные приложения, связанные с этой политикой шифруются при заблокированном устройство|



