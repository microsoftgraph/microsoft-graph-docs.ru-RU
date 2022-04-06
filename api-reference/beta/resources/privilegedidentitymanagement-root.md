---
title: Служба Privileged Identity Management
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory и ролями ресурсов Azure.
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: governance
author: japere
ms.openlocfilehash: 241c9f44ac942ad9f3d67b030539f22425f86a14
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509247"
---
# <a name="privileged-identity-management-deprecated"></a>Служба Privileged Identity Management (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>API Privileged Identity Management (PIM) для **ролей Azure AD** устарел и перестал возвращать данные 31 мая 2021 г. Используйте API [управления ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) и см. ниже [руководство по миграции](#migrate-from-pim-v2-to-pim-v3-apis).
>
>API Privileged Identity Management (PIM) для **ресурсов Azure** скоро перестанет поддерживаться. Используйте новый [REST API PIM Azure для ресурсов Azure](/rest/api/authorization/role-eligibility-schedule-requests). Чтобы осуществить миграцию, см. ниже руководство по миграции.

Служба [Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) позволяет контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им. К этой области относится доступ к ресурсам в Azure AD, ресурсам Azure и другим службам Майкрософт, таким как Microsoft 365 или Microsoft Intune.

За последние несколько лет было несколько итераций API PIM. Эта итерация является второй (здесь она называется PIM версии 2), и ее заменяет PIM версии 3. Дополнительные сведения об истории API PIM см. в разделе [История версий API PIM](/azure/active-directory/privileged-identity-management/pim-apis#pim-api-history).

В Microsoft Graph предусмотрены следующие интерфейсы API PIM версии 2, которые можно использовать для управления ролями Azure AD и ролями ресурсов Azure. Рекомендуется перейти с PIM версии 2 на PIM версии 3.

- [API для ролей Azure AD](privilegedidentitymanagement-directory.md) (поддержка прекращена)
- [API для ресурсов Azure](privilegedidentitymanagement-resources.md)

## <a name="migrate-from-pim-v2-to-pim-v3-apis"></a>Переход с PIM версии 2 на API PIM версии 3

[!INCLUDE [pimv2AADRoles-migration](../../includes/pimv2AADRoles-migration.md)]

[!INCLUDE [pimv2AzureResources-migration](../../includes/pimv2AzureResources-migration.md)]

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
