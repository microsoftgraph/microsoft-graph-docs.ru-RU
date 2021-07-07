---
title: тип ресурса roleManagement
description: Ресурс управления ролью RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 42cad38bf690b6bb6958cfde99282f049a1a1d10
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317023"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет организацию Microsoft 365 ролей RBAC, которая предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у различных поставщиков RBAC. 

API управления единой ролью в настоящее время поддерживает следующих поставщиков RBAC в Microsoft 365:
- облачный КОМПЬЮТЕР 
- управление устройствами (Intune)
- directory (роли каталога Azure AD)
- управление правами (управление правами Azure AD)
 
Подробнее: 
* [Роли в Microsoft 365, в том числе Azure AD, роли для служб и межуслуковые](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* [Делегирования и ролей в управлении правами Azure AD.](/azure/active-directory/governance/entitlement-management-delegate)
* [Управление доступом на основе ролей (RBAC) в Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Methods

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|cloudPC|[rbacApplicationMultiple](rbacapplicationmultiple.md)|Предоставляет доступ к определениям ролей и назначениям ролей поставщика облачных ПК RBAC. Только для чтения. Допускается значение null.|
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
