---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413691"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Тип перечисления managedAppDataEncryptionType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет уровень, на который приложение шифрование для управляемых приложений

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useDeviceSettings|0|Приложение шифрование на основе параметров по умолчанию на устройстве.|
|afterDeviceRestart|1|Приложение шифрование при перезапуске устройства.|
|whenDeviceLockedExceptOpenFiles|2|Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых|
|whenDeviceLocked|3|Данные приложения, связанные с этой политикой шифруются при заблокированном устройство|




