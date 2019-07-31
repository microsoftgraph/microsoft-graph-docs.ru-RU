---
title: Отчеты о действиях в Yammer
description: Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: efdb4ba603be33f18cd66529edd724f6e1a3798d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963833"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="2f4bc-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="2f4bc-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f4bc-104">Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="2f4bc-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="2f4bc-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="2f4bc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="2f4bc-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="2f4bc-106">Reports</span></span>

| <span data-ttu-id="2f4bc-107">Функция</span><span class="sxs-lookup"><span data-stu-id="2f4bc-107">Function</span></span>                                 | <span data-ttu-id="2f4bc-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="2f4bc-108">CSV return type</span></span> | <span data-ttu-id="2f4bc-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="2f4bc-109">JSON return type</span></span>                         | <span data-ttu-id="2f4bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f4bc-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2f4bc-111">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="2f4bc-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="2f4bc-112">Поток</span><span class="sxs-lookup"><span data-stu-id="2f4bc-112">Stream</span></span>          | [<span data-ttu-id="2f4bc-113">Яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="2f4bc-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="2f4bc-114">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="2f4bc-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="2f4bc-115">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="2f4bc-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="2f4bc-116">Stream</span><span class="sxs-lookup"><span data-stu-id="2f4bc-116">Stream</span></span>          | [<span data-ttu-id="2f4bc-117">Яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="2f4bc-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="2f4bc-118">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="2f4bc-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="2f4bc-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="2f4bc-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="2f4bc-120">Поток</span><span class="sxs-lookup"><span data-stu-id="2f4bc-120">Stream</span></span>          | [<span data-ttu-id="2f4bc-121">Яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="2f4bc-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="2f4bc-122">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="2f4bc-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
