---
title: тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e102061864c39fcba9354fce916cf57c43a88b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007231"
---
# <a name="defaultuserrolepermissions-resource-type"></a>тип ресурса defaultUserRolePermissions

Содержит определенные настраиваемые разрешения роли пользователя по умолчанию в Azure Active Directory (AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Логический | Указывает, может ли пользователь по умолчанию создавать приложения. |  
| allowedToCreateSecurityGroups | Boolean | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
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
