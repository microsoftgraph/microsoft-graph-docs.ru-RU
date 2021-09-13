---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 792f490ef9aa8ccdf6155b0eee0daf9f7c66b3b9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118668"
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

## <a name="relationships"></a>Отношения

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
