---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00a521ee9474d023bfcb5e72cc2e8ac45d270341a7e65ed29f920eaf33bc50f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205838"
---
# <a name="educationterm-resource-type"></a>Тип ресурса educationTerm

Пространство имен: microsoft.graph

Срок. Представляет определенную часть учебного года. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                       |
| :---------- | :----- | :-------------------------------- |
| displayName | String | Отображаемое имя срока.         |
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
