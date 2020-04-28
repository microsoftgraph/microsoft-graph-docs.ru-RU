---
title: Тип ресурса Ролеманажемент
description: Ресурс управления ролями RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 71c9a12cec6fa58d60f71fe1adcf1af3715da1de
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215780"
---
# <a name="rolemanagement-resource-type"></a>Тип ресурса Ролеманажемент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект управления ролями Microsoft 365 RBAC. Предоставляет доступ к определениям ролей и назначениям ролей, предоставляемым поставщикам RBAC. В настоящее время поддерживается только поставщик каталогов. Для получения дополнительных сведений см. [разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="methods"></a>Methods

Нет

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|каталога|[рбакаппликатион](rbacapplication.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Нет

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
