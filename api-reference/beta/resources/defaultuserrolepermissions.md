---
title: Тип ресурса Дефаултусерролепермиссионс
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ee3df9779d5c69ec35bdc4ac9d373554cb0728e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049949"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Тип ресурса Дефаултусерролепермиссионс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит некоторые настраиваемые разрешения роли пользователя по умолчанию в Azure AD.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| алловедтокреатеаппс | Boolean | Указывает, может ли роль пользователя по умолчанию создавать приложения. |  
| алловедтокреатесекуритиграупс | Boolean | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
| алловедтореадосерусерс | Boolean | Указывает, может ли роль пользователя по умолчанию читать других пользователей. |  

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


