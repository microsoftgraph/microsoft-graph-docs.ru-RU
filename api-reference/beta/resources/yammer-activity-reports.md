---
title: Отчеты о действиях в Yammer
description: Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f46ea743aed25a40d0894a003a11eae49b2829d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046094"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="abc0e-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="abc0e-103">Yammer activity reports</span></span>

<span data-ttu-id="abc0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc0e-105">Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="abc0e-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="abc0e-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Activity Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="abc0e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="abc0e-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="abc0e-107">Reports</span></span>

| <span data-ttu-id="abc0e-108">Функция</span><span class="sxs-lookup"><span data-stu-id="abc0e-108">Function</span></span>                                 | <span data-ttu-id="abc0e-109">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="abc0e-109">CSV return type</span></span> | <span data-ttu-id="abc0e-110">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="abc0e-110">JSON return type</span></span>                         | <span data-ttu-id="abc0e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="abc0e-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="abc0e-112">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="abc0e-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="abc0e-113">Stream</span><span class="sxs-lookup"><span data-stu-id="abc0e-113">Stream</span></span>          | [<span data-ttu-id="abc0e-114">яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="abc0e-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="abc0e-115">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="abc0e-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="abc0e-116">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="abc0e-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="abc0e-117">Stream</span><span class="sxs-lookup"><span data-stu-id="abc0e-117">Stream</span></span>          | [<span data-ttu-id="abc0e-118">яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="abc0e-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="abc0e-119">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="abc0e-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="abc0e-120">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="abc0e-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="abc0e-121">Stream</span><span class="sxs-lookup"><span data-stu-id="abc0e-121">Stream</span></span>          | [<span data-ttu-id="abc0e-122">яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="abc0e-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="abc0e-123">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="abc0e-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |


