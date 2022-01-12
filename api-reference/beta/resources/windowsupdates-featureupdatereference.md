---
title: тип ресурса featureUpdateReference
description: Представляет Windows 10 обновления функций.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 21fcec33dd0072aed12205f44a24eac7c4ba7569
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61836666"
---
# <a name="featureupdatereference-resource-type"></a>тип ресурса featureUpdateReference

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Windows 10 обновления функций.

В развертывании одна и та же ссылка на обновление функций может привести к тому, что устройства получают различные изменения обновления, но содержимое считается контекстуальным эквивалентом для всех устройств в развертывании.

Наследует [от windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|version|String|Указывает обновление функций по версии.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateReference",
  "version": "String"
}
```

