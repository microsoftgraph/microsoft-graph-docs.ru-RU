---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398529"
---
# <a name="operatingsystemversionrange-resource-type"></a>Тип ресурса operatingSystemVersionRange

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Диапазон версии операционной системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание этого диапазона (например действительно 1702 сборок)|
|lowestVersion|String|Низший включительно версия, которая содержит этот диапазон.|
|highestVersion|String|Наибольший включительно версию, которая содержит этот диапазон.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```




