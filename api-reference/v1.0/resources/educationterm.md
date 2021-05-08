---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41a878f58736f608cf9cc9f0c45867bf48669b1a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231838"
---
# <a name="educationterm-resource-type"></a>Тип ресурса educationTerm

Пространство имен: microsoft.graph

Срок. Представляет определенную часть учебного года. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                       |
| :---------- | :----- | :-------------------------------- |
| displayName | Строка | Отображаемое имя срока.         |
| externalId  | String | Идентификатор срока в системе синхронизации. |
| startDate   | Date   | Начало срока.                |
| endDate     | Date   | Конец срока.                  |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTerm"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTerm",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date",
  "displayName": "String"
}
```
