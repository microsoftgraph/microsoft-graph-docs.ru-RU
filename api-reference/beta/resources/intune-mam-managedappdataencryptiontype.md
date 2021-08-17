---
title: тип enum managedAppDataEncryptionType
description: Представляет уровень шифрования данных приложений для управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d36cabacda74f33a5057257b5890f9496a9f64e28d2e36e808bbac8c17d9c24d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145231"
---
# <a name="managedappdataencryptiontype-enum-type"></a>тип enum managedAppDataEncryptionType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет уровень шифрования данных приложений для управляемых приложений

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useDeviceSettings|0|Данные приложения шифруются в зависимости от параметров по умолчанию на устройстве.|
|afterDeviceRestart|1 |Данные приложения шифруются при перезапуске устройства.|
|whenDeviceLockedExceptOpenFiles|2|Данные приложения, связанные с этой политикой, шифруются при блокировке устройства, за исключением открытых файлов.|
|whenDeviceLocked|3 |Данные приложения, связанные с этой политикой, шифруются при блокировке устройства|




