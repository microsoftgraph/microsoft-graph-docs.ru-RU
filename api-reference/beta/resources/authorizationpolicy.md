---
title: Тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 42786b6813b0c433a073a7bbbb77615a3bafc564
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159943"
---
# <a name="authorizationpolicy-resource-type"></a>Тип ресурса authorizationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|guestUserRoleId|Guid| Представляет templateId роли, которая должна быть предоставлена гостевому пользователю. Список доступных шаблонов ролей можно найти в списке [unifiedRoleDefinitions.](../api/rbacapplication-list-roledefinitions.md) В настоящее время поддерживаются следующие роли: Пользователь (a0b1b346-4d3e-4e8b-98f8-753987be4970), гостевой пользователь (10dae51f-b6af-40 16-8d66-8c2a99b929b3) и ограниченный гостевой пользователь (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|enabledPreviewFeatures|Коллекция String| Список функций, включенных для закрытой предварительной версии в клиенте. | 
|blockMsolPowerShell|Boolean| Чтобы отключить использование MSOL PowerShell, установите для этого свойства true. При установке true также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не влияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Boolean| Указывает, может ли Self-Serve сброс паролей может использоваться пользователями в клиенте. | 
|allowedToSignUpEmailBasedSubscriptions|Boolean| Указывает, могут ли пользователи зарегистрироваться для подписок на основе электронной почты. | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| Указывает, может ли пользователь присоединиться к клиенту по электронной почте. | 
|allowInvitesFrom|String|Указывает, кто может приглашать внешних пользователей в организацию. Возможные значения:<ul><li>`none` – Запретить всем, включая администраторов, приглашать внешних пользователей. Параметр по умолчанию для правительства США.</li><li>`adminsAndGuestInviters` - Разрешить участникам ролей глобальных администраторов, администраторов пользователей и приглашений гостей приглашать внешних пользователей.</li><li>`adminsGuestInvitersAndAllMembers` - Разрешить вышеуказанным ролям администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</li><li>`everyone` - Разрешить всем пользователям в организации, включая гостевых пользователей, приглашать внешних пользователей. Настройка по умолчанию для всех облачных сред, кроме правительства США.</li></ul> |
|permissionGrantPolicyIdsAssignedToDefaultUserRole|Коллекция String|Указывает, разрешено ли согласие пользователя на доступ к приложениям, и, если да, какая политика согласия приложения (permissionGrantPolicy) управляет разрешением пользователей на предоставление согласия. Значения должны быть в формате , где находится ид встроенной или настраиваемой политики согласия `managePermissionGrantsForSelf.{id}` `{id}` [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies)  Пустой список указывает, что согласие пользователя на приложения отключено. |

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
