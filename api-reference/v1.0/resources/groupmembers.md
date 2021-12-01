---
title: сложный тип groupMembers
description: Определяет коллекцию пользователей в клиенте, которым будет разрешено в качестве запрашивателя, утверждения или рецензента.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18260b0b94ddc50e60e60f427e0e4f879912758d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242817"
---
# <a name="groupmembers-complex-type"></a>сложный тип groupMembers

Пространство имен: microsoft.graph


Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакетов доступа.
Значение указывает, что этот тип определяет коллекцию пользователей в клиенте, которым будет разрешено в качестве запрашивателя, утвержденного или рецензента, которые являются членами `@odata.type` `#microsoft.graph.groupMembers` определенной группы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Имя группы в Azure AD. Только для чтения. |
|groupId|String|ID группы [в](group.md) Azure AD.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupMembers",
  "groupId": "String",
  "description": "String"
}
```



