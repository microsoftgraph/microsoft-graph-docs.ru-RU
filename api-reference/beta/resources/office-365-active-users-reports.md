---
title: Отчеты об активных пользователях Office 365
description: Отчет активных пользователей Office 365 используется для получения числа лицензий продукта используются с пользователями в организации и детализации для получения сведений о том, какие пользователи используют какие продукты. В этом отчете может помочь администраторам определение использования продуктов или пользователей, которым могут понадобиться дополнительные учебные курсы или сведения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 638550fbc44acd0154a2dab5c062e2061fa9c582
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571767"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="a0aee-104">Отчеты об активных пользователях Office 365</span><span class="sxs-lookup"><span data-stu-id="a0aee-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0aee-105">Отчет активных пользователей Office 365 используется для получения числа лицензий продукта используются с пользователями в организации и детализации для получения сведений о том, какие пользователи используют какие продукты.</span><span class="sxs-lookup"><span data-stu-id="a0aee-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="a0aee-106">В этом отчете может помочь администраторам определение использования продуктов или пользователей, которым могут понадобиться дополнительные учебные курсы или сведения.</span><span class="sxs-lookup"><span data-stu-id="a0aee-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="a0aee-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="a0aee-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="a0aee-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="a0aee-108">Reports</span></span>
| <span data-ttu-id="a0aee-109">Функция</span><span class="sxs-lookup"><span data-stu-id="a0aee-109">Function</span></span>                                 | <span data-ttu-id="a0aee-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="a0aee-110">CSV return type</span></span> | <span data-ttu-id="a0aee-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="a0aee-111">JSON return type</span></span>                         | <span data-ttu-id="a0aee-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a0aee-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="a0aee-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="a0aee-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="a0aee-114">Stream</span><span class="sxs-lookup"><span data-stu-id="a0aee-114">Stream</span></span>          | [<span data-ttu-id="a0aee-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="a0aee-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="a0aee-116">Получите сведения об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="a0aee-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="a0aee-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="a0aee-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="a0aee-118">Stream</span><span class="sxs-lookup"><span data-stu-id="a0aee-118">Stream</span></span>          | [<span data-ttu-id="a0aee-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="a0aee-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="a0aee-120">Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a0aee-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="a0aee-121">Получение количества пользователей по службам</span><span class="sxs-lookup"><span data-stu-id="a0aee-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="a0aee-122">Поток</span><span class="sxs-lookup"><span data-stu-id="a0aee-122">Stream</span></span>          | [<span data-ttu-id="a0aee-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="a0aee-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="a0aee-124">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="a0aee-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
