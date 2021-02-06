---
title: Сложный тип requestorSettings
description: Используется для `requestorSettings` свойства политики назначения пакета доступа. Предоставляет дополнительные параметры для выбора, кто может создать запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a9bd91605d106b488de21f29baefe4b31d28f323
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133730"
---
# <a name="requestorsettings-resource-type"></a>Тип ресурса requestorSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для **свойства requestorSettings** политики [назначения пакета доступа.](accesspackageassignmentpolicy.md) Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на пакет доступа для этой политики.

| Кто может запросить | scopeType | Коллекция allowedRequestors|
|:----------------|:----------|:------------------|
|Никто|`NoSubjects`|пустой массив|
|Конкретный пользователь в каталоге|`SpecificDirectorySubjects`|[singleUser](singleuser.md)|
|Пользователи в каталоге, которые являются участниками группы|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|Пользователи в каталоге со `userType` значением `member`|`AllExistingDirectoryMemberUsers`|пустой массив|
|Пользователи в каталоге|`AllExistingDirectorySubjects`|пустой массив|
|Пользователи в определенных подключенных организациях|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|Пользователи из всех подключенных организаций, для свойства состояния подключенной организации установлено состояние `configured` .|`AllConfiguredConnectedOrganizationSubjects`|пустой массив|
|Любой пользователь|`AllExternalSubjects`|пустой массив|

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |Строка |Кто может запросить. Один из `NoSubjects` , , , , , , или `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllConfiguredConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` .  |
| acceptRequests | Boolean | Указывает, принимаются ли новые запросы для этой политики. |
| allowedRequestors | [Коллекция userSet](userset.md)| Пользователи, которым разрешено запрашивать эту политику, которые могут быть [singleUser,](singleuser.md) [groupMembers](groupmembers.md)и [connectedOrganizationMembers.](connectedorganizationmembers.md) |

## <a name="json-representation"></a>Представление в формате JSON


Ниже приводится представление свойства **requestorSettings** политики в JSON, которое позволяет участникам группы запрашивать запросы.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings"
}-->

```json
{
  "scopeType": "SpecificDirectorySubjects",
  "acceptRequests": true,
  "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.groupMembers",
         "isBackup": false,
         "id": "string (identifier)",
         "description": "Authorized requestors"
       }
   ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


