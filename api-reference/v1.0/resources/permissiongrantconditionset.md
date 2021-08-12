---
title: Тип ресурса permissionGrantConditionSet
description: Указывает правило соответствия условиям, при которых событие включается или исключается из политики предоставления разрешений.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 774d0f8dce0a5e1128f8e2399fb8399f5ee84b1fa28aeee9fd2a0574ae5a4100
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196966"
---
# <a name="permissiongrantconditionset-resource-type"></a>Тип ресурса permissionGrantConditionSet

Пространство имен: microsoft.graph

Набор условий предоставления разрешений используется для указания правила соответствия в [политике предоставления разрешений](permissiongrantpolicy.md), чтобы включить или исключить событие предоставления разрешения.

Набор условий предоставления разрешений содержит несколько условий. Чтобы событие соответствовало набору условий предоставления разрешений, должны выполняться все условия.

## <a name="properties"></a>Свойства

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор набора условий предоставления разрешений. Ключ. Только для чтения. |
| permissionClassification | String | [Классификация разрешений](delegatedpermissionclassification.md) для предоставляемого разрешения или `all` для соответствия любой классификации разрешений (включая неклассифицированные разрешения). Значение по умолчанию: `all`. |
| permissionType | permissionType | Тип предоставляемого разрешения. Возможные значения: `application` — для разрешений приложений (например, роли приложений), `delegated` — для делегированных разрешений. Значение `delegatedUserConsentable` указывает делегированные разрешения, которые не были настроены издателем API для требования согласия администратора. Это значение можно использовать во встроенных политиках предоставления разрешений, но нельзя использовать в настраиваемых политиках предоставления разрешений. Обязательно. |
| resourceApplication | String | **appId** приложения ресурсов (например, API), для которого предоставляется разрешение, или `any` для соответствия любому приложению ресурсов или API. Значение по умолчанию: `any`. |
| permissions | Коллекция строк | Список значений **id** для соответствия определенным разрешениям или список с одним значением `all` для соответствия любым разрешениям. **id** делегированных разрешений доступны в свойстве **oauth2PermissionScopes** объекта [**servicePrincipal**](serviceprincipal.md) API. **id** разрешений приложений доступны в свойстве **appRoles** объекта [**servicePrincipal**](serviceprincipal.md) API. **id** разрешений приложений для конкретных ресурсов доступны в свойстве **resourceSpecificApplicationPermissions** объекта [**servicePrincipal**](serviceprincipal.md) API. По умолчанию используется единственное значение `all`. |
| clientApplicationIds | Коллекция String | Список значений **appId** для соответствия клиентским приложениям или список с одним значением `all` для соответствия любым клиентским приложениям. По умолчанию используется единственное значение `all`. |
| clientApplicationTenantIds | Коллекция String | Список идентификаторов клиента Azure Active Directory, в котором зарегистрировано клиентское приложение, или список с одним значением `all` для соответствия клиентским приложениям, зарегистрированным в любом клиенте. По умолчанию используется единственное значение `all`. |
| clientApplicationPublisherIds | Коллекция String | Список идентификаторов Microsoft Partner Network (MPN) для проверенных издателей клиентского приложения или список с одним значением `all` для соответствия клиентским приложениям от любого издателя. По умолчанию используется единственное значение `all`. |
| clientApplicationsFromVerifiedPublisherOnly | Логический | Присвойте значение `true` для соответствия только клиентским приложениям проверенного издателя. Присвойте значение `false` для соответствия любому клиентскому приложению, даже если у него нет проверенного издателя. Значение по умолчанию: `false`. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
}-->

```json
{
    "id": "string (identifier)",
    "permissionClassification": "string",
    "permissionType": "string",
    "resourceApplication": "string",
    "permissions": [ "string" ],
    "clientApplicationIds": [ "string" ],
    "clientApplicationTenantIds": [ "string" ],
    "clientApplicationPublisherIds": [ "string" ],
    "clientApplicationsFromVerifiedPublisherOnly": false
}
```
