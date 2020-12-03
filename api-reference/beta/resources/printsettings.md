---
title: Тип ресурса Принтсеттингс
description: Представляет параметры на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 01c98eb68031018e6f7a32837e49a2095c7880d2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521238"
---
# <a name="printsettings-resource-type"></a>Тип ресурса Принтсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры на уровне клиента для универсальной службы печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|документконверсионенаблед|Логический|Указывает, включено ли преобразование документов для клиента. Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (XPS — PDF).|

## <a name="json-representation"></a>Представление JSON

Ниже представлено представление объекта Принтсеттингс в формате JSON.
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


