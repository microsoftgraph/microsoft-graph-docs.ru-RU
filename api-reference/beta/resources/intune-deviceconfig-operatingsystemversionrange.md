---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b00d3df68ad0d6cf13d9b4f4a5cff541aa33893a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368431"
---
# <a name="operatingsystemversionrange-resource-type"></a>Тип ресурса Оператингсистемверсионранже

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Диапазон версий операционной системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание этого диапазона (например, "допустимые сборки 1702")|
|ловестверсион|String|Наименьшая включающая версия, содержащаяся в этом диапазоне.|
|хигхестверсион|String|Максимальная включающая версия, которую содержит этот диапазон.|

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



