---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7fe455bc0e934e08b858a084009ac5c8364a673
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950965"
---
# <a name="operatingsystemversionrange-resource-type"></a>Тип ресурса Оператингсистемверсионранже

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Диапазон версий операционной системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание этого диапазона (например, "допустимые сборки 1702")|
|Ловестверсион|Строка|Наименьшая включающая версия, содержащаяся в этом диапазоне.|
|Хигхестверсион|Строка|Максимальная включающая версия, которую содержит этот диапазон.|

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




