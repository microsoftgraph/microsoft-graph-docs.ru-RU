---
title: Тип ресурса Аусоризатионполици
description: Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71e4d01ba54c9043ff827b3749be63442d06ac
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581250"
---
# <a name="authorizationpolicy-resource-type"></a>Тип ресурса Аусоризатионполици

Пространство имен: microsoft.graph

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
|блоккмсолповершелл|Логический| Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true. Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не повлияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](defaultuserrolepermissions.md)| Задает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Логический| Указывает, может ли функция сброса пароля Self-Serve использоваться пользователями клиента. | 
|allowedToSignUpEmailBasedSubscriptions|Логический| Указывает, могут ли пользователи регистрироваться на почтовые подписки. | 
|allowEmailVerifiedUsersToJoinOrganization|Логический| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 
|алловинвитесфром|String|Указывает, кто может приглашать внешних пользователей в Организации. Возможные значения:<ul><li>`none` — Запретить всем, в том числе администраторам, приглашать внешних пользователей. Настройка по умолчанию для государственных организаций США.</li><li>`adminsAndGuestInviters` — Разрешить членам группы "Администраторы", "Администраторы пользователей" и "гость" приглашать внешних пользователей.</li><li>`adminsGuestInvitersAndAllMembers` — Разрешить внешним пользователям приглашать этих ролей администратора и других участников роли пользователей.</li><li>`everyone` — Разрешить всем пользователям в Организации, в том числе гостям, приглашать внешних пользователей. Значение по умолчанию для всех облачных сред, кроме государственных организаций США.</li></ul> |

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
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```
