---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
author: mmast-msft
ms.openlocfilehash: 1a816d4e176147d549381465154e35cf0a821b98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317901"
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
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
