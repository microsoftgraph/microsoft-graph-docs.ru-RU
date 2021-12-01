---
title: тип ресурса roleManagement
description: Microsoft 365 управления доступом на основе ролей (RBAC).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2836a8c4832d38c0e8c2e974d9eda7163c0f2313
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241655"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

Представляет собой Microsoft 365 управления ролями управления доступом (RBAC). Этот ресурс предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у поставщиков RBAC. **Поставщики** каталогов (Azure Active Directory) и **deviceManagement** (Intune) в настоящее время поддерживаются.

Дополнительные сведения см. в указанных ниже статьях. 
* [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/roles/custom-overview).
* [Управление доступом на основе ролей (RBAC) в Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|каталог|[rbacApplication](rbacapplication.md)| Только для чтения. Допускается значение null.|
|entitlementManagement|[entitlementManagement](entitlementmanagement.md)| Контейнер для всех ресурсов управления правами в управлении удостоверением Azure AD.|

## <a name="json-representation"></a>Представление JSON

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