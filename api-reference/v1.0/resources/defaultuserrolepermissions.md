---
title: Тип ресурса Дефаултусерролепермиссионс
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f2b4fbc4b4a496905f8199b065ecd94e849365e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581245"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Тип ресурса Дефаултусерролепермиссионс

Содержит определенные настраиваемые разрешения роли пользователя по умолчанию в Azure Active Directory (AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| алловедтокреатеаппс | Логический | Указывает, может ли роль пользователя по умолчанию создавать приложения. |  
| алловедтокреатесекуритиграупс | Логический | Указывает, может ли роль пользователя по умолчанию создавать группы безопасности. |  
| алловедтореадосерусерс | Логический | Указывает, может ли роль пользователя по умолчанию читать других пользователей. |
|пермиссионгрантполиЦиесассигнед|Коллекция объектов string|Указывает, разрешено ли согласие пользователя на приложения, и, если это так, какое разрешение на предоставление согласия и какая политика согласия приложения (Пермиссионгрантполици) управляет разрешением на предоставление разрешений для пользователей. Значение должно быть в формате `managePermissionGrantsForSelf.{id}` , где `{id}` — это **идентификатор** встроенной или настраиваемой [политики согласия приложения](/azure/active-directory/manage-apps/manage-app-consent-policies). Пустой список указывает на то, что согласие пользователя на приложения отключено. |

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
