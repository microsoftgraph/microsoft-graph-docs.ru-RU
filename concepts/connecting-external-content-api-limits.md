---
title: Ограничения API соединителей Microsoft Graph
description: Ограничения API соединителей Microsoft Graph
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 6ab757d16a10f2291ad9bac5034e9fe7357a7188
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645968"
---
# <a name="microsoft-graph-connector-api-limits"></a><span data-ttu-id="320fc-103">Ограничения API соединителей Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="320fc-103">Microsoft Graph connector API limits</span></span>

<span data-ttu-id="320fc-104">В этом разделе описывается реализация и ограничения эксплуатации для соединителей Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="320fc-104">This topic describes implementation and operational limits for Microsoft Graph connectors.</span></span> <span data-ttu-id="320fc-105">При разработке соединителей помните об этих ограничениях.</span><span class="sxs-lookup"><span data-stu-id="320fc-105">Keep these limits in mind when designing connectors.</span></span>

## <a name="connection-limits"></a><span data-ttu-id="320fc-106">Ограничения подключений</span><span class="sxs-lookup"><span data-stu-id="320fc-106">Connection limits</span></span>

| <span data-ttu-id="320fc-107">**Ограничение**</span><span class="sxs-lookup"><span data-stu-id="320fc-107">**Limit**</span></span> | <span data-ttu-id="320fc-108">**Описание**</span><span class="sxs-lookup"><span data-stu-id="320fc-108">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="320fc-109">**10 подключений**</span><span class="sxs-lookup"><span data-stu-id="320fc-109">**10 connections**</span></span> | <span data-ttu-id="320fc-110">Максимальное количество ресурсов [подключений](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) на клиента Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="320fc-110">The maximum number of [connection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) resources per Microsoft 365 tenant.</span></span> |
| <span data-ttu-id="320fc-111">**700 000 элементов**</span><span class="sxs-lookup"><span data-stu-id="320fc-111">**700,000 items**</span></span> | <span data-ttu-id="320fc-112">Максимальное количество [элементов](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) на подключение.</span><span class="sxs-lookup"><span data-stu-id="320fc-112">The maximum number of [items](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) per connection.</span></span> |
| <span data-ttu-id="320fc-113">**70 ГБ**</span><span class="sxs-lookup"><span data-stu-id="320fc-113">**70 GB**</span></span> | <span data-ttu-id="320fc-114">Максимальное количество байтов подключения.</span><span class="sxs-lookup"><span data-stu-id="320fc-114">The maximum byte size of a connection.</span></span> |

## <a name="schema-limits"></a><span data-ttu-id="320fc-115">Ограничения схемы</span><span class="sxs-lookup"><span data-stu-id="320fc-115">Schema limits</span></span>

| <span data-ttu-id="320fc-116">**Ограничение**</span><span class="sxs-lookup"><span data-stu-id="320fc-116">**Limit**</span></span> | <span data-ttu-id="320fc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="320fc-117">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="320fc-118">**128 свойств**</span><span class="sxs-lookup"><span data-stu-id="320fc-118">**128 properties**</span></span> | <span data-ttu-id="320fc-119">Максимальное количество свойств, которые можно определить в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true), характеризующих данные, полученные через подключение.</span><span class="sxs-lookup"><span data-stu-id="320fc-119">The maximum number of properties that can be defined in a [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true), characterizing the data ingested through a connection.</span></span> |

## <a name="group-limits"></a><span data-ttu-id="320fc-120">Ограничения для групп</span><span class="sxs-lookup"><span data-stu-id="320fc-120">Group limits</span></span>

| <span data-ttu-id="320fc-121">**Ограничение**</span><span class="sxs-lookup"><span data-stu-id="320fc-121">**Limit**</span></span> | <span data-ttu-id="320fc-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="320fc-122">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="320fc-123">100,000</span><span class="sxs-lookup"><span data-stu-id="320fc-123">100,000</span></span> | <span data-ttu-id="320fc-124">Максимальное количество [внешних групп](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) на клиента Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="320fc-124">The maximum number of [external groups](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) per Microsoft 365 tenant.</span></span> |
| <span data-ttu-id="320fc-125">**1000 запросов/с**</span><span class="sxs-lookup"><span data-stu-id="320fc-125">**1000 requests/sec**</span></span> | <span data-ttu-id="320fc-126">Максимальное количество запросов, разрешенных в секунду в пороге[регулирования](#throttling) администрирования группы.</span><span class="sxs-lookup"><span data-stu-id="320fc-126">The maximum number of requests allowed per second in the group administration [throttling](#throttling) threshold.</span></span> |

## <a name="item-ingestion"></a><span data-ttu-id="320fc-127">Прием элементов</span><span class="sxs-lookup"><span data-stu-id="320fc-127">Item ingestion</span></span>

| <span data-ttu-id="320fc-128">**Ограничение**</span><span class="sxs-lookup"><span data-stu-id="320fc-128">**Limit**</span></span> | <span data-ttu-id="320fc-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="320fc-129">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="320fc-130">**4 элемента/с (250 МБ в час)**</span><span class="sxs-lookup"><span data-stu-id="320fc-130">**4 items/sec (250 MB/hour)**</span></span> | <span data-ttu-id="320fc-131">Ограничение пропускной способности для приема элементов через подключение.</span><span class="sxs-lookup"><span data-stu-id="320fc-131">The throughput limit to ingest items through a connection.</span></span> |
| <span data-ttu-id="320fc-132">**4 МБ**</span><span class="sxs-lookup"><span data-stu-id="320fc-132">**4 MB**</span></span> | <span data-ttu-id="320fc-133">Максимальный размер элемента; это ограничение применяется к телу запроса при [приеме и индексации элемента](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="320fc-133">The maximum size of an item; this limit applies to the request body when [ingesting and indexing an item](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span></span> |
| <span data-ttu-id="320fc-134">**Н/Д**</span><span class="sxs-lookup"><span data-stu-id="320fc-134">**N/A**</span></span> | <span data-ttu-id="320fc-135">Максимальный размер свойства.</span><span class="sxs-lookup"><span data-stu-id="320fc-135">The maximum size of a property.</span></span> |

## <a name="throttling"></a><span data-ttu-id="320fc-136">Регулирование</span><span class="sxs-lookup"><span data-stu-id="320fc-136">Throttling</span></span>

<span data-ttu-id="320fc-p102">При превышении порогового значения [регулирования](throttling.md) Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="320fc-p102">When a [throttling](throttling.md) threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>
