---
title: Тип ресурса Ролеманажемент
description: Ресурс управления ролями RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 71c59c1e44123b60dd46b2c72e71aabfc7a64c25
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991784"
---
# <a name="rolemanagement-resource-type"></a>Тип ресурса Ролеманажемент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект управления ролями Microsoft 365 RBAC. Предоставляет доступ к определениям ролей и назначениям ролей, предоставляемым поставщикам RBAC. В настоящее время поддерживаются поставщики Active Directory (Azure AD) и deviceManagement (Intune). 

Дополнительные сведения см. в статье: 
* [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* [Управление доступом на основе ролей (RBAC) в Microsoft Intune](https://docs.microsoft.com/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|каталога|[рбакаппликатион](rbacapplication.md)| Только для чтения. Допускается значение null.|
|deviceManagement|[рбакаппликатионмултипле](rbacapplicationmultiple.md)| Только для чтения. Допускается значение null.|

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
