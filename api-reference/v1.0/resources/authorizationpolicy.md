---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ce482195ce7921eb43f2e4d1845a95f750688f1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448872"
---
# <a name="authorizationpolicy-resource-type"></a>тип ресурса authorizationPolicy

Пространство имен: microsoft.graph

Представляет политику, которая может управлять настройками авторизации Azure Active Directory. Это однотон, который наследуется от базового типа политики и всегда существует для клиента.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Ознакомьтесь с объектом authorizationPolicy. |
| [Обновление авторизацииPolicy](../api/authorizationpolicy-update.md) | Нет | Обновление объекта authorizationPolicy. |

## <a name="properties"></a>Свойства  
| Свойство | Тип | Описание | 
|-|-|-|
|id|String| ID политики авторизации. Обязательно. Только для чтения.| 
|displayName|String| Отображение имени для этой политики. |  
|description|String| Описание этой политики.|  
|blockMsolPowerShell|Логический| Чтобы отключить использование MSOL PowerShell, установите это свойство true. Настройка true также отключит пользовательский доступ к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не влияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Логический| Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента. | 
|allowedToSignUpEmailBasedSubscriptions|Логический| Указывает, могут ли пользователи подписываться на подписки на основе электронной почты. | 
|allowEmailVerifiedUsersToJoinOrganization|Логический| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 
|allowInvitesFrom|String|Указывает, кто может приглашать внешних пользователей в организацию. Возможные значения:<ul><li>`none` - Запретить всем, включая администраторов, приглашать внешних пользователей. Параметр по умолчанию для правительства США.</li><li>`adminsAndGuestInviters` - Разрешить участникам глобальных администраторов, администраторов пользователей и приглашенных приглашений приглашать внешних пользователей.</li><li>`adminsGuestInvitersAndAllMembers` - Разрешить вышеперечисленные роли администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</li><li>`everyone` - Разрешить всем в организации, включая гостевых пользователей, приглашать внешних пользователей. Параметр по умолчанию для всех облачных сред, кроме правительства США.</li></ul> |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```
