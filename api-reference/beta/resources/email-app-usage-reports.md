---
title: Отчеты об использовании почтовых приложений
description: Можно видеть, сколько приложений электронной почты используются для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: 92390033e544bc0163923e2bdad6e99212b66f92
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527782"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="2d8e6-104">Отчеты об использовании почтовых приложений</span><span class="sxs-lookup"><span data-stu-id="2d8e6-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d8e6-105">Можно видеть, сколько приложений электронной почты используются для подключения к Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2d8e6-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="2d8e6-106">Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.</span><span class="sxs-lookup"><span data-stu-id="2d8e6-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="2d8e6-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="2d8e6-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="2d8e6-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="2d8e6-108">Reports</span></span>

| <span data-ttu-id="2d8e6-109">Функция</span><span class="sxs-lookup"><span data-stu-id="2d8e6-109">Function</span></span>                                 | <span data-ttu-id="2d8e6-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="2d8e6-110">CSV return type</span></span> | <span data-ttu-id="2d8e6-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="2d8e6-111">JSON return type</span></span>                         | <span data-ttu-id="2d8e6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8e6-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2d8e6-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="2d8e6-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="2d8e6-114">Stream</span><span class="sxs-lookup"><span data-stu-id="2d8e6-114">Stream</span></span>          | [<span data-ttu-id="2d8e6-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="2d8e6-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="2d8e6-116">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="2d8e6-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="2d8e6-117">Получение количества пользователей по приложениям</span><span class="sxs-lookup"><span data-stu-id="2d8e6-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="2d8e6-118">Stream</span><span class="sxs-lookup"><span data-stu-id="2d8e6-118">Stream</span></span>          | [<span data-ttu-id="2d8e6-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="2d8e6-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="2d8e6-120">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="2d8e6-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="2d8e6-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="2d8e6-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="2d8e6-122">Stream</span><span class="sxs-lookup"><span data-stu-id="2d8e6-122">Stream</span></span>          | [<span data-ttu-id="2d8e6-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="2d8e6-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="2d8e6-124">Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="2d8e6-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="2d8e6-125">Получение количества пользователей по версиям</span><span class="sxs-lookup"><span data-stu-id="2d8e6-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="2d8e6-126">Поток</span><span class="sxs-lookup"><span data-stu-id="2d8e6-126">Stream</span></span>          | [<span data-ttu-id="2d8e6-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="2d8e6-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="2d8e6-128">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="2d8e6-128">Get the count of unique users by Outlook desktop version.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
