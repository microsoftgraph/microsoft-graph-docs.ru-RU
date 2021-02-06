---
title: Служба Privileged Identity Management
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory и ролями ресурсов Azure.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: acea0d13baefebe5b42833ae1bd6968705ed1c3d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136236"
---
# <a name="privileged-identity-management"></a><span data-ttu-id="4e6db-103">Управление привилегированными пользователями</span><span class="sxs-lookup"><span data-stu-id="4e6db-103">Privileged Identity Management</span></span>

<span data-ttu-id="4e6db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e6db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6db-105">[Служба Privileged Identity Management (PIM) в Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) позволяет контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им.</span><span class="sxs-lookup"><span data-stu-id="4e6db-105">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="4e6db-106">Сюда входит доступ к ресурсам в Azure AD, ресурсам Azure и другим службам Microsoft Online Services, таким как Microsoft 365 или Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4e6db-106">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Microsoft 365 or Microsoft Intune.</span></span> <span data-ttu-id="4e6db-107">В Microsoft Graph предусмотрены интерфейсы API, которые можно использовать для управления ролями Azure AD и ролями ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="4e6db-107">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="4e6db-108">Интерфейсы API для ролей Azure AD</span><span class="sxs-lookup"><span data-stu-id="4e6db-108">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="4e6db-109">Интерфейсы API для ролей ресурсов Azure</span><span class="sxs-lookup"><span data-stu-id="4e6db-109">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="4e6db-110">Поддержка API для управления ролями Azure AD прекращается в большинстве клиентов, кроме нескольких, использующих более раннюю версию управления привилегированными пользователями (PIM).</span><span class="sxs-lookup"><span data-stu-id="4e6db-110">The API to manage Azure AD roles is deprecated for most tenants except for a few that use an older version of Privileged Identity Management (PIM).</span></span> <span data-ttu-id="4e6db-111">Дополнительные сведения о версиях PIM см. в разделе [Определение версии PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span><span class="sxs-lookup"><span data-stu-id="4e6db-111">For more information about PIM versions, see [Determine your version of PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span></span> <span data-ttu-id="4e6db-112">Если вы используете новую версию и у вас возникает ошибка **TenantEnabledInAadRoleMigration**, вы можете подождать появления нового API для функций PIM в API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) для ролей Azure AD или использовать API [ресурса Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) для ролей Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4e6db-112">If you are using the new version and are recieving a **TenantEnabledInAadRoleMigration** error, you can wait until a new API is available for PIM functionality under the [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) API for Azure AD roles, or you can use the [Azure Resource](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) API for your Azure AD roles.</span></span> <span data-ttu-id="4e6db-113">Чтобы использовать API **ресурса Azure**, замените `azureResources` на `aadRoles` для `provider_id` и используйте свой идентификатор клиента для `resource_id`.</span><span class="sxs-lookup"><span data-stu-id="4e6db-113">To use the **Azure resource** API, replace `azureResources` with `aadRoles` for `provider_id` and use your tenant id for `resource_id`.</span></span> <span data-ttu-id="4e6db-114">Мы рекомендуем дождаться нового API.</span><span class="sxs-lookup"><span data-stu-id="4e6db-114">We recommend that you wait for the new API.</span></span> <span data-ttu-id="4e6db-115">После появления нового API вы сможете продолжать использование API **ресурса Azure**.</span><span class="sxs-lookup"><span data-stu-id="4e6db-115">You will be able to continue using the **Azure resource** API after the new API is available.</span></span> <span data-ttu-id="4e6db-116">Кроме того, любые новые функции на портале Azure будут доступны только через новый API.</span><span class="sxs-lookup"><span data-stu-id="4e6db-116">Any new features made available in the Azure portal will also be made exclusively available through the new API.</span></span>

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
