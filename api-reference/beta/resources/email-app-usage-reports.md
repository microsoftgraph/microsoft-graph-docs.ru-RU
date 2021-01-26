---
title: Отчеты об использовании почтовых приложений
description: Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: efa7a747ae26da8f34c32d9473a84f95b7433ee0
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982707"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="55d57-104">Отчеты об использовании почтовых приложений</span><span class="sxs-lookup"><span data-stu-id="55d57-104">Email app usage reports</span></span>

<span data-ttu-id="55d57-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55d57-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55d57-106">Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="55d57-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="55d57-107">Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.</span><span class="sxs-lookup"><span data-stu-id="55d57-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="55d57-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании почтовых приложений.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)</span><span class="sxs-lookup"><span data-stu-id="55d57-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="55d57-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="55d57-109">Reports</span></span>

| <span data-ttu-id="55d57-110">Функция</span><span class="sxs-lookup"><span data-stu-id="55d57-110">Function</span></span>                                 | <span data-ttu-id="55d57-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="55d57-111">CSV return type</span></span> | <span data-ttu-id="55d57-112">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="55d57-112">JSON return type</span></span>                         | <span data-ttu-id="55d57-113">Описание</span><span class="sxs-lookup"><span data-stu-id="55d57-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="55d57-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="55d57-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="55d57-115">Stream</span><span class="sxs-lookup"><span data-stu-id="55d57-115">Stream</span></span>          | [<span data-ttu-id="55d57-116">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="55d57-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="55d57-117">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="55d57-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="55d57-118">Получение количества пользователей по приложениям</span><span class="sxs-lookup"><span data-stu-id="55d57-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="55d57-119">Поток</span><span class="sxs-lookup"><span data-stu-id="55d57-119">Stream</span></span>          | [<span data-ttu-id="55d57-120">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="55d57-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="55d57-121">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="55d57-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="55d57-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="55d57-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="55d57-123">Stream</span><span class="sxs-lookup"><span data-stu-id="55d57-123">Stream</span></span>          | [<span data-ttu-id="55d57-124">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="55d57-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="55d57-125">Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="55d57-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="55d57-126">Получение количества пользователей по версиям</span><span class="sxs-lookup"><span data-stu-id="55d57-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="55d57-127">Поток</span><span class="sxs-lookup"><span data-stu-id="55d57-127">Stream</span></span>          | [<span data-ttu-id="55d57-128">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="55d57-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="55d57-129">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="55d57-129">Get the count of unique users by Outlook desktop version.</span></span> |


