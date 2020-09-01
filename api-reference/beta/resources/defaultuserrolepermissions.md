---
title: Тип ресурса Дефаултусерролепермиссионс
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca90884220f65bca752fcabe2e0ffe37578cdf90
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319829"
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

## <a name="relationships"></a>Отношения

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
