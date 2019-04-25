---
title: Отчеты об активации Office 365
description: Отчет об активации Office 365 предоставляет представление о том, какие пользователи активировали подписки на Office 365 по крайней мере на одном устройстве. Он содержит сведения об активации подписки на Office 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581600"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="c568e-105">Отчеты об активации Office 365</span><span class="sxs-lookup"><span data-stu-id="c568e-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c568e-106">Отчет об активации Office 365 предоставляет представление о том, какие пользователи активировали подписки на Office 365 по крайней мере на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="c568e-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="c568e-107">Он содержит сведения об активации подписки на Office 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="c568e-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="c568e-108">Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.</span><span class="sxs-lookup"><span data-stu-id="c568e-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="c568e-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="c568e-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="c568e-110">Отчеты</span><span class="sxs-lookup"><span data-stu-id="c568e-110">Reports</span></span>
| <span data-ttu-id="c568e-111">Функция</span><span class="sxs-lookup"><span data-stu-id="c568e-111">Function</span></span>                                 | <span data-ttu-id="c568e-112">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="c568e-112">CSV return type</span></span> | <span data-ttu-id="c568e-113">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="c568e-113">JSON return type</span></span>                         | <span data-ttu-id="c568e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c568e-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="c568e-115">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="c568e-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="c568e-116">Stream</span><span class="sxs-lookup"><span data-stu-id="c568e-116">Stream</span></span>          | [<span data-ttu-id="c568e-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="c568e-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="c568e-118">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="c568e-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="c568e-119">Получение количества активаций</span><span class="sxs-lookup"><span data-stu-id="c568e-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="c568e-120">Поток</span><span class="sxs-lookup"><span data-stu-id="c568e-120">Stream</span></span>          | [<span data-ttu-id="c568e-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="c568e-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="c568e-122">Получите сведения о количестве активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="c568e-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="c568e-123">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="c568e-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="c568e-124">Поток</span><span class="sxs-lookup"><span data-stu-id="c568e-124">Stream</span></span>          | [<span data-ttu-id="c568e-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="c568e-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="c568e-126">Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="c568e-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
