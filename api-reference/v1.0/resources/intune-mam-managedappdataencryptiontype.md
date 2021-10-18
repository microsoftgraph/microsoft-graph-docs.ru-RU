---
title: тип enum managedAppDataEncryptionType
description: Представляет уровень шифрования данных приложений для управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7ca4e0fe6580cbc06002ff49c1d7b078c60da71f
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446970"
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



