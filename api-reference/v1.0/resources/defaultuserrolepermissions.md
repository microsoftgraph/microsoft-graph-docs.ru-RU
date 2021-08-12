---
title: тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c55f24fc0733a0cd20e88a080f83fcda8314aa3bad3dcc18122aaf2eea7ada13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178495"
---
# <a name="defaultuserrolepermissions-resource-type"></a>тип ресурса defaultUserRolePermissions

Содержит определенные настраиваемые разрешения роли пользователя по умолчанию в Azure Active Directory (AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Логическое | Указывает, может ли пользователь по умолчанию создавать приложения. |  
| allowedToCreateSecurityGroups | Логическое | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
| allowedToReadOtherUsers | Логический | Указывает, может ли пользователь по умолчанию читать другие пользователи. |
|permissionGrantPoliciesAssigned|Коллекция String|Указывает, разрешено ли согласие пользователя на приложения и разрешено ли оно, какое разрешение на предоставление согласия и какая политика согласия приложения (permissionGrantPolicy) регулирует разрешение для пользователей на предоставление согласия. Значение должно быть в формате , где находится id встроенной или настраиваемой политики согласия `managePermissionGrantsForSelf.{id}` `{id}` [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies)  Пустой список указывает, что согласие пользователя на приложения отключено. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true,
  "permissionGrantPoliciesAssigned": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
