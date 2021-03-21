---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 85af4636f52e49717e864f2ccb9d710fea313eb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962520"
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
|id|String| ID политики авторизации. Обязательный. Только для чтения.| 
|displayName|String| Отображение имени для этой политики. |  
|description|String| Описание этой политики.|  
|blockMsolPowerShell|Boolean| Чтобы отключить использование MSOL PowerShell, установите это свойство true. Настройка true также отключит пользовательский доступ к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не влияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Boolean| Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента. | 
|allowedToSignUpEmailBasedSubscriptions|Boolean| Указывает, могут ли пользователи подписываться на подписки на основе электронной почты. | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 
|allowInvitesFrom|allowInvitesFrom|Указывает, кто может приглашать внешних пользователей в организацию. Возможные значения: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.  `everyone` — это параметр по умолчанию для всех облачных сред, за исключением правительства США. Подробнее в таблице [ниже](#allowinvitesfrom-values). |

### <a name="allowinvitesfrom-values"></a>allowInvitesFrom values

|Member|Описание|
|:---|:---|
|Нет|Запретить всем, включая администраторов, приглашать внешних пользователей. Параметр по умолчанию для правительства США.|
|adminsAndGuestInviters|Разрешить участникам глобальных администраторов, администраторов пользователей и приглашенных приглашений приглашать внешних пользователей.|
|adminsGuestInvitersAndAllMembers|Разрешить вышеперечисленные роли администратора и всем другим участникам роли пользователя приглашать внешних пользователей.|
|все|Разрешить всем в организации, включая гостевых пользователей, приглашать внешних пользователей. Параметр по умолчанию для всех облачных сред, кроме правительства США.|

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
