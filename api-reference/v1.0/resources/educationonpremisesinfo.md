---
title: тип ресурса educationOnPremisesInfo
description: Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ace4f32edf7a708debea828bfc510aec630a7100
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078891"
---
# <a name="educationonpremisesinfo-resource-type"></a>тип ресурса educationOnPremisesInfo

Пространство имен: microsoft.graph

Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| immutableId | Строка | Уникальный идентификатор объекта пользователя в Active Directory. |

## <a name="relationships"></a>Отношения

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
