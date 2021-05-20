---
title: Служба Privileged Identity Management
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory и ролями ресурсов Azure.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 31f19ab4c6dbb79c5bbf60c045b3367e2d819ee9
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546079"
---
# <a name="privileged-identity-management"></a>Управление привилегированными пользователями

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Служба Privileged Identity Management (PIM) в Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) позволяет контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им. Сюда входит доступ к ресурсам в Azure AD, ресурсам Azure и другим службам Microsoft Online Services, таким как Microsoft 365 или Microsoft Intune. В Microsoft Graph предусмотрены интерфейсы API, которые можно использовать для управления ролями Azure AD и ролями ресурсов Azure.

- [Интерфейсы API для ролей Azure AD](privilegedidentitymanagement-directory.md)
- [Интерфейсы API для ролей ресурсов Azure](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> Поддержка API для управления ролями Azure AD прекращается в большинстве клиентов, кроме нескольких, использующих более раннюю версию управления привилегированными пользователями (PIM). Дополнительные сведения о версиях PIM см. в разделе [Определение версии PIM](/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim). Если вы используете новую версию и у вас возникает ошибка **TenantEnabledInAadRoleMigration**, вы можете подождать появления нового API для функций PIM в API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) для ролей Azure AD или использовать API [ресурса Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true) для ролей Azure AD. Чтобы использовать API **ресурса Azure**, замените `azureResources` на `aadRoles` для `provider_id` и используйте свой идентификатор клиента для `resource_id`. Мы рекомендуем дождаться нового API. После появления нового API вы сможете продолжать использование API **ресурса Azure**. Кроме того, любые новые функции на портале Azure будут доступны только через новый API.

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
