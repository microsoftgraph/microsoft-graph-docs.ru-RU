---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 769c4d405473ef800b92fbecb8797588cf59eb57
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944304"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>тип ресурса resourceSpecificPermissionGrant

Пространство имен: microsoft.graph

РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.

## <a name="methods"></a>Методы

|  Метод                                                                   |  Возвращаемый тип                                                                     | Описание                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[Список разрешений группы](../api/group-list-permissiongrants.md) | [коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Список разрешений, предоставленных в определенной группе. |

## <a name="properties"></a>Свойства

| Свойство        | Тип          | Описание                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | string        | Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами. Только для чтения.           |
| deletedDateTime | dateTimeOffset| Не используется.                                                                             |
| clientId        | String        | ID приложения Azure AD, которое было предоставлено доступ. Только для чтения.                            |
| clientAppId     | String        | ID директора службы приложения Azure AD, которое было предоставлено доступ. Только для чтения.   |
| resourceAppId   | String        | ID приложения Azure AD, на который размещен ресурс. Только для чтения.                        |
| permissionType  | String        | Тип разрешения. Возможные значения: `Application`, `Delegated`. Только для чтения. |
| разрешение      | String        | Имя разрешения. Только для чтения.                                                |

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