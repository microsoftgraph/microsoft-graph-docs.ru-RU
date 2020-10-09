---
title: Тип ресурса Аусоризатионполици
description: Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b12c026c38d5292de707b3a324746b77f38fe8f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402627"
---
# <a name="authorizationpolicy-resource-type"></a>Тип ресурса Аусоризатионполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять параметрами авторизации Azure Active Directory. Это одноэлементный экземпляр, который наследуется от базового типа политики и всегда существует для клиента. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Аусоризатионполици](../api/authorizationpolicy-get.md) | [аусоризатионполици](authorizationpolicy.md) | Чтение объекта Аусоризатионполици. |
| [Обновление Аусоризатионполици](../api/authorizationpolicy-update.md) | Нет | Обновление объекта Аусоризатионполици. |

## <a name="properties"></a>Свойства  
| Свойство | Тип | Описание | 
|-|-|-|
|id|String| Идентификатор политики авторизации. Обязательно. Только для чтения.| 
|displayName|String| Отображаемое имя для этой политики. |  
|description|String| Описание этой политики.|  
|гуестусерролеид|Guid| Представляет templateId роли для роли, которая должна быть выделена пользователю "гость". Обратитесь к [списку унифиедроледефинитионс](../api/rbacapplication-list-roledefinitions.md) , чтобы найти список доступных шаблонов ролей. В настоящее время поддерживаются следующие роли: пользователь (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и незащищенный гостевой пользователь (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|енабледпревиевфеатурес|Коллекция объектов string| Список компонентов, включенных для закрытой предварительной версии в клиенте. | 
|блоккмсолповершелл|Логический| Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true. Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не повлияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultUserRolePermissions.md)| Задает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Логический| Указывает, может ли функция сброса пароля Self-Serve использоваться пользователями клиента. | 
|allowedToSignUpEmailBasedSubscriptions|Логический| Указывает, могут ли пользователи регистрироваться на почтовые подписки. | 
|allowEmailVerifiedUsersToJoinOrganization|Логический| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 
|алловинвитесфром|String|Указывает, кто может приглашать внешних пользователей в Организации. Возможные значения:<ul><li>`none` — Запретить всем, в том числе администраторам, приглашать внешних пользователей. Настройка по умолчанию для государственных организаций США.</li><li>`adminsAndGuestInviters` — Разрешить членам группы "Администраторы", "Администраторы пользователей" и "гость" приглашать внешних пользователей.</li><li>`adminsGuestInvitersAndAllMembers` — Разрешить внешним пользователям приглашать этих ролей администратора и других участников роли пользователей.</li><li>`everyone` — Разрешить всем пользователям в Организации, в том числе гостям, приглашать внешних пользователей. Значение по умолчанию для всех облачных сред, кроме государственных организаций США.</li></ul> |
|пермиссионгрантполициидсассигнедтодефаултусерроле|Коллекция объектов string|Указывает, разрешено ли согласие пользователя на приложения, и, если это так, то, какая политика согласия приложений (Пермиссионгрантполици) управляет разрешением пользователей на предоставление согласия. Значения должны быть в формате `managePermissionGrantsForSelf.{id}` , где `{id}` — это **идентификатор** встроенной или настраиваемой [политики согласия приложений](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-app-consent-policies). Пустой список указывает на то, что согласие пользователя на приложения отключено. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
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
