---
title: тип ресурса educationOnPremisesInfo
description: Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4c5da3180b1c15f2363bfd651d0f4e3d68f41b60
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232262"
---
# <a name="educationonpremisesinfo-resource-type"></a>тип ресурса educationOnPremisesInfo

Пространство имен: microsoft.graph

Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| immutableId | Строка | Уникальный идентификатор объекта пользователя в Active Directory. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOnPremisesInfo",
  "immutableId": "String"
}
```
