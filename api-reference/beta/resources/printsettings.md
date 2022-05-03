---
title: Тип ресурса printSettings
description: Представляет параметры на уровне клиента для службы универсальной печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0339843083695904080104882ba9385a840b4c9e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176648"
---
# <a name="printsettings-resource-type"></a>Тип ресурса printSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры на уровне клиента для службы универсальной печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|documentConversionEnabled|Логическое|Указывает, включено ли преобразование документов для клиента. Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (xps в PDF) при необходимости.|

## <a name="json-representation"></a>Представление JSON

Ниже приведено представление printSettings в формате JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printSettings"
}-->

```json
{
  "documentConversionEnabled": true
}
```


