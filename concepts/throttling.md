---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 32aa347085701234ffc08c5450aca480a1796e22
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183941"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="46216-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="46216-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="46216-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="46216-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="46216-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="46216-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="46216-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="46216-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="46216-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="46216-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="46216-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="46216-119">Common throttling scenarios</span></span>

<span data-ttu-id="46216-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="46216-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="46216-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="46216-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="46216-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="46216-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="46216-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="46216-123">Best practices to handle throttling</span></span>

<span data-ttu-id="46216-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="46216-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="46216-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="46216-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="46216-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="46216-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="46216-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="46216-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="46216-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="46216-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="46216-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="46216-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="46216-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="46216-132">Retry the request.</span></span>
3. <span data-ttu-id="46216-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="46216-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="46216-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="46216-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="46216-136">User</span><span class="sxs-lookup"><span data-stu-id="46216-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="46216-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="46216-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="46216-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="46216-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="46216-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="46216-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="46216-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="46216-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="46216-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="46216-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="46216-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="46216-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="46216-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="46216-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="46216-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="46216-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="46216-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46216-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="46216-146">Отчет</span><span class="sxs-lookup"><span data-stu-id="46216-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="46216-147">Подписка</span><span class="sxs-lookup"><span data-stu-id="46216-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="46216-148">Запрос на оценку угроз</span><span class="sxs-lookup"><span data-stu-id="46216-148">Threat assessment request</span></span>](/graph/api/resources/threatassessmentrequest)
- [<span data-ttu-id="46216-149">Запрос на оценку почты</span><span class="sxs-lookup"><span data-stu-id="46216-149">Mail assessment request</span></span>](/graph/api/resources/mailassessmentrequest)
- [<span data-ttu-id="46216-150">Запрос на оценку файла электронной почты</span><span class="sxs-lookup"><span data-stu-id="46216-150">Email file assessment request</span></span>](/graph/api/resources/emailfileassessmentrequest)
- [<span data-ttu-id="46216-151">Запрос на оценку файла</span><span class="sxs-lookup"><span data-stu-id="46216-151">File assessment request</span></span>](/graph/api/resources/fileassessmentrequest)
- [<span data-ttu-id="46216-152">Запрос на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="46216-152">URL assessment request</span></span>](/graph/api/resources/urlassessmentrequest)
- [<span data-ttu-id="46216-153">Результаты оценки угроз</span><span class="sxs-lookup"><span data-stu-id="46216-153">Threat assessment result</span></span>](/graph/api/resources/threatassessmentresult)
- [<span data-ttu-id="46216-154">Популярное</span><span class="sxs-lookup"><span data-stu-id="46216-154">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="46216-155">Используемая аналитика</span><span class="sxs-lookup"><span data-stu-id="46216-155">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="46216-156">Совместная аналитика</span><span class="sxs-lookup"><span data-stu-id="46216-156">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="46216-157">Параметры пользователя</span><span class="sxs-lookup"><span data-stu-id="46216-157">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="46216-158">Приглашение</span><span class="sxs-lookup"><span data-stu-id="46216-158">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="46216-159">Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="46216-159">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="46216-160">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="46216-160">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="46216-161">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="46216-161">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="46216-162">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="46216-162">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="46216-163">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="46216-163">Best practices to avoid throttling</span></span>

<span data-ttu-id="46216-164">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="46216-164">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="46216-165">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="46216-165">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="46216-166">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="46216-166">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="46216-167">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="46216-167">Service-specific limits</span></span>

<span data-ttu-id="46216-168">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="46216-168">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="46216-169">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="46216-169">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="46216-170">Любой запрос можно оценивать с учетом нескольких ограничений, в зависимости от области применения ограничения (для каждого приложения во всех клиентах, по клиенту для всех приложений, для каждого приложения по отдельному клиенту и т. д.), типа запроса (GET, POST, PATCH и т. д.) и других факторов.</span><span class="sxs-lookup"><span data-stu-id="46216-170">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="46216-171">Первое достигнутое ограничение запускает действие регулирования.</span><span class="sxs-lookup"><span data-stu-id="46216-171">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="46216-172">Помимо специальных ограничений для служб, описанных в этом разделе, применяются следующие глобальные ограничения:</span><span class="sxs-lookup"><span data-stu-id="46216-172">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="46216-173">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="46216-173">Request type</span></span> | <span data-ttu-id="46216-174">Для каждого приложения во всех клиентах</span><span class="sxs-lookup"><span data-stu-id="46216-174">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="46216-175">Любой</span><span class="sxs-lookup"><span data-stu-id="46216-175">Any</span></span>          | <span data-ttu-id="46216-176">2000 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-176">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="46216-177">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="46216-177">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="46216-178">**Примечание.** В этом разделе термин *“клиент”* обозначает организацию Microsoft 365, в которой установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="46216-178">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="46216-179">Этот клиент может быть тем же самым, что и клиент, с которым создавалось приложение, в случае приложения с одним клиентом, или же он может отличаться в случае с [приложением, включающим несколько клиентов](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="46216-179">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="46216-180">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="46216-180">Outlook service limits</span></span>

<span data-ttu-id="46216-181">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="46216-181">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="46216-182">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="46216-182">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="46216-183">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="46216-183">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="46216-184">Указанные ниже ограничения относятся к общедоступному облаку, а также к [национальным облачным развертываниям](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="46216-184">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="46216-185">Ограничение</span><span class="sxs-lookup"><span data-stu-id="46216-185">Limit</span></span>                                                      | <span data-ttu-id="46216-186">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="46216-186">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="46216-187">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="46216-187">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="46216-188">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="46216-188">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="46216-189">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="46216-189">4 concurrent requests</span></span>                                      | <span data-ttu-id="46216-190">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="46216-190">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="46216-191">Отправка 15 мегабайт (МБ) (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="46216-191">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="46216-192">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="46216-192">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="46216-193">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="46216-193">Outlook service resources</span></span>

<span data-ttu-id="46216-194">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="46216-194">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="46216-195">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="46216-195">Calendar API resources</span></span>

- [<span data-ttu-id="46216-196">event</span><span class="sxs-lookup"><span data-stu-id="46216-196">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="46216-197">eventMessage</span><span class="sxs-lookup"><span data-stu-id="46216-197">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="46216-198">calendar</span><span class="sxs-lookup"><span data-stu-id="46216-198">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="46216-199">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="46216-199">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="46216-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="46216-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="46216-201">attachment</span><span class="sxs-lookup"><span data-stu-id="46216-201">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="46216-202">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="46216-202">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="46216-203">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="46216-203">Mail API resources</span></span>

- [<span data-ttu-id="46216-204">message</span><span class="sxs-lookup"><span data-stu-id="46216-204">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="46216-205">mailFolder</span><span class="sxs-lookup"><span data-stu-id="46216-205">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="46216-206">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="46216-206">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="46216-207">messageRule</span><span class="sxs-lookup"><span data-stu-id="46216-207">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="46216-208">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="46216-208">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="46216-209">attachment</span><span class="sxs-lookup"><span data-stu-id="46216-209">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="46216-210">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="46216-210">Personal contacts API resources</span></span>

- [<span data-ttu-id="46216-211">contact</span><span class="sxs-lookup"><span data-stu-id="46216-211">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="46216-212">contactFolder</span><span class="sxs-lookup"><span data-stu-id="46216-212">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="46216-213">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="46216-213">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="46216-214">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="46216-214">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="46216-215">person</span><span class="sxs-lookup"><span data-stu-id="46216-215">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="46216-216">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="46216-216">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="46216-217">outlookTask</span><span class="sxs-lookup"><span data-stu-id="46216-217">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="46216-218">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="46216-218">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="46216-219">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="46216-219">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="46216-220">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="46216-220">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="46216-221">attachment</span><span class="sxs-lookup"><span data-stu-id="46216-221">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="46216-222">Ограничения службы облачного взаимодействия</span><span class="sxs-lookup"><span data-stu-id="46216-222">Cloud communication service limits</span></span>

| <span data-ttu-id="46216-223">Ресурс</span><span class="sxs-lookup"><span data-stu-id="46216-223">Resource</span></span>      | <span data-ttu-id="46216-224">Ограничения на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="46216-224">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="46216-225">Звонки</span><span class="sxs-lookup"><span data-stu-id="46216-225">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="46216-226">10 000 звонков в месяц и 100 параллельных вызовов</span><span class="sxs-lookup"><span data-stu-id="46216-226">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="46216-227">Сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="46216-227">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="46216-228">2000 собраний на пользователя каждый месяц</span><span class="sxs-lookup"><span data-stu-id="46216-228">2000 meetings/user each month</span></span> |
| <span data-ttu-id="46216-229">[Присутствие](/graph/api/resources/presence) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="46216-229">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="46216-230">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-230">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="46216-231">Ограничения службы OneNote</span><span class="sxs-lookup"><span data-stu-id="46216-231">OneNote service limits</span></span>

| <span data-ttu-id="46216-232">Тип ограничения</span><span class="sxs-lookup"><span data-stu-id="46216-232">Limit type</span></span> | <span data-ttu-id="46216-233">Ограничение по приложению на каждого пользователя (делегированный контекст)</span><span class="sxs-lookup"><span data-stu-id="46216-233">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="46216-234">Ограничение по приложению (контекст "только для приложений")</span><span class="sxs-lookup"><span data-stu-id="46216-234">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="46216-235">Частота запросов</span><span class="sxs-lookup"><span data-stu-id="46216-235">Requests rate</span></span> | <span data-ttu-id="46216-236">120 запросов в 1 минуту и 400 запросов в 1 час</span><span class="sxs-lookup"><span data-stu-id="46216-236">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="46216-237">240 запросов в 1 минуту и 800 запросов в 1 час</span><span class="sxs-lookup"><span data-stu-id="46216-237">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="46216-238">Параллельные запросы</span><span class="sxs-lookup"><span data-stu-id="46216-238">Concurrent requests</span></span> | <span data-ttu-id="46216-239">5 параллельных запросов</span><span class="sxs-lookup"><span data-stu-id="46216-239">5 concurrent requests</span></span> | <span data-ttu-id="46216-240">20 параллельных запросов</span><span class="sxs-lookup"><span data-stu-id="46216-240">20 concurrent requests</span></span> |

<span data-ttu-id="46216-241">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="46216-241">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="46216-242">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="46216-242">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="46216-243">Дополнительные сведения о рекомендациях см. в статье [Регулирование в API OneNote и как его избежать](https://developer.microsoft.com/ru-RU/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span><span class="sxs-lookup"><span data-stu-id="46216-243">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/ru-RU/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="46216-244">**Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="46216-244">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="46216-245">Ограничения службы Project Rome</span><span class="sxs-lookup"><span data-stu-id="46216-245">Project Rome service limits</span></span>

| <span data-ttu-id="46216-246">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="46216-246">Request type</span></span> | <span data-ttu-id="46216-247">Ограничение на каждого пользователя для всех приложений</span><span class="sxs-lookup"><span data-stu-id="46216-247">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="46216-248">GET</span><span class="sxs-lookup"><span data-stu-id="46216-248">GET</span></span>          | <span data-ttu-id="46216-249">400 запросов в течение 5 минут и 12000 запросов в течение 1 дня</span><span class="sxs-lookup"><span data-stu-id="46216-249">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="46216-250">POST, PUT, PATCH, DELETE</span><span class="sxs-lookup"><span data-stu-id="46216-250">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="46216-251">100 запросов в течение 5 минут и 8000 запросов в течение 1 дня</span><span class="sxs-lookup"><span data-stu-id="46216-251">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="46216-252">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="46216-252">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="46216-253">activityHistoryItem, userActivity</span><span class="sxs-lookup"><span data-stu-id="46216-253">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="46216-254">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="46216-254">Microsoft Teams service limits</span></span>

<span data-ttu-id="46216-255">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="46216-255">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="46216-256">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="46216-256">Teams request type</span></span>                                   | <span data-ttu-id="46216-257">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="46216-257">Limit per app per tenant</span></span>        | <span data-ttu-id="46216-258">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="46216-258">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="46216-259">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="46216-259">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="46216-260">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="46216-260">15000 requests every 10 seconds</span></span> | <span data-ttu-id="46216-261">н/д</span><span class="sxs-lookup"><span data-stu-id="46216-261">n/a</span></span> |
| <span data-ttu-id="46216-262">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="46216-262">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="46216-263">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-263">60 rps</span></span>                          | <span data-ttu-id="46216-264">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-264">600 rps</span></span> |
| <span data-ttu-id="46216-265">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="46216-265">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="46216-266">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-266">30 rps</span></span>                         | <span data-ttu-id="46216-267">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-267">300 rps</span></span>  |
| <span data-ttu-id="46216-268">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="46216-268">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="46216-269">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-269">30 rps</span></span>                         | <span data-ttu-id="46216-270">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-270">300 rps</span></span>  |
| <span data-ttu-id="46216-271">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="46216-271">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="46216-272">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-272">15 rps</span></span>                         | <span data-ttu-id="46216-273">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-273">150 rps</span></span>  |
| <span data-ttu-id="46216-274">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="46216-274">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="46216-275">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-275">30 rps</span></span>                         | <span data-ttu-id="46216-276">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-276">300 rps</span></span>  |
| <span data-ttu-id="46216-277">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="46216-277">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="46216-278">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-278">6 rps</span></span> | <span data-ttu-id="46216-279">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-279">150 rps</span></span>  | 
| <span data-ttu-id="46216-280">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="46216-280">GET channel message</span></span>  | <span data-ttu-id="46216-281">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-281">5 rps</span></span> | <span data-ttu-id="46216-282">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-282">100 rps</span></span> |
| <span data-ttu-id="46216-283">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="46216-283">GET 1:1/group chat message</span></span>  | <span data-ttu-id="46216-284">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-284">3 rps</span></span> | <span data-ttu-id="46216-285">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-285">30 rps</span></span> |
| <span data-ttu-id="46216-286">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="46216-286">POST channel message</span></span> | <span data-ttu-id="46216-287">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-287">2 rps</span></span> | <span data-ttu-id="46216-288">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-288">20 rps</span></span> |
| <span data-ttu-id="46216-289">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="46216-289">POST 1:1/group chat message</span></span> | <span data-ttu-id="46216-290">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-290">2 rps</span></span> | <span data-ttu-id="46216-291">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-291">20 rps</span></span> |
| <span data-ttu-id="46216-292">GET /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="46216-292">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="46216-293">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-293">60 rps</span></span> | <span data-ttu-id="46216-294">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-294">600 rps</span></span> |
| <span data-ttu-id="46216-295">POST, PATCH, PUT /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="46216-295">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="46216-296">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-296">30 rps</span></span> | <span data-ttu-id="46216-297">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-297">300 rps</span></span> |
| <span data-ttu-id="46216-298">DELETE /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="46216-298">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="46216-299">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-299">15 rps</span></span> | <span data-ttu-id="46216-300">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-300">150 rps</span></span> |

<span data-ttu-id="46216-301">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="46216-301">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="46216-302">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="46216-302">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="46216-303">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="46216-303">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="information-protection"></a><span data-ttu-id="46216-304">Защита информации</span><span class="sxs-lookup"><span data-stu-id="46216-304">Information protection</span></span>

<span data-ttu-id="46216-305">Указанные ниже ограничения применяются к любому запросу в `/informationProtection`.</span><span class="sxs-lookup"><span data-stu-id="46216-305">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="46216-306">Операция</span><span class="sxs-lookup"><span data-stu-id="46216-306">Operation</span></span>                 | <span data-ttu-id="46216-307">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="46216-307">Limit per tenant</span></span>                                            | <span data-ttu-id="46216-308">Ограничение на ресурс (электронная почта, URL-адрес, файл)</span><span class="sxs-lookup"><span data-stu-id="46216-308">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="46216-309">POST</span><span class="sxs-lookup"><span data-stu-id="46216-309">POST</span></span>                      | <span data-ttu-id="46216-310">150 запросов в течение 15 минут и 10000 запросов в течение 24 часов</span><span class="sxs-lookup"><span data-stu-id="46216-310">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="46216-311">1 запрос в течение 15 минут и 3 запроса в течение 24 часов</span><span class="sxs-lookup"><span data-stu-id="46216-311">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="46216-312">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="46216-312">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="46216-313">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span><span class="sxs-lookup"><span data-stu-id="46216-313">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="46216-314">Ограничения в отношении защиты удостоверений и службы условного доступа</span><span class="sxs-lookup"><span data-stu-id="46216-314">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="46216-315">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="46216-315">Request type</span></span> | <span data-ttu-id="46216-316">Ограничение на клиента для всех приложений</span><span class="sxs-lookup"><span data-stu-id="46216-316">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="46216-317">Любой</span><span class="sxs-lookup"><span data-stu-id="46216-317">Any</span></span> | <span data-ttu-id="46216-318">1 запрос в секунду</span><span class="sxs-lookup"><span data-stu-id="46216-318">1 request per second</span></span> |

<span data-ttu-id="46216-319">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="46216-319">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="46216-320">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="46216-320">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="46216-321">**Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="46216-321">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="46216-322">Ограничения службы аналитики</span><span class="sxs-lookup"><span data-stu-id="46216-322">Insights service limits</span></span>

<span data-ttu-id="46216-323">Указанные ниже ограничения применяются к любому запросу в `me/insights` или `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="46216-323">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="46216-324">Ограничение</span><span class="sxs-lookup"><span data-stu-id="46216-324">Limit</span></span>                                                      | <span data-ttu-id="46216-325">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="46216-325">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="46216-326">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="46216-326">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="46216-327">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="46216-327">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="46216-328">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="46216-328">4 concurrent requests</span></span>                                      | <span data-ttu-id="46216-329">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="46216-329">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="46216-330">Ограничения службы отчетов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="46216-330">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="46216-331">Указанные ниже ограничения применяются к любому запросу в `/reports`.</span><span class="sxs-lookup"><span data-stu-id="46216-331">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="46216-332">Операция</span><span class="sxs-lookup"><span data-stu-id="46216-332">Operation</span></span>                 | <span data-ttu-id="46216-333">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="46216-333">Limit per app per tenant</span></span>     | <span data-ttu-id="46216-334">Ограничение на клиента для всех приложений</span><span class="sxs-lookup"><span data-stu-id="46216-334">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="46216-335">Любой запрос (CSV)</span><span class="sxs-lookup"><span data-stu-id="46216-335">Any request (CSV)</span></span>         | <span data-ttu-id="46216-336">14 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="46216-336">14 requests per 10 minutes</span></span>   | <span data-ttu-id="46216-337">40 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="46216-337">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="46216-338">Любой запрос (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="46216-338">Any request (JSON, beta)</span></span>  | <span data-ttu-id="46216-339">100 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="46216-339">100 requests per 10 minutes</span></span>  | <span data-ttu-id="46216-340">н/д</span><span class="sxs-lookup"><span data-stu-id="46216-340">n/a</span></span>                        |

<span data-ttu-id="46216-341">Указанные выше ограничения применяются по отдельности к каждому API отчетов.</span><span class="sxs-lookup"><span data-stu-id="46216-341">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="46216-342">Например, запрос на API отчетов об активности пользователей Microsoft Teams и запрос на доступ к отчету об активности пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.</span><span class="sxs-lookup"><span data-stu-id="46216-342">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="46216-343">Ограничения службы диспетчера приглашений</span><span class="sxs-lookup"><span data-stu-id="46216-343">Invitation manager service limits</span></span>

<span data-ttu-id="46216-344">Указанные ниже ограничения применяются к любому запросу в `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="46216-344">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="46216-345">Операция</span><span class="sxs-lookup"><span data-stu-id="46216-345">Operation</span></span>                 | <span data-ttu-id="46216-346">Ограничение на клиента для всех приложений</span><span class="sxs-lookup"><span data-stu-id="46216-346">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="46216-347">Любая операция</span><span class="sxs-lookup"><span data-stu-id="46216-347">Any operation</span></span>             | <span data-ttu-id="46216-348">150 запросов за 5 секунд</span><span class="sxs-lookup"><span data-stu-id="46216-348">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="46216-349">Ограничения службы обнаружений и инцидентов безопасности</span><span class="sxs-lookup"><span data-stu-id="46216-349">Security detections and incidents service limits</span></span>

<span data-ttu-id="46216-350">Указанные ниже ограничения применяются к любому запросу в `/security`.</span><span class="sxs-lookup"><span data-stu-id="46216-350">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="46216-351">Операция</span><span class="sxs-lookup"><span data-stu-id="46216-351">Operation</span></span>                  | <span data-ttu-id="46216-352">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="46216-352">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="46216-353">Любые операции с `alert`, `securityActions`  `secureScore`</span><span class="sxs-lookup"><span data-stu-id="46216-353">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="46216-354">150 запросов в минуту</span><span class="sxs-lookup"><span data-stu-id="46216-354">150 requests per minute</span></span>      |
| <span data-ttu-id="46216-355">Любая операция с `tiIndicator`</span><span class="sxs-lookup"><span data-stu-id="46216-355">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="46216-356">1000 запросов в минуту</span><span class="sxs-lookup"><span data-stu-id="46216-356">1000 requests per minute</span></span> |
| <span data-ttu-id="46216-357">Любая операция с `secureScore` или `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="46216-357">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="46216-358">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="46216-358">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="46216-359">Любая операция с `secureScore` или `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="46216-359">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="46216-360">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="46216-360">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="46216-361">Ограничения службы для открытых расширений и расширений схемы</span><span class="sxs-lookup"><span data-stu-id="46216-361">Open and schema extensions service limits</span></span>

| <span data-ttu-id="46216-362">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="46216-362">Request type</span></span> | <span data-ttu-id="46216-363">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="46216-363">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="46216-364">Любой</span><span class="sxs-lookup"><span data-stu-id="46216-364">Any</span></span>          | <span data-ttu-id="46216-365">455 запросов в течение 10 секунд</span><span class="sxs-lookup"><span data-stu-id="46216-365">455 requests per 10 seconds</span></span> |

<span data-ttu-id="46216-366">Указанные выше ограничения действуют для следующих ресурсов: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post и user.</span><span class="sxs-lookup"><span data-stu-id="46216-366">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="46216-367">Ограничения службы для образования</span><span class="sxs-lookup"><span data-stu-id="46216-367">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="46216-368">Ограничения службы Excel</span><span class="sxs-lookup"><span data-stu-id="46216-368">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="46216-369">Ограничения службы журналов аудита удостоверения и доступа</span><span class="sxs-lookup"><span data-stu-id="46216-369">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="46216-370">Ограничения службы поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="46216-370">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="46216-371">Ограничения службы Intune</span><span class="sxs-lookup"><span data-stu-id="46216-371">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="46216-372">Ограничения службы Skype</span><span class="sxs-lookup"><span data-stu-id="46216-372">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="46216-373">Ограничения службы подписки</span><span class="sxs-lookup"><span data-stu-id="46216-373">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
