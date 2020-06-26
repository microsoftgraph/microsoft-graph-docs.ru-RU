---
title: Отчеты о действиях в Yammer
description: Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 6c431bf8bd72d2afb380d13c3cef310c2b1e672e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897087"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="ba0b0-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="ba0b0-103">Yammer activity reports</span></span>

<span data-ttu-id="ba0b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba0b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba0b0-105">Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="ba0b0-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="ba0b0-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Activity Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="ba0b0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="ba0b0-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="ba0b0-107">Reports</span></span>

| <span data-ttu-id="ba0b0-108">Функция</span><span class="sxs-lookup"><span data-stu-id="ba0b0-108">Function</span></span>                                 | <span data-ttu-id="ba0b0-109">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="ba0b0-109">CSV return type</span></span> | <span data-ttu-id="ba0b0-110">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="ba0b0-110">JSON return type</span></span>                         | <span data-ttu-id="ba0b0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba0b0-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ba0b0-112">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="ba0b0-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="ba0b0-113">Stream</span><span class="sxs-lookup"><span data-stu-id="ba0b0-113">Stream</span></span>          | [<span data-ttu-id="ba0b0-114">яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="ba0b0-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="ba0b0-115">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="ba0b0-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="ba0b0-116">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="ba0b0-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="ba0b0-117">Stream</span><span class="sxs-lookup"><span data-stu-id="ba0b0-117">Stream</span></span>          | [<span data-ttu-id="ba0b0-118">яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="ba0b0-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="ba0b0-119">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="ba0b0-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="ba0b0-120">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="ba0b0-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="ba0b0-121">Stream</span><span class="sxs-lookup"><span data-stu-id="ba0b0-121">Stream</span></span>          | [<span data-ttu-id="ba0b0-122">яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="ba0b0-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="ba0b0-123">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="ba0b0-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
