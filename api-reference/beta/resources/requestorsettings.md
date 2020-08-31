---
title: сложный тип Рекуесторсеттингс
description: Используется для `requestorSettings` Свойства политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора пользователей, которые могут создавать запросы.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f54a0c00c7a906e67d8c2861eae7c8437a28fad0
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311839"
---
# <a name="requestorsettings-resource-type"></a>Тип ресурса Рекуесторсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для свойства **рекуесторсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Предоставляет дополнительные параметры для выбора пользователей, которые могут создать запрос для пакета доступа в этой политике.

| Кто может запрашивать | scopeType | Коллекция Алловедрекуесторс|
|:----------------|:----------|:------------------|
|Никто|`NoSubjects`|пустой массив|
|Отдельный пользователь в каталоге|`SpecificDirectorySubjects`|[SingleUser.](singleuser.md)|
|Пользователи в каталоге, которые являются участниками группы|`SpecificDirectorySubjects`|[граупмемберс](groupmembers.md)|
|Пользователи в каталоге со `userType` значением `member`|`AllExistingDirectoryMemberUsers`|пустой массив|
|Пользователи в каталоге|`AllExistingDirectorySubjects`|пустой массив|
|Пользователи в определенных подключенных организациях|`SpecificConnectedOrganizationSubjects`|[коннектедорганизатионмемберс](connectedorganizationmembers.md)|
|Пользователи из любых подключенных организаций, у которых в свойстве State для связанной организации задано значение `configured` .|`AllConfiguredConnectedOrganizationSubjects`|пустой массив|
|Любой пользователь|`AllExternalSubjects`|пустой массив|

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |String |Кто может запрашивать. Один из `NoSubjects` ,,,,, `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` или `AllExternalSubjects` .  |
| акцептрекуестс | Логический | Указывает, принимаются ли новые запросы для этой политики. |
| алловедрекуесторс | Коллекция [User](userset.md) Collection| Пользователи, которым разрешено запрашивать эту политику, которая может быть [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md)и [коннектедорганизатионмемберс](connectedorganizationmembers.md). |

## <a name="json-representation"></a>Представление JSON


Ниже приведено представление объекта **рекуесторсеттингс** в формате JSON, которое позволяет членам группы запрашивать.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings",
  "baseType": ""
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
