---
title: Отчеты об активации Office 365
description: Отчет активации Office 365 позволяет представление, из которых пользователи активации Office 365 подписок на по крайней мере одно устройство. Предоставляет декомпозиции Office 365 ProPlus, Project и Visio Pro для активации подписки Office 365, а также декомпозиции активаций различных рабочего стола и устройств. В этом отчете может помочь определить пользователей, которые могут потребоваться дополнительную поддержку для активации подписки Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573681"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="6f513-105">Отчеты об активации Office 365</span><span class="sxs-lookup"><span data-stu-id="6f513-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f513-106">Отчет активации Office 365 позволяет представление, из которых пользователи активации Office 365 подписок на по крайней мере одно устройство.</span><span class="sxs-lookup"><span data-stu-id="6f513-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="6f513-107">Предоставляет декомпозиции Office 365 ProPlus, Project и Visio Pro для активации подписки Office 365, а также декомпозиции активаций различных рабочего стола и устройств.</span><span class="sxs-lookup"><span data-stu-id="6f513-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="6f513-108">В этом отчете может помочь определить пользователей, которые могут потребоваться дополнительную поддержку для активации подписки Office.</span><span class="sxs-lookup"><span data-stu-id="6f513-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="6f513-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="6f513-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="6f513-110">Отчеты</span><span class="sxs-lookup"><span data-stu-id="6f513-110">Reports</span></span>
| <span data-ttu-id="6f513-111">Функция</span><span class="sxs-lookup"><span data-stu-id="6f513-111">Function</span></span>                                 | <span data-ttu-id="6f513-112">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="6f513-112">CSV return type</span></span> | <span data-ttu-id="6f513-113">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="6f513-113">JSON return type</span></span>                         | <span data-ttu-id="6f513-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6f513-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6f513-115">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="6f513-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="6f513-116">Stream</span><span class="sxs-lookup"><span data-stu-id="6f513-116">Stream</span></span>          | [<span data-ttu-id="6f513-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="6f513-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="6f513-118">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="6f513-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="6f513-119">Получение количества активаций</span><span class="sxs-lookup"><span data-stu-id="6f513-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="6f513-120">Поток</span><span class="sxs-lookup"><span data-stu-id="6f513-120">Stream</span></span>          | [<span data-ttu-id="6f513-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="6f513-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="6f513-122">Получите сведения о количестве активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="6f513-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="6f513-123">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="6f513-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="6f513-124">Stream</span><span class="sxs-lookup"><span data-stu-id="6f513-124">Stream</span></span>          | [<span data-ttu-id="6f513-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="6f513-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="6f513-126">Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6f513-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
