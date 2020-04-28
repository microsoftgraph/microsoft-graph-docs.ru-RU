---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a5cd426cb4118f1da8e16ce8e097175851204dbb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466401"
---
# <a name="operatingsystemversionrange-resource-type"></a>Тип ресурса Оператингсистемверсионранже

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Диапазон версий операционной системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание этого диапазона (например, "допустимые сборки 1702")|
|ловестверсион|String|Наименьшая включающая версия, содержащаяся в этом диапазоне.|
|хигхестверсион|String|Максимальная включающая версия, которую содержит этот диапазон.|

## <a name="relationships"></a>Связи
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



