---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ab311af46b80c48e5860b2d42aaee68abddf590
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098617"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Тип ресурса deviceEnrollmentPlatformRestriction

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения на регистрацию для определенных платформ

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|platformBlocked|Boolean|Указывает, блокируется ли регистрация платформы|
|personalDeviceEnrollmentBlocked|Boolean|Указывает, блокируется ли регистрация личных устройств|
|osMinimumVersion|String|Минимальная поддерживаемая версия ОС|
|osMaximumVersion|String|Максимальная поддерживаемая версия ОС|

## <a name="relationships"></a>Отношения
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




