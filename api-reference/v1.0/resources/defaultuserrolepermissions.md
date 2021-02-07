---
title: Тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения для роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e89f175a62615efe172646613897222a9ae75fa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137559"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Тип ресурса defaultUserRolePermissions

Содержит определенные настраиваемые разрешения роли пользователя по умолчанию в Azure Active Directory (AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Boolean | Указывает, может ли роль пользователя по умолчанию создавать приложения. |  
| allowedToCreateSecurityGroups | Boolean | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
| allowedToReadOtherUsers | Boolean | Указывает, может ли роль пользователя по умолчанию читать других пользователей. |
|permissionGrantPoliciesAssigned|Коллекция String|Указывает, разрешено ли согласие пользователя на доступ к приложениям, и, если да, какое разрешение на предоставление согласия и какая политика согласия приложения (permissionGrantPolicy) управляет разрешением пользователей на предоставление согласия. Значение должно быть в `managePermissionGrantsForSelf.{id}` формате, где находится `{id}` **ид** встроенной или настраиваемой политики согласия [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies) Пустой список указывает, что согласие пользователя на приложения отключено. |

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
