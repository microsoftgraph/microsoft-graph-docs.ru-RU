---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 108420e3c575f6a1ede395b64fbef0314fdcface
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264656"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>тип ресурса resourceSpecificPermissionGrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объявляет разрешения, предоставленные конкретному приложению Azure AD для экземпляра ресурса в Microsoft Graph.

Дополнительные сведения о предоставлении приложениям согласия на доступ к конкретному экземпляру ресурса см. в примере " Согласие на [доступ к ресурсам".](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)

## <a name="methods"></a>Методы

|  Метод                                                                   |  Возвращаемый тип                                                                     | Описание                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[Список предоставленных разрешений чата](../api/chat-list-permissiongrants.md)   | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, определенных для ресурсов, которые были предоставлены в определенном [чате.](chat.md)  |
|[Перечисление предоставленных разрешений группы](../api/group-list-permissiongrants.md) | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, определенных для ресурсов, которые были предоставлены в определенной [группе.](group.md) |
|[Перечисление предоставленных разрешений команды](../api/team-list-permissiongrants.md) | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, определенных для ресурсов, которые были предоставлены в определенной [группе.](team.md) |

## <a name="properties"></a>Свойства

| Свойство        | Тип          | Описание                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | string        | Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами. Только для чтения.           |
| deletedDateTime | dateTimeOffset| Не используется.                                                                             |
| clientId        | string        | ID приложения Azure AD, которое было предоставлено доступ. Только для чтения.                            |
| clientAppId     | string        | ID директора службы приложения Azure AD, которое было предоставлено доступ. Только для чтения.   |
| resourceAppId   | string        | ID приложения Azure AD, на который размещен ресурс. Только для чтения.                        |
| permissionType  | string        | Тип разрешения. Возможные значения: `Application`, `Delegated`. Только для чтения. |
| разрешение      | string        | Имя разрешения, определенного для ресурса. Только для чтения.                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
}-->

```json
{
  "id": "string (identifier)",
  "deletedDateTime": "dateTimeOffset",
  "clientId": "string",
  "clientAppId": "string",
  "resourceAppId": "string",
  "permissionType": "string",
  "permission": "string"
}
```


