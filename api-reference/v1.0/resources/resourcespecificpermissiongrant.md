---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fd6e9e09a092719f20de2c34f2120537cd00606
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162198"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>тип ресурса resourceSpecificPermissionGrant

Пространство имен: microsoft.graph

РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.

Дополнительные сведения о предоставлении приложениям согласия на доступ к конкретному экземпляру ресурса см. в примере " Согласие на [доступ к ресурсам".](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)

## <a name="methods"></a>Методы

|  Метод                                                                   |  Возвращаемый тип                                                                     | Описание                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[Перечисление предоставленных разрешений группы](../api/group-list-permissiongrants.md) | Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, определенных для ресурсов, которые были предоставлены в определенной [группе.](group.md) |

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