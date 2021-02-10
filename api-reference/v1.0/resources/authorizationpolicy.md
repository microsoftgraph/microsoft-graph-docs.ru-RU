---
title: Тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 12fe4ad670d2bb5056d05fde533d4b690068f7a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154217"
---
# <a name="authorizationpolicy-resource-type"></a>Тип ресурса authorizationPolicy

Пространство имен: microsoft.graph

Представляет политику, которая может управлять настройками авторизации Azure Active Directory. Это однотон, наследуется от базового типа политики и всегда существует для клиента.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Чтение объекта authorizationPolicy. |
| [Обновление authorizationPolicy](../api/authorizationpolicy-update.md) | Нет | Обновление объекта authorizationPolicy. |

## <a name="properties"></a>Свойства  
| Свойство | Тип | Описание | 
|-|-|-|
|id|String| ИД политики авторизации. Обязательно. Только для чтения.| 
|displayName|String| Отображаемого имени для этой политики. |  
|description|String| Описание этой политики.|  
|blockMsolPowerShell|Логическое| Чтобы отключить использование MSOL PowerShell, установите для этого свойства true. При установке true также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не влияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Логическое| Указывает, может ли функция Self-Serve сброса пароля может использоваться пользователями в клиенте. | 
|allowedToSignUpEmailBasedSubscriptions|Логическое| Указывает, могут ли пользователи зарегистрироваться для подписок на основе электронной почты. | 
|allowEmailVerifiedUsersToJoinOrganization|Логическое| Указывает, может ли пользователь присоединиться к клиенту по электронной почте. | 
|allowInvitesFrom|String|Указывает, кто может приглашать внешних пользователей в организацию. Возможные значения:<ul><li>`none` – Запретить всем, включая администраторов, приглашать внешних пользователей. Настройка по умолчанию для правительства США.</li><li>`adminsAndGuestInviters` - Разрешить участникам ролей глобальных администраторов, администраторов пользователей и приглашений гостей приглашать внешних пользователей.</li><li>`adminsGuestInvitersAndAllMembers` - Разрешить вышеуказанным ролям администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</li><li>`everyone` - Разрешить всем пользователям в организации, включая гостевых пользователей, приглашать внешних пользователей. Значение по умолчанию для всех облачных сред, кроме правительства США.</li></ul> |

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
