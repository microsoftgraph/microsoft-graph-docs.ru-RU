---
title: Тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения для роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6ee2e8deccf73929b68079379efb0f6d93a3369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135676"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Тип ресурса defaultUserRolePermissions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит определенные настраиваемые разрешения для роли пользователя по умолчанию в Azure AD.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Boolean | Указывает, может ли роль пользователя по умолчанию создавать приложения. |  
| allowedToCreateSecurityGroups | Boolean | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
| allowedToReadOtherUsers | Boolean | Указывает, может ли роль пользователя по умолчанию читать других пользователей. |  

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


