---
title: Служба Privileged Identity Management
description: Интерфейсы API службы Azure AD Privileged Identity Management для управления ролями Azure Active Directory и ролями ресурсов Azure.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a4ca96d9296843fe716512f6d316d60f6c7b61d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965798"
---
# <a name="privileged-identity-management"></a><span data-ttu-id="4d4b9-103">Управление привилегированными пользователями (PIM)</span><span class="sxs-lookup"><span data-stu-id="4d4b9-103">Privileged Identity Management</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d4b9-104">[Служба Privileged Identity Management (PIM) в Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) позволяет контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им.</span><span class="sxs-lookup"><span data-stu-id="4d4b9-104">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="4d4b9-105">В частности, эти возможности поддерживаются для доступа к ресурсам в Azure AD, ресурсам Azure и других служб Microsoft Online Services, таких как Office 365 или Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4d4b9-105">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Office 365 or Microsoft Intune.</span></span> <span data-ttu-id="4d4b9-106">В Microsoft Graph предусмотрены интерфейсы API, которые можно использовать для управления ролями Azure AD и ролями ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="4d4b9-106">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="4d4b9-107">Интерфейсы API для ролей Azure AD</span><span class="sxs-lookup"><span data-stu-id="4d4b9-107">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="4d4b9-108">Интерфейсы API для ролей ресурсов Azure</span><span class="sxs-lookup"><span data-stu-id="4d4b9-108">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="4d4b9-109">Этот API для управления ролями Azure AD будет изменяться с июня по ноябрь 2019 года для соответствия пространству имен и соглашению для [интерфейсов API ресурсов Azure](privilegedidentitymanagement-resources.md).</span><span class="sxs-lookup"><span data-stu-id="4d4b9-109">The API to manage Azure AD roles will change between June and November of 2019 to follow the namespace and convention of the [Azure resource API](privilegedidentitymanagement-resources.md).</span></span> <span data-ttu-id="4d4b9-110">Служба Azure AD PIM станет ресурсом в соответствии с соглашением о ресурсах Azure.</span><span class="sxs-lookup"><span data-stu-id="4d4b9-110">Azure AD PIM will become a resource under the Azure resource convention.</span></span> <span data-ttu-id="4d4b9-111">Если это изменение непосредственно повлияет на ваш клиент, заполните [форму изменения интерфейса API Graph для Azure AD PIM](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u), чтобы получить дополнительные сведения, поддержку и возможность запланировать время для этого изменения API.</span><span class="sxs-lookup"><span data-stu-id="4d4b9-111">If this change will directly affect your tenant, please complete the [Graph API change for Azure AD PIM form](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u) to get additional information, support, and the ability to schedule a time for this API change.</span></span>

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
