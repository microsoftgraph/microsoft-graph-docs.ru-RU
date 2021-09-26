---
title: тип ресурса roleManagement
description: Ресурс управления ролью RBAC
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e401d0442c25ffcacb5887a0033c1d149ed51380
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766749"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет организацию Microsoft 365 ролей RBAC, которая предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у различных поставщиков RBAC. 

API управления единой ролью в настоящее время поддерживает следующих поставщиков RBAC в Microsoft 365:
- Облачный КОМПЬЮТЕР 
- управление устройствами (Intune)
- directory (роли каталога Azure AD)
- управление правами (управление правами Azure AD)
 
Дополнительные сведения см. в статьях: 
* [Роли в Microsoft 365, в том числе Azure AD, роли для служб и межуслуковые](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* [Делегирования и ролей в управлении правами Azure AD.](/azure/active-directory/governance/entitlement-management-delegate)
* [Управление доступом на основе ролей (RBAC) в Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|cloudPC|[rbacApplicationMultiple](rbacapplicationmultiple.md)|Предоставляет доступ к определениям ролей и назначениям ролей поставщика cloud PC RBAC. Только для чтения. Допускается значение null.|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| Предоставляет доступ к определениям ролей и назначениям ролей поставщика RBAC Intune. Только для чтения. Допускается значение null.|
|каталог|[rbacApplication](rbacapplication.md)|Предоставляет доступ к определениям ролей и назначениям ролей поставщика Azure AD RBAC. Только для чтения. Допускается значение null.|
|entitlementManagement|[rbacApplication](rbacapplication.md)| Предоставляет доступ к определениям ролей и назначениям ролей управления правами Azure AD. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Нет.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
