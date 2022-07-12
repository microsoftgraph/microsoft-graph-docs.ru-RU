---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень шифрования данных приложения для управляемых приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d7480b7db8a28ef36a2ec0402de5024790881da
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734678"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Тип перечисления managedAppDataEncryptionType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет уровень шифрования данных приложения для управляемых приложений.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useDeviceSettings|0|Данные приложения шифруются на основе параметров по умолчанию на устройстве.|
|afterDeviceRestart|1|Данные приложения шифруются при перезапуске устройства.|
|whenDeviceLockedExceptOpenFiles|2|Данные приложения, связанные с этой политикой, шифруются при блокировке устройства, за исключением открытых файлов.|
|whenDeviceLocked|3|Данные приложения, связанные с этой политикой, шифруются при блокировке устройства|





