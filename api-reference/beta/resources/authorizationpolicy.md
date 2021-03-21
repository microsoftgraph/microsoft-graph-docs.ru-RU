---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3b52ba6c458a69a63135b00a9b53a717eef77091
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962107"
---
# <a name="authorizationpolicy-resource-type"></a>тип ресурса authorizationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять настройками авторизации Azure Active Directory. Это однотон, который наследуется от базового типа политики и всегда существует для клиента. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Ознакомьтесь с объектом authorizationPolicy. |
| [Обновление авторизацииPolicy](../api/authorizationpolicy-update.md) | Нет | Обновление объекта authorizationPolicy. |

## <a name="properties"></a>Свойства  
| Свойство | Тип | Описание | 
|-|-|-|
|id|Строка| ID политики авторизации. Обязательный. Только для чтения.| 
|displayName|Строка| Отображение имени для этой политики. |  
|description|Строка| Описание этой политики.|  
|guestUserRoleId|Guid| Представляет шаблон roleId для роли, которая должна быть предоставлена гостевому пользователю. Чтобы найти список доступных шаблонов ролей, обратитесь к list [unifiedRoleDefinitions.](../api/rbacapplication-list-roledefinitions.md) В настоящее время поддерживаются следующие роли: User `a0b1b346-4d3e-4e8b-98f8-753987be4970` (), Guest User `10dae51f-b6af-4016-8d66-8c2a99b929b3` () и Restricted Guest User `2af84b1e-32c8-42b7-82bc-daa82404023b` (). | 
|enabledPreviewFeatures|Коллекция строк| Список функций, включенных для личного предварительного просмотра в клиенте. | 
|blockMsolPowerShell|Boolean| Чтобы отключить использование MSOL PowerShell, установите это свойство true. Настройка true также отключит пользовательский доступ к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не влияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Boolean| Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента. | 
|allowedToSignUpEmailBasedSubscriptions|Boolean| Указывает, могут ли пользователи подписываться на подписки на основе электронной почты. | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 
|allowInvitesFrom|allowInvitesFrom|Указывает, кто может приглашать внешних пользователей в организацию. Возможные значения: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.  `everyone` — это параметр по умолчанию для всех облачных сред, за исключением правительства США. Подробнее в таблице [ниже](#allowinvitesfrom-values).|
|permissionGrantPolicyIdsAssignedToDefaultUserRole|Коллекция строк|Указывает, разрешено ли согласие пользователя на приложения, и если это так, какая политика согласия приложения (permissionGrantPolicy) регулирует разрешение для пользователей на предоставление согласия. Значения должны быть в формате , где находится id встроенной или настраиваемой политики согласия `managePermissionGrantsForSelf.{id}` `{id}` [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies)  Пустой список указывает, что согласие пользователя на приложения отключено. |

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
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": "[String]"
}
```
