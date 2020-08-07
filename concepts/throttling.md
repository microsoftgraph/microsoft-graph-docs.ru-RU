---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 71bb61a6bb2a72cc3e2cc4192e1a6d218ab4c3b4
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589181"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="8a7dc-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a7dc-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="8a7dc-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="8a7dc-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="8a7dc-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="8a7dc-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="8a7dc-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="8a7dc-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="8a7dc-119">Common throttling scenarios</span></span>

<span data-ttu-id="8a7dc-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="8a7dc-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="8a7dc-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="8a7dc-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="8a7dc-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="8a7dc-123">Best practices to handle throttling</span></span>

<span data-ttu-id="8a7dc-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="8a7dc-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="8a7dc-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="8a7dc-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="8a7dc-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="8a7dc-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="8a7dc-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-132">Retry the request.</span></span>
3. <span data-ttu-id="8a7dc-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="8a7dc-135">Все ресурсы и API, описанные в разделе [Ограничения для отдельных служб](#service-specific-limits), предоставляют заголовок `Retry-After`, если не указано иное.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-135">All the resources and APIs described in the [Service-specific limits](#service-specific-limits) section provide a `Retry-After` header except when noted.</span></span>

<span data-ttu-id="8a7dc-136">Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-136">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="8a7dc-137">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-137">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="8a7dc-138">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-138">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="8a7dc-139">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-139">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="8a7dc-140">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="8a7dc-140">Best practices to avoid throttling</span></span>

<span data-ttu-id="8a7dc-141">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-141">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="8a7dc-142">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-142">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="8a7dc-143">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-143">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="8a7dc-144">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="8a7dc-144">Service-specific limits</span></span>

<span data-ttu-id="8a7dc-145">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-145">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="8a7dc-146">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-146">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="8a7dc-147">Любой запрос можно оценивать с учетом нескольких ограничений, в зависимости от области применения ограничения (для каждого приложения во всех клиентах, по клиенту для всех приложений, для каждого приложения по отдельному клиенту и т. д.), типа запроса (GET, POST, PATCH и т. д.) и других факторов.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-147">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="8a7dc-148">Первое достигнутое ограничение запускает действие регулирования.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-148">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="8a7dc-149">Помимо специальных ограничений для служб, описанных в этом разделе, применяются следующие глобальные ограничения:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-149">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="8a7dc-150">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-150">Request type</span></span> | <span data-ttu-id="8a7dc-151">Для каждого приложения во всех клиентах</span><span class="sxs-lookup"><span data-stu-id="8a7dc-151">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="8a7dc-152">Любой</span><span class="sxs-lookup"><span data-stu-id="8a7dc-152">Any</span></span>          | <span data-ttu-id="8a7dc-153">2000 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-153">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="8a7dc-154">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-154">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="8a7dc-155">**Примечание.** В этом разделе термин *“клиент”* обозначает организацию Microsoft 365, в которой установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-155">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="8a7dc-156">Этот клиент может быть тем же самым, что и клиент, с которым создавалось приложение, в случае приложения с одним клиентом, или же он может отличаться в случае с [приложением, включающим несколько клиентов](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-156">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="8a7dc-157">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="8a7dc-157">Outlook service limits</span></span>

<span data-ttu-id="8a7dc-158">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-158">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="8a7dc-159">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-159">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="8a7dc-160">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-160">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="8a7dc-161">Указанные ниже ограничения относятся к общедоступному облаку, а также к [национальным облачным развертываниям](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-161">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="8a7dc-162">Ограничение</span><span class="sxs-lookup"><span data-stu-id="8a7dc-162">Limit</span></span>                                                      | <span data-ttu-id="8a7dc-163">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="8a7dc-163">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="8a7dc-164">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="8a7dc-164">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="8a7dc-165">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="8a7dc-165">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="8a7dc-166">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-166">4 concurrent requests</span></span>                                      | <span data-ttu-id="8a7dc-167">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="8a7dc-167">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="8a7dc-168">Отправка 15 мегабайт (МБ) (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-168">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="8a7dc-169">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="8a7dc-169">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="8a7dc-170">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="8a7dc-170">Outlook service resources</span></span>

<span data-ttu-id="8a7dc-171">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-171">The following resources are provided by the Outlook service.</span></span>

##### <a name="search-api-resources-preview"></a><span data-ttu-id="8a7dc-172">Ресурсы API поиска (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-172">Search API resources (preview)</span></span>

- [<span data-ttu-id="8a7dc-173">Внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-173">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a><span data-ttu-id="8a7dc-174">Ресурсы API профиля</span><span class="sxs-lookup"><span data-stu-id="8a7dc-174">Profile API resources</span></span>

- [<span data-ttu-id="8a7dc-175">Фотография</span><span class="sxs-lookup"><span data-stu-id="8a7dc-175">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a><span data-ttu-id="8a7dc-176">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="8a7dc-176">Calendar API resources</span></span>

- [<span data-ttu-id="8a7dc-177">event</span><span class="sxs-lookup"><span data-stu-id="8a7dc-177">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="8a7dc-178">eventMessage</span><span class="sxs-lookup"><span data-stu-id="8a7dc-178">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="8a7dc-179">calendar</span><span class="sxs-lookup"><span data-stu-id="8a7dc-179">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="8a7dc-180">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="8a7dc-180">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="8a7dc-181">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8a7dc-181">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="8a7dc-182">attachment</span><span class="sxs-lookup"><span data-stu-id="8a7dc-182">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="8a7dc-183">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-183">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="8a7dc-184">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="8a7dc-184">Mail API resources</span></span>

- [<span data-ttu-id="8a7dc-185">message</span><span class="sxs-lookup"><span data-stu-id="8a7dc-185">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="8a7dc-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="8a7dc-186">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="8a7dc-187">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="8a7dc-187">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="8a7dc-188">messageRule</span><span class="sxs-lookup"><span data-stu-id="8a7dc-188">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="8a7dc-189">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8a7dc-189">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="8a7dc-190">attachment</span><span class="sxs-lookup"><span data-stu-id="8a7dc-190">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="8a7dc-191">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="8a7dc-191">Personal contacts API resources</span></span>

- [<span data-ttu-id="8a7dc-192">contact</span><span class="sxs-lookup"><span data-stu-id="8a7dc-192">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="8a7dc-193">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8a7dc-193">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="8a7dc-194">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8a7dc-194">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="8a7dc-195">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="8a7dc-195">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="8a7dc-196">person</span><span class="sxs-lookup"><span data-stu-id="8a7dc-196">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="8a7dc-197">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-197">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="8a7dc-198">outlookTask</span><span class="sxs-lookup"><span data-stu-id="8a7dc-198">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="8a7dc-199">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8a7dc-199">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="8a7dc-200">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="8a7dc-200">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="8a7dc-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8a7dc-201">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="8a7dc-202">attachment</span><span class="sxs-lookup"><span data-stu-id="8a7dc-202">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="8a7dc-203">Ограничения службы облачного взаимодействия</span><span class="sxs-lookup"><span data-stu-id="8a7dc-203">Cloud communication service limits</span></span>

| <span data-ttu-id="8a7dc-204">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8a7dc-204">Resource</span></span>      | <span data-ttu-id="8a7dc-205">Ограничения на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="8a7dc-205">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="8a7dc-206">Звонки</span><span class="sxs-lookup"><span data-stu-id="8a7dc-206">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="8a7dc-207">10 000 звонков в месяц и 100 параллельных вызовов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-207">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="8a7dc-208">Сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="8a7dc-208">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="8a7dc-209">2000 собраний на пользователя каждый месяц</span><span class="sxs-lookup"><span data-stu-id="8a7dc-209">2000 meetings/user each month</span></span> |
| <span data-ttu-id="8a7dc-210">[Присутствие](/graph/api/resources/presence) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-210">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="8a7dc-211">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-211">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="8a7dc-212">Ограничения службы OneNote</span><span class="sxs-lookup"><span data-stu-id="8a7dc-212">OneNote service limits</span></span>

| <span data-ttu-id="8a7dc-213">Тип ограничения</span><span class="sxs-lookup"><span data-stu-id="8a7dc-213">Limit type</span></span> | <span data-ttu-id="8a7dc-214">Ограничение по приложению на каждого пользователя (делегированный контекст)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-214">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="8a7dc-215">Ограничение по приложению (контекст "только для приложений")</span><span class="sxs-lookup"><span data-stu-id="8a7dc-215">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="8a7dc-216">Частота запросов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-216">Requests rate</span></span> | <span data-ttu-id="8a7dc-217">120 запросов в 1 минуту и 400 запросов в 1 час</span><span class="sxs-lookup"><span data-stu-id="8a7dc-217">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="8a7dc-218">240 запросов в 1 минуту и 800 запросов в 1 час</span><span class="sxs-lookup"><span data-stu-id="8a7dc-218">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="8a7dc-219">Параллельные запросы</span><span class="sxs-lookup"><span data-stu-id="8a7dc-219">Concurrent requests</span></span> | <span data-ttu-id="8a7dc-220">5 параллельных запросов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-220">5 concurrent requests</span></span> | <span data-ttu-id="8a7dc-221">20 параллельных запросов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-221">20 concurrent requests</span></span> |

<span data-ttu-id="8a7dc-222">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-222">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="8a7dc-223">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="8a7dc-223">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="8a7dc-224">Дополнительные сведения о рекомендациях см. в статье [Регулирование в API OneNote и как его избежать](https://developer.microsoft.com/ru-RU/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-224">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/ru-RU/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="8a7dc-225">**Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-225">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="8a7dc-226">Ограничения службы Project Rome</span><span class="sxs-lookup"><span data-stu-id="8a7dc-226">Project Rome service limits</span></span>

| <span data-ttu-id="8a7dc-227">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-227">Request type</span></span> | <span data-ttu-id="8a7dc-228">Ограничение на каждого пользователя для всех приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-228">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="8a7dc-229">GET</span><span class="sxs-lookup"><span data-stu-id="8a7dc-229">GET</span></span>          | <span data-ttu-id="8a7dc-230">400 запросов в течение 5 минут и 12000 запросов в течение 1 дня</span><span class="sxs-lookup"><span data-stu-id="8a7dc-230">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="8a7dc-231">POST, PUT, PATCH, DELETE</span><span class="sxs-lookup"><span data-stu-id="8a7dc-231">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="8a7dc-232">100 запросов в течение 5 минут и 8000 запросов в течение 1 дня</span><span class="sxs-lookup"><span data-stu-id="8a7dc-232">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="8a7dc-233">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-233">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="8a7dc-234">activityHistoryItem, userActivity</span><span class="sxs-lookup"><span data-stu-id="8a7dc-234">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="8a7dc-235">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8a7dc-235">Microsoft Teams service limits</span></span>

<span data-ttu-id="8a7dc-236">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-236">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="8a7dc-237">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="8a7dc-237">Teams request type</span></span>                                   | <span data-ttu-id="8a7dc-238">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="8a7dc-238">Limit per app per tenant</span></span>        | <span data-ttu-id="8a7dc-239">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-239">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="8a7dc-240">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8a7dc-240">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="8a7dc-241">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="8a7dc-241">15000 requests every 10 seconds</span></span> | <span data-ttu-id="8a7dc-242">н/д</span><span class="sxs-lookup"><span data-stu-id="8a7dc-242">n/a</span></span> |
| <span data-ttu-id="8a7dc-243">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-243">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="8a7dc-244">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-244">60 rps</span></span>                          | <span data-ttu-id="8a7dc-245">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-245">600 rps</span></span> |
| <span data-ttu-id="8a7dc-246">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-246">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="8a7dc-247">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-247">30 rps</span></span>                         | <span data-ttu-id="8a7dc-248">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-248">300 rps</span></span>  |
| <span data-ttu-id="8a7dc-249">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-249">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="8a7dc-250">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-250">30 rps</span></span>                         | <span data-ttu-id="8a7dc-251">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-251">300 rps</span></span>  |
| <span data-ttu-id="8a7dc-252">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-252">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="8a7dc-253">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-253">15 rps</span></span>                         | <span data-ttu-id="8a7dc-254">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-254">150 rps</span></span>  |
| <span data-ttu-id="8a7dc-255">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="8a7dc-255">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="8a7dc-256">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-256">30 rps</span></span>                         | <span data-ttu-id="8a7dc-257">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-257">300 rps</span></span>  |
| <span data-ttu-id="8a7dc-258">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="8a7dc-258">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="8a7dc-259">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-259">6 rps</span></span> | <span data-ttu-id="8a7dc-260">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-260">150 rps</span></span>  | 
| <span data-ttu-id="8a7dc-261">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="8a7dc-261">GET channel message</span></span>  | <span data-ttu-id="8a7dc-262">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-262">5 rps</span></span> | <span data-ttu-id="8a7dc-263">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-263">100 rps</span></span> |
| <span data-ttu-id="8a7dc-264">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="8a7dc-264">GET 1:1/group chat message</span></span>  | <span data-ttu-id="8a7dc-265">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-265">3 rps</span></span> | <span data-ttu-id="8a7dc-266">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-266">30 rps</span></span> |
| <span data-ttu-id="8a7dc-267">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="8a7dc-267">POST channel message</span></span> | <span data-ttu-id="8a7dc-268">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-268">2 rps</span></span> | <span data-ttu-id="8a7dc-269">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-269">20 rps</span></span> |
| <span data-ttu-id="8a7dc-270">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="8a7dc-270">POST 1:1/group chat message</span></span> | <span data-ttu-id="8a7dc-271">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-271">2 rps</span></span> | <span data-ttu-id="8a7dc-272">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-272">20 rps</span></span> |
| <span data-ttu-id="8a7dc-273">GET /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="8a7dc-273">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="8a7dc-274">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-274">60 rps</span></span> | <span data-ttu-id="8a7dc-275">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-275">600 rps</span></span> |
| <span data-ttu-id="8a7dc-276">POST, PATCH, PUT /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="8a7dc-276">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="8a7dc-277">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-277">30 rps</span></span> | <span data-ttu-id="8a7dc-278">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-278">300 rps</span></span> |
| <span data-ttu-id="8a7dc-279">DELETE /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="8a7dc-279">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="8a7dc-280">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-280">15 rps</span></span> | <span data-ttu-id="8a7dc-281">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-281">150 rps</span></span> |

<span data-ttu-id="8a7dc-282">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-282">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="8a7dc-283">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-283">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="8a7dc-284">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-284">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

<span data-ttu-id="8a7dc-285">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-285">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="8a7dc-286">aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-286">aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.</span></span>

### <a name="information-protection"></a><span data-ttu-id="8a7dc-287">Защита информации</span><span class="sxs-lookup"><span data-stu-id="8a7dc-287">Information protection</span></span>

<span data-ttu-id="8a7dc-288">Указанные ниже ограничения применяются к любому запросу в `/informationProtection`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-288">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="8a7dc-289">Операция</span><span class="sxs-lookup"><span data-stu-id="8a7dc-289">Operation</span></span>                 | <span data-ttu-id="8a7dc-290">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="8a7dc-290">Limit per tenant</span></span>                                            | <span data-ttu-id="8a7dc-291">Ограничение на ресурс (электронная почта, URL-адрес, файл)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-291">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="8a7dc-292">POST</span><span class="sxs-lookup"><span data-stu-id="8a7dc-292">POST</span></span>                      | <span data-ttu-id="8a7dc-293">150 запросов в течение 15 минут и 10000 запросов в течение 24 часов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-293">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="8a7dc-294">1 запрос в течение 15 минут и 3 запроса в течение 24 часов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-294">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="8a7dc-295">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-295">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="8a7dc-296">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-296">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="8a7dc-297">Ограничения в отношении защиты удостоверений и службы условного доступа</span><span class="sxs-lookup"><span data-stu-id="8a7dc-297">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="8a7dc-298">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-298">Request type</span></span> | <span data-ttu-id="8a7dc-299">Ограничение на клиента для всех приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-299">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="8a7dc-300">Любой</span><span class="sxs-lookup"><span data-stu-id="8a7dc-300">Any</span></span> | <span data-ttu-id="8a7dc-301">1 запрос в секунду</span><span class="sxs-lookup"><span data-stu-id="8a7dc-301">1 request per second</span></span> |

<span data-ttu-id="8a7dc-302">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-302">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="8a7dc-303">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-303">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="8a7dc-304">**Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-304">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="8a7dc-305">Ограничения службы аналитики</span><span class="sxs-lookup"><span data-stu-id="8a7dc-305">Insights service limits</span></span>

<span data-ttu-id="8a7dc-306">Указанные ниже ограничения применяются к любому запросу в `me/insights` или `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-306">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="8a7dc-307">Ограничение</span><span class="sxs-lookup"><span data-stu-id="8a7dc-307">Limit</span></span>                                                      | <span data-ttu-id="8a7dc-308">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="8a7dc-308">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="8a7dc-309">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="8a7dc-309">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="8a7dc-310">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="8a7dc-310">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="8a7dc-311">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-311">4 concurrent requests</span></span>                                      | <span data-ttu-id="8a7dc-312">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="8a7dc-312">v1.0 and beta endpoints</span></span>   |

<span data-ttu-id="8a7dc-313">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-313">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="8a7dc-314">people, trending, usedinsight, sharedInsight.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-314">people, trending, usedinsight, sharedInsight.</span></span>

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="8a7dc-315">Ограничения службы отчетов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a7dc-315">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="8a7dc-316">Указанные ниже ограничения применяются к любому запросу в `/reports`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-316">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="8a7dc-317">Операция</span><span class="sxs-lookup"><span data-stu-id="8a7dc-317">Operation</span></span>                 | <span data-ttu-id="8a7dc-318">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="8a7dc-318">Limit per app per tenant</span></span>     | <span data-ttu-id="8a7dc-319">Ограничение на клиента для всех приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-319">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="8a7dc-320">Любой запрос (CSV)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-320">Any request (CSV)</span></span>         | <span data-ttu-id="8a7dc-321">14 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="8a7dc-321">14 requests per 10 minutes</span></span>   | <span data-ttu-id="8a7dc-322">40 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="8a7dc-322">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="8a7dc-323">Любой запрос (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="8a7dc-323">Any request (JSON, beta)</span></span>  | <span data-ttu-id="8a7dc-324">100 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="8a7dc-324">100 requests per 10 minutes</span></span>  | <span data-ttu-id="8a7dc-325">н/д</span><span class="sxs-lookup"><span data-stu-id="8a7dc-325">n/a</span></span>                        |

<span data-ttu-id="8a7dc-326">Указанные выше ограничения применяются по отдельности к каждому API отчетов.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-326">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="8a7dc-327">Например, запрос к API отчетов об активности пользователей Microsoft Teams и запрос к API отчетов об активности пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-327">For example, a request to the Microsoft Teams user activity report API and a request to the Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

<span data-ttu-id="8a7dc-328">Указанные выше ограничения применяются для ресурса **report**.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-328">The preceding limits apply to the **report** resource.</span></span>  

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="8a7dc-329">Ограничения службы диспетчера приглашений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-329">Invitation manager service limits</span></span>

<span data-ttu-id="8a7dc-330">Указанные ниже ограничения применяются к любому запросу в `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-330">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="8a7dc-331">Операция</span><span class="sxs-lookup"><span data-stu-id="8a7dc-331">Operation</span></span>                 | <span data-ttu-id="8a7dc-332">Ограничение на клиента для всех приложений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-332">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="8a7dc-333">Любая операция</span><span class="sxs-lookup"><span data-stu-id="8a7dc-333">Any operation</span></span>             | <span data-ttu-id="8a7dc-334">150 запросов за 5 секунд</span><span class="sxs-lookup"><span data-stu-id="8a7dc-334">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="8a7dc-335">Ограничения службы обнаружений и инцидентов безопасности</span><span class="sxs-lookup"><span data-stu-id="8a7dc-335">Security detections and incidents service limits</span></span>

<span data-ttu-id="8a7dc-336">Указанные ниже ограничения применяются к любому запросу в `/security`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-336">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="8a7dc-337">Операция</span><span class="sxs-lookup"><span data-stu-id="8a7dc-337">Operation</span></span>                  | <span data-ttu-id="8a7dc-338">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="8a7dc-338">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="8a7dc-339">Любые операции с `alert`, `securityActions`  `secureScore`</span><span class="sxs-lookup"><span data-stu-id="8a7dc-339">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="8a7dc-340">150 запросов в минуту</span><span class="sxs-lookup"><span data-stu-id="8a7dc-340">150 requests per minute</span></span>      |
| <span data-ttu-id="8a7dc-341">Любая операция с `tiIndicator`</span><span class="sxs-lookup"><span data-stu-id="8a7dc-341">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="8a7dc-342">1000 запросов в минуту</span><span class="sxs-lookup"><span data-stu-id="8a7dc-342">1000 requests per minute</span></span> |
| <span data-ttu-id="8a7dc-343">Любая операция с `secureScore` или `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="8a7dc-343">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="8a7dc-344">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="8a7dc-344">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="8a7dc-345">Любая операция с `secureScore` или `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="8a7dc-345">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="8a7dc-346">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-346">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="8a7dc-347">Ограничения службы для открытых расширений и расширений схемы</span><span class="sxs-lookup"><span data-stu-id="8a7dc-347">Open and schema extensions service limits</span></span>

| <span data-ttu-id="8a7dc-348">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-348">Request type</span></span> | <span data-ttu-id="8a7dc-349">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="8a7dc-349">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="8a7dc-350">Любой</span><span class="sxs-lookup"><span data-stu-id="8a7dc-350">Any</span></span>          | <span data-ttu-id="8a7dc-351">455 запросов в течение 10 секунд</span><span class="sxs-lookup"><span data-stu-id="8a7dc-351">455 requests per 10 seconds</span></span> |

<span data-ttu-id="8a7dc-352">Указанные выше ограничения действуют для следующих ресурсов: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post и user.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-352">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

### <a name="files-and-lists-service-limits"></a><span data-ttu-id="8a7dc-353">Ограничения службы для файлов и списков</span><span class="sxs-lookup"><span data-stu-id="8a7dc-353">Files and lists service limits</span></span>

<span data-ttu-id="8a7dc-354">Ограничения службы для OneDrive, OneDrive для бизнеса и SharePoint Online недоступны.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-354">Service limits for OneDrive, OneDrive for Business, and SharePoint Online are not available.</span></span> <span data-ttu-id="8a7dc-355">Подробнее см. в статье [Почему нельзя просто назвать точные пределы регулирования?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span><span class="sxs-lookup"><span data-stu-id="8a7dc-355">For more information, see [why can't you just tell me the exact throttling limits?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span></span>

<span data-ttu-id="8a7dc-356">Сведения, приведенные в этой статье, относятся к следующим ресурсам:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-356">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="8a7dc-357">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site и thumbnailSet.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-357">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site, and thumbnailSet.</span></span>

### <a name="tasks-and-plans-service-limits"></a><span data-ttu-id="8a7dc-358">Ограничения службы для задач и планов</span><span class="sxs-lookup"><span data-stu-id="8a7dc-358">Tasks and plans service limits</span></span>

<span data-ttu-id="8a7dc-359">Ограничения службы для Планировщика недоступны.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-359">Service limits for Planner are not available.</span></span>

<span data-ttu-id="8a7dc-360">Сведения, приведенные в этой статье, относятся к следующим ресурсам:</span><span class="sxs-lookup"><span data-stu-id="8a7dc-360">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="8a7dc-361">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails и plannerUser.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-361">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, and plannerUser.</span></span>

### <a name="identity-and-access-data-policy-operation-service-limits"></a><span data-ttu-id="8a7dc-362">Ограничения службы операций с политикой данных удостоверений и доступа</span><span class="sxs-lookup"><span data-stu-id="8a7dc-362">Identity and access data policy operation service limits</span></span>

| <span data-ttu-id="8a7dc-363">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="8a7dc-363">Request type</span></span> | <span data-ttu-id="8a7dc-364">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="8a7dc-364">Limit per tenant</span></span> |
| ------------ | ---------------- |
| <span data-ttu-id="8a7dc-365">POST для `exportPersonalData`</span><span class="sxs-lookup"><span data-stu-id="8a7dc-365">POST on `exportPersonalData`</span></span> | <span data-ttu-id="8a7dc-366">1000 запросов в день по любой теме и 100 запросов по теме в день</span><span class="sxs-lookup"><span data-stu-id="8a7dc-366">1000 requests per day for any subject and 100 per subject per day</span></span> |
| <span data-ttu-id="8a7dc-367">Любой другой запрос</span><span class="sxs-lookup"><span data-stu-id="8a7dc-367">Any other request</span></span> | <span data-ttu-id="8a7dc-368">10000 запросов в час</span><span class="sxs-lookup"><span data-stu-id="8a7dc-368">10000 requests per hour</span></span> |

<span data-ttu-id="8a7dc-369">Указанные выше ограничения действуют для следующих ресурсов: dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-369">The preceding limits apply to the following resources: dataPolicyOperation.</span></span>

> <span data-ttu-id="8a7dc-370">**Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="8a7dc-370">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="8a7dc-371">Ограничения службы для образования</span><span class="sxs-lookup"><span data-stu-id="8a7dc-371">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="8a7dc-372">Ограничения службы Excel</span><span class="sxs-lookup"><span data-stu-id="8a7dc-372">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="8a7dc-373">Ограничения службы журналов аудита удостоверения и доступа</span><span class="sxs-lookup"><span data-stu-id="8a7dc-373">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="8a7dc-374">Ограничения службы поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="8a7dc-374">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="8a7dc-375">Ограничения службы Intune</span><span class="sxs-lookup"><span data-stu-id="8a7dc-375">Intune service limits</span></span>

[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="skype-service-limits"></a><span data-ttu-id="8a7dc-376">Ограничения службы Skype</span><span class="sxs-lookup"><span data-stu-id="8a7dc-376">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="8a7dc-377">Ограничения службы подписки</span><span class="sxs-lookup"><span data-stu-id="8a7dc-377">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
