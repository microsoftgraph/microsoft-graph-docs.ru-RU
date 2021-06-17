---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 56d7ea203f4ed72f45a3650197c1484f817567e6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992319"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>тип ресурса resourceSpecificPermissionGrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.

## <a name="methods"></a>Методы

|  Метод                                                                   |  Возвращаемый тип                                                                     | Описание                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[Список разрешений чата](../api/chat-list-permissiongrants.md)   | [коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, предоставленных в определенном чате.  |
|[Список разрешений группы](../api/group-list-permissiongrants.md) | [коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, предоставленных в определенной группе. |
|[Список разрешений группы](../api/team-list-permissiongrants.md)   | [коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, предоставленных в определенной группе.  |

## <a name="properties"></a>Свойства

| Свойство        | Тип          | Описание                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | string        | Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами. Только для чтения.           |
| deletedDateTime | dateTimeOffset| Не используется.                                                                             |
| clientId        | string        | ID приложения Azure AD, которое было предоставлено доступ. Только для чтения.                            |
| clientAppId     | string        | ID директора службы приложения Azure AD, которое было предоставлено доступ. Только для чтения.   |
| resourceAppId   | string        | ID приложения Azure AD, на который размещен ресурс. Только для чтения.                        |
| permissionType  | string        | Тип разрешения. Возможные значения: `Application`, `Delegated`. Только для чтения. |
| разрешение      | string        | Имя разрешения. Только для чтения.                                                |

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


