---
title: тип ресурса roleManagement
description: Microsoft 365 управления доступом на основе ролей (RBAC).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6f28f6e682ebba03740e5cd07d17de838d2aea18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097934"
---
# <a name="rolemanagement-resource-type"></a>тип ресурса roleManagement

Пространство имен: microsoft.graph

Представляет собой Microsoft 365 управления ролями управления доступом (RBAC). Этот ресурс предоставляет доступ к определениям ролей и назначениям ролей, которые всплыли у поставщиков RBAC. **Поставщики** каталогов (Azure Active Directory) и **deviceManagement** (Intune) в настоящее время поддерживаются.

Подробнее: 
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