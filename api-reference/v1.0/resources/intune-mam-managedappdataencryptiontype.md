---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
author: tfitzmac
ms.openlocfilehash: 3cbb733eb578ca839e32851d8a6d217f69d6799d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330326"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Тип перечисления managedAppDataEncryptionType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет уровень, на который приложение шифрование для управляемых приложений
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useDeviceSettings|0|Приложение шифрование на основе параметров по умолчанию на устройстве.|
|afterDeviceRestart|1|Приложение шифрование при перезапуске устройства.|
|whenDeviceLockedExceptOpenFiles|2|Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых|
|whenDeviceLocked|3|Данные приложения, связанные с этой политикой шифруются при заблокированном устройство|



