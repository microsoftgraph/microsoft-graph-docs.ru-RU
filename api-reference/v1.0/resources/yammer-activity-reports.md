---
title: Отчеты о действиях в Yammer
description: Благодаря отчетам о действиях в Yammer вы сможете узнать уровень активности использования этой сети в организации, просматривая количество действий, выполняемых в организации, и уникальных пользователей, которые публикуют, оценивают и читают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: b6f92ba4745d69cf2ce341412eee88403218414c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533361"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="c0c23-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="c0c23-103">Yammer activity reports</span></span>

<span data-ttu-id="c0c23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0c23-105">Благодаря отчетам о действиях в Yammer вы сможете узнать уровень активности использования этой сети в организации, просматривая количество действий, выполняемых в организации, и уникальных пользователей, которые публикуют, оценивают и читают сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="c0c23-105">You can use the Yammer activity reports to understand the level of your organization's engagement with Yammer by seeing how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="c0c23-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="c0c23-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="c0c23-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="c0c23-107">Reports</span></span>

| <span data-ttu-id="c0c23-108">Функция</span><span class="sxs-lookup"><span data-stu-id="c0c23-108">Function</span></span>                                 | <span data-ttu-id="c0c23-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0c23-109">Return Type</span></span> | <span data-ttu-id="c0c23-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c23-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="c0c23-111">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="c0c23-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="c0c23-112">Stream</span><span class="sxs-lookup"><span data-stu-id="c0c23-112">Stream</span></span>      | <span data-ttu-id="c0c23-113">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="c0c23-113">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="c0c23-114">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="c0c23-114">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="c0c23-115">Stream</span><span class="sxs-lookup"><span data-stu-id="c0c23-115">Stream</span></span>      | <span data-ttu-id="c0c23-116">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="c0c23-116">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="c0c23-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="c0c23-117">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="c0c23-118">Stream</span><span class="sxs-lookup"><span data-stu-id="c0c23-118">Stream</span></span>      | <span data-ttu-id="c0c23-119">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="c0c23-119">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
