---
title: тип enum managedAppDataEncryptionType
description: Представляет уровень шифрования данных приложений для управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e826358b3d920d265858fbff02f6768142a8b6f764492ec2d7f12d7b8125947d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192357"
---
# <a name="managedappdataencryptiontype-enum-type"></a>тип enum managedAppDataEncryptionType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет уровень шифрования данных приложений для управляемых приложений

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useDeviceSettings|0|Данные приложения шифруются в зависимости от параметров по умолчанию на устройстве.|
|afterDeviceRestart|1|Данные приложения шифруются при перезапуске устройства.|
|whenDeviceLockedExceptOpenFiles|2|Данные приложения, связанные с этой политикой, шифруются при блокировке устройства, за исключением открытых файлов.|
|whenDeviceLocked|3|Данные приложения, связанные с этой политикой, шифруются при блокировке устройства|




