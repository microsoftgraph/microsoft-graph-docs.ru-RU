---
title: Служба Privileged Identity Management
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory и ролями ресурсов Azure.
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 09d416ebe637a82f174b9668d4b9396626e0d5a3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695477"
---
# <a name="privileged-identity-management-deprecated"></a>Служба Privileged Identity Management (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>API Privileged Identity Management (PIM) для **ролей Azure AD** устарел и перестал возвращать данные 31 мая 2021 г. Используйте API [Управление ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true).
>
>API Privileged Identity Management (PIM) для **ролей ресурсов Azure** скоро выйдет из употребления. Используйте новый [REST API PIM Azure для ролей ресурсов Azure](/rest/api/authorization/role-eligibility-schedule-requests).

[Служба Privileged Identity Management (PIM) в Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) позволяет контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им. Сюда входит доступ к ресурсам в Azure AD, ресурсам Azure и другим службам Microsoft Online Services, таким как Microsoft 365 или Microsoft Intune.

В Microsoft Graph предусмотрены следующие интерфейсы API, которые можно использовать для управления ролями Azure AD и ролями ресурсов Azure.

- [Интерфейсы API для ролей Azure AD](privilegedidentitymanagement-directory.md)
- [Интерфейсы API для ролей ресурсов Azure](privilegedidentitymanagement-resources.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
