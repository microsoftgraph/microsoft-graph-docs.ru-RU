---
title: connectedOrganizationMembers сложный тип
description: Тип connectedOrganizationMembers определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивателя, утверждения или рецензента.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb5fce001b0a1e202d0b8f7b1a7f294208e812c1
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242931"
---
# <a name="connectedorganizationmembers-complex-type"></a>connectedOrganizationMembers сложный тип

Пространство имен: microsoft.graph


Используется в параметрах запроса политики назначения пакета доступа. Значение указывает, что этот тип определяет коллекцию пользователей, связанных с подключенной организацией, которым будет разрешено `@odata.type` `#microsoft.graph.connectedOrganizationMembers` запрашивать пакет доступа. [](connectedorganization.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|connectedOrganizationId|Строка|ID связанной [организации в](connectedorganization.md) управлении правами.|
|description|Строка|Имя связанной организации.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectedOrganizationMembers",
  "connectedOrganizationId": "String",
  "description": "String"
}
```



