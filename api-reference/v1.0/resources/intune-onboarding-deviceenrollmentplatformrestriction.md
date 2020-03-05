---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df465172d02b701b8b9f9439a32644f5df541f45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448146"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Тип ресурса deviceEnrollmentPlatformRestriction

Пространство имен: Microsoft. Graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения на регистрацию для определенных платформ

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|platformBlocked|Логический|Указывает, блокируется ли регистрация платформы|
|personalDeviceEnrollmentBlocked|Boolean|Указывает, блокируется ли регистрация личных устройств|
|osMinimumVersion|String|Минимальная поддерживаемая версия ОС|
|osMaximumVersion|String|Максимальная поддерживаемая версия ОС|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```




