---
title: Тип ресурса Принтсеттингс
description: Представляет параметры на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c9af888d85256b88d4212cc84ba74d8dcdd5b590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973822"
---
# <a name="printsettings-resource-type"></a>Тип ресурса Принтсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры на уровне клиента для универсальной службы печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|документконверсионенаблед|Boolean|Указывает, включено ли преобразование документов для клиента. Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (XPS — PDF).|

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


