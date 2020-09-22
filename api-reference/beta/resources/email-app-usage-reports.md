---
title: Отчеты об использовании почтовых приложений
description: Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 03d33080a1d37512431c1922c217a8abe83a4828
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055521"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="fd3bb-104">Отчеты об использовании почтовых приложений</span><span class="sxs-lookup"><span data-stu-id="fd3bb-104">Email app usage reports</span></span>

<span data-ttu-id="fd3bb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd3bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd3bb-106">Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="fd3bb-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="fd3bb-107">Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.</span><span class="sxs-lookup"><span data-stu-id="fd3bb-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="fd3bb-108">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="fd3bb-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="fd3bb-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="fd3bb-109">Reports</span></span>

| <span data-ttu-id="fd3bb-110">Функция</span><span class="sxs-lookup"><span data-stu-id="fd3bb-110">Function</span></span>                                 | <span data-ttu-id="fd3bb-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="fd3bb-111">CSV return type</span></span> | <span data-ttu-id="fd3bb-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="fd3bb-112">JSON return type</span></span>                         | <span data-ttu-id="fd3bb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fd3bb-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="fd3bb-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="fd3bb-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="fd3bb-115">Stream</span><span class="sxs-lookup"><span data-stu-id="fd3bb-115">Stream</span></span>          | [<span data-ttu-id="fd3bb-116">емаилаппусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="fd3bb-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="fd3bb-117">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="fd3bb-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="fd3bb-118">Получение количества пользователей по приложениям</span><span class="sxs-lookup"><span data-stu-id="fd3bb-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="fd3bb-119">Поток</span><span class="sxs-lookup"><span data-stu-id="fd3bb-119">Stream</span></span>          | [<span data-ttu-id="fd3bb-120">емаилаппусажеаппсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="fd3bb-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="fd3bb-121">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="fd3bb-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="fd3bb-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="fd3bb-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="fd3bb-123">Stream</span><span class="sxs-lookup"><span data-stu-id="fd3bb-123">Stream</span></span>          | [<span data-ttu-id="fd3bb-124">емаилаппусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="fd3bb-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="fd3bb-125">Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="fd3bb-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="fd3bb-126">Получение количества пользователей по версиям</span><span class="sxs-lookup"><span data-stu-id="fd3bb-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="fd3bb-127">Поток</span><span class="sxs-lookup"><span data-stu-id="fd3bb-127">Stream</span></span>          | [<span data-ttu-id="fd3bb-128">емаилаппусажеверсионсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="fd3bb-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="fd3bb-129">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="fd3bb-129">Get the count of unique users by Outlook desktop version.</span></span> |


