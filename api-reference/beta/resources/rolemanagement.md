---
title: тип ресурса roleManagement
description: Ресурс управления ролью RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 241de0b72a9ffad507975fca408fe49f0b0a90f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440131"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сущность управления ролью Microsoft 365 RBAC. Предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у поставщиков RBAC. В настоящее время поддерживаются поставщики каталогов (Azure AD) и deviceManagement (Intune). 

Дополнительные сведения см. в указанных ниже статьях. 
* [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* [Управление доступом на основе ролей (RBAC) с Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Methods

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|каталог|[rbacApplication](rbacapplication.md)| Только для чтения. Допускается значение null.|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| Только для чтения. Допускается значение null.|

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
