---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cb35f7745a22a4a2eda43c48b3fc870ba1a88cce
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231590"
---
# <a name="authorizationpolicy-resource-type"></a>тип ресурса authorizationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять Azure Active Directory параметров авторизации. Это однотон, который наследуется от базового типа политики и всегда существует для клиента. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get authorizationPolicy](../api/authorizationpolicy-get.md) | [authorizationPolicy](authorizationpolicy.md) | Ознакомьтесь с объектом authorizationPolicy. |
| [Обновление авторизацииPolicy](../api/authorizationpolicy-update.md) | Нет | Обновление объекта authorizationPolicy. |

## <a name="properties"></a>Свойства  
| Свойство | Тип | Описание | 
|-|-|-|
|allowedToSignUpEmailBasedSubscriptions|Логический| Указывает, могут ли пользователи подписываться на подписки на основе электронной почты. | 
|allowedToUseSSPR|Логический| Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента. | 
|allowEmailVerifiedUsersToJoinOrganization|Логический| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 
|allowInvitesFrom|allowInvitesFrom|Указывает, кто может приглашать внешних пользователей в организацию. Возможные значения: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.  `everyone` — это параметр по умолчанию для всех облачных сред, за исключением правительства США. Дополнительные сведения см. в [таблице ниже](#allowinvitesfrom-values).|
|blockMsolPowerShell|Логический| Чтобы отключить использование MSOL PowerShell, установите это свойство `true` . Это также отключит доступ пользователей к конечной точке устаревшей службы, используемой MSOL PowerShell. Это не влияет на azure AD Подключение Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|description|String| Описание этой политики.|  
|displayName|String| Отображение имени для этой политики. |  
|enabledPreviewFeatures|Коллекция объектов string| Список функций, включенных для личного предварительного просмотра в клиенте. | 
|guestUserRoleId|Guid| Представляет шаблон roleId для роли, которая должна быть предоставлена гостевому пользователю. Чтобы найти список доступных шаблонов ролей, обратитесь к list [unifiedRoleDefinitions.](../api/rbacapplication-list-roledefinitions.md) В настоящее время поддерживаются следующие роли: User `a0b1b346-4d3e-4e8b-98f8-753987be4970` (), Guest User `10dae51f-b6af-4016-8d66-8c2a99b929b3` () и Restricted Guest User `2af84b1e-32c8-42b7-82bc-daa82404023b` (). | 
|id|String| ID политики авторизации. Обязательно. Только для чтения.| 
|permissionGrantPolicyIdsAssignedToDefaultUserRole|Коллекция объектов string|Указывает, разрешено ли согласие пользователя на приложения, и если это так, какая политика согласия приложения (permissionGrantPolicy) регулирует разрешение для пользователей на предоставление согласия. Значения должны быть в формате , где находится id встроенной или настраиваемой политики согласия `managePermissionGrantsForSelf.{id}` `{id}` [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies)  Пустой список указывает, что согласие пользователя на приложения отключено. |

### <a name="allowinvitesfrom-values"></a>allowInvitesFrom values

|Member|Описание|
|:---|:---|
|нет|Запретить всем, включая администраторов, приглашать внешних пользователей. Параметр по умолчанию для правительства США.|
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
