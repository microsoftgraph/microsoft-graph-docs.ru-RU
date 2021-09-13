---
title: тип enum managedAppDataEncryptionType
description: Представляет уровень шифрования данных приложений для управляемых приложений
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3840d0e2249225974e04017bca3e8d8c19be5c2a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118077"
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




