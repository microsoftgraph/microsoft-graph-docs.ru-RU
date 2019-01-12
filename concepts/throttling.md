---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 8b3b8c5b0ec5a5209ad96f87dc677f4331c24e0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812645"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="4ce43-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4ce43-105">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="4ce43-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="4ce43-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="4ce43-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="4ce43-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="4ce43-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="4ce43-111">What happens when throttling occurs?</span></span>

<span data-ttu-id="4ce43-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="4ce43-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="4ce43-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="4ce43-119">Common throttling scenarios</span></span>

<span data-ttu-id="4ce43-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="4ce43-120">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="4ce43-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="4ce43-121">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="4ce43-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="4ce43-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="4ce43-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="4ce43-123">Best practices to handle throttling</span></span>

<span data-ttu-id="4ce43-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="4ce43-124">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="4ce43-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="4ce43-125">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="4ce43-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="4ce43-126">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="4ce43-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="4ce43-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="4ce43-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле *Retry-After*. Самый быстрый способ отключить регулирование — применить к запросам задержку *Retry-After*, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="4ce43-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the *Retry-After* field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="4ce43-131">Подождите столько секунд, сколько указано в поле *Retry-After*.</span><span class="sxs-lookup"><span data-stu-id="4ce43-131">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="4ce43-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="4ce43-132">Retry the request.</span></span>
3. <span data-ttu-id="4ce43-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку Retry-After, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="4ce43-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="4ce43-135">Заголовок Retry-After сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="4ce43-135">The following resources currently provide a retry-after header:</span></span>
- <span data-ttu-id="4ce43-136">[пользователь](/graph/api/resources/user?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-136">[User](/graph/api/resources/user?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="4ce43-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="4ce43-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="4ce43-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="4ce43-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="4ce43-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>

<span data-ttu-id="4ce43-145">Развернутое описание регулирования в Microsoft Cloud см. в [этой статье](https://msdn.microsoft.com/library/office/dn589798.aspx).</span><span class="sxs-lookup"><span data-stu-id="4ce43-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://msdn.microsoft.com/library/office/dn589798.aspx).</span></span>
