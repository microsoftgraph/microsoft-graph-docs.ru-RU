---
title: тип ресурса educationOnPremisesInfo
description: Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c461c63309588fc01fef94fb53a3b9c6e0f2722858f1baaa93a663804e344b7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182534"
---
# <a name="educationonpremisesinfo-resource-type"></a>тип ресурса educationOnPremisesInfo

Пространство имен: microsoft.graph

Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| immutableId | String | Уникальный идентификатор объекта пользователя в Active Directory. |

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
