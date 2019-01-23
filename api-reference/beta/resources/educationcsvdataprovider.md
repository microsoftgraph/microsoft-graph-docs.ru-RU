---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c9211d5f7ca25b78c6e76c3744f6941e3b172bb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399348"
---
# <a name="educationcsvdataprovider-resource-type"></a>Тип ресурса educationCsvDataProvider

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  

На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **пользовательских настроек** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Необязательный настроек применяется для синхронизации профилей.|

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
