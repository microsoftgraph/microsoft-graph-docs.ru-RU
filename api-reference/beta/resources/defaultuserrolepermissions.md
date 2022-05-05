---
title: Тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71edaa99eedc7a37abe5694ace6e5c3c05e29884
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202331"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Тип ресурса defaultUserRolePermissions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит настраиваемые разрешения настраиваемой роли пользователя по умолчанию в Azure AD.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Логическое | Указывает, может ли роль пользователя по умолчанию создавать приложения. |  
| allowedToCreateSecurityGroups | Логическое | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
| allowedToReadBitlockerKeysForOwnedDevice | Логическое | Указывает, могут ли зарегистрированные владельцы устройства считывать собственные ключи восстановления BitLocker с ролью пользователя по умолчанию. |
| allowedToReadOtherUsers | Логическое | Указывает, может ли роль пользователя по умолчанию читать других пользователей. |  

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
  "allowedToReadBitlockerKeysForOwnedDevice": true,
  "allowedToReadOtherUsers": true
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


