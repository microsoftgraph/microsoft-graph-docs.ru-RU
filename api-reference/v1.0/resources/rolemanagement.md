---
title: тип ресурса roleManagement
description: Microsoft 365 управления доступом на основе ролей (RBAC).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 055e90c1fe006cf7babfdea4f7c585d66ff295d0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394511"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

Представляет собой Microsoft 365 управления ролями управления доступом (RBAC). Этот ресурс предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у поставщиков RBAC. **В настоящее** время поддерживаются поставщики каталогов (Azure Active Directory), **entitlementManagement** и **deviceManagement** (Intune).

Дополнительные сведения см. в указанных ниже статьях. 
* [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/roles/custom-overview).
* [Делегирования и ролей в управлении правами Azure AD](/azure/active-directory/governance/entitlement-management-delegate).
* [Управление доступом на основе ролей (RBAC) в Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|каталог|[rbacApplication](rbacapplication.md)| Только для чтения. Допускается значение null.|
|entitlementManagement|[rbacApplication](rbacapplication.md)| Контейнер для ролей и назначений для [ресурсов управления правами](entitlementmanagement.md) .|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```