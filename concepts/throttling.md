---
title: Руководство по регулированию Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 12ae7bf122d23c6460dcbc253b1fe743768e49ba
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123717"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="feaac-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="feaac-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="feaac-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="feaac-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="feaac-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="feaac-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="feaac-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="feaac-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="feaac-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="feaac-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="feaac-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="feaac-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="feaac-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="feaac-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="feaac-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="feaac-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="feaac-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="feaac-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="feaac-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="feaac-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="feaac-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="feaac-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="feaac-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="feaac-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="feaac-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="feaac-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="feaac-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="feaac-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="feaac-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="feaac-119">Common throttling scenarios</span></span>

<span data-ttu-id="feaac-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="feaac-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="feaac-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="feaac-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="feaac-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="feaac-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="feaac-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="feaac-123">Best practices to handle throttling</span></span>

<span data-ttu-id="feaac-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="feaac-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="feaac-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="feaac-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="feaac-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="feaac-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="feaac-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="feaac-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="feaac-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="feaac-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="feaac-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="feaac-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="feaac-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="feaac-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="feaac-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="feaac-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="feaac-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="feaac-132">Retry the request.</span></span>
3. <span data-ttu-id="feaac-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="feaac-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="feaac-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="feaac-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="feaac-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="feaac-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="feaac-136">User</span><span class="sxs-lookup"><span data-stu-id="feaac-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="feaac-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="feaac-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="feaac-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="feaac-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="feaac-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="feaac-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="feaac-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="feaac-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="feaac-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="feaac-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="feaac-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="feaac-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="feaac-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="feaac-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="feaac-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="feaac-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="feaac-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="feaac-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="feaac-146">Отчет</span><span class="sxs-lookup"><span data-stu-id="feaac-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="feaac-147">Подписка</span><span class="sxs-lookup"><span data-stu-id="feaac-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="feaac-148">Популярное</span><span class="sxs-lookup"><span data-stu-id="feaac-148">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="feaac-149">Используемая аналитика</span><span class="sxs-lookup"><span data-stu-id="feaac-149">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="feaac-150">Совместная аналитика</span><span class="sxs-lookup"><span data-stu-id="feaac-150">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="feaac-151">Параметры пользователя</span><span class="sxs-lookup"><span data-stu-id="feaac-151">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="feaac-152">Приглашение</span><span class="sxs-lookup"><span data-stu-id="feaac-152">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="feaac-153">Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="feaac-153">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="feaac-154">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="feaac-154">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="feaac-155">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="feaac-155">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="feaac-156">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="feaac-156">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="feaac-157">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="feaac-157">Best practices to avoid throttling</span></span>

<span data-ttu-id="feaac-158">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="feaac-158">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="feaac-159">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="feaac-159">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="feaac-160">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="feaac-160">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="feaac-161">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="feaac-161">Service-specific limits</span></span>

<span data-ttu-id="feaac-162">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="feaac-162">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="feaac-163">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="feaac-163">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="feaac-164">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="feaac-164">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="feaac-165">**Примечание.** В этом разделе термин *“клиент”* обозначает организацию Microsoft 365, в которой установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="feaac-165">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="feaac-166">Этот клиент может быть тем же самым, что и клиент, с которым создавалось приложение, в случае приложения с одним клиентом, или же он может отличаться в случае с [приложением, включающим несколько клиентов](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="feaac-166">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="feaac-167">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="feaac-167">Outlook service limits</span></span>

<span data-ttu-id="feaac-168">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="feaac-168">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="feaac-169">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="feaac-169">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="feaac-170">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="feaac-170">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="feaac-171">Указанные ниже ограничения относятся к общедоступному облаку, а также к [национальным облачным развертываниям](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="feaac-171">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="feaac-172">Ограничение</span><span class="sxs-lookup"><span data-stu-id="feaac-172">Limit</span></span>                                                      | <span data-ttu-id="feaac-173">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="feaac-173">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="feaac-174">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="feaac-174">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="feaac-175">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="feaac-175">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="feaac-176">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="feaac-176">4 concurrent requests</span></span>                                      | <span data-ttu-id="feaac-177">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="feaac-177">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="feaac-178">Отправка 15 мегабайт (МБ) (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="feaac-178">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="feaac-179">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="feaac-179">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="feaac-180">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="feaac-180">Outlook service resources</span></span>

<span data-ttu-id="feaac-181">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="feaac-181">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="feaac-182">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="feaac-182">Calendar API resources</span></span>

- [<span data-ttu-id="feaac-183">event</span><span class="sxs-lookup"><span data-stu-id="feaac-183">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="feaac-184">eventMessage</span><span class="sxs-lookup"><span data-stu-id="feaac-184">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="feaac-185">calendar</span><span class="sxs-lookup"><span data-stu-id="feaac-185">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="feaac-186">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="feaac-186">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="feaac-187">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="feaac-187">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="feaac-188">attachment</span><span class="sxs-lookup"><span data-stu-id="feaac-188">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="feaac-189">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="feaac-189">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="feaac-190">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="feaac-190">Mail API resources</span></span>

- [<span data-ttu-id="feaac-191">message</span><span class="sxs-lookup"><span data-stu-id="feaac-191">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="feaac-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="feaac-192">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="feaac-193">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="feaac-193">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="feaac-194">messageRule</span><span class="sxs-lookup"><span data-stu-id="feaac-194">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="feaac-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="feaac-195">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="feaac-196">attachment</span><span class="sxs-lookup"><span data-stu-id="feaac-196">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="feaac-197">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="feaac-197">Personal contacts API resources</span></span>

- [<span data-ttu-id="feaac-198">contact</span><span class="sxs-lookup"><span data-stu-id="feaac-198">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="feaac-199">contactFolder</span><span class="sxs-lookup"><span data-stu-id="feaac-199">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="feaac-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="feaac-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="feaac-201">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="feaac-201">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="feaac-202">person</span><span class="sxs-lookup"><span data-stu-id="feaac-202">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="feaac-203">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="feaac-203">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="feaac-204">outlookTask</span><span class="sxs-lookup"><span data-stu-id="feaac-204">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="feaac-205">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="feaac-205">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="feaac-206">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="feaac-206">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="feaac-207">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="feaac-207">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="feaac-208">attachment</span><span class="sxs-lookup"><span data-stu-id="feaac-208">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="feaac-209">Ограничения службы облачного взаимодействия</span><span class="sxs-lookup"><span data-stu-id="feaac-209">Cloud communication service limits</span></span>

| <span data-ttu-id="feaac-210">Ресурс</span><span class="sxs-lookup"><span data-stu-id="feaac-210">Resource</span></span>      | <span data-ttu-id="feaac-211">Ограничения на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="feaac-211">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="feaac-212">Звонки</span><span class="sxs-lookup"><span data-stu-id="feaac-212">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="feaac-213">10 000 звонков в месяц и 100 параллельных вызовов</span><span class="sxs-lookup"><span data-stu-id="feaac-213">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="feaac-214">Сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="feaac-214">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="feaac-215">2000 собраний на пользователя каждый месяц</span><span class="sxs-lookup"><span data-stu-id="feaac-215">2000 meetings/user each month</span></span> |
| <span data-ttu-id="feaac-216">[Присутствие](/graph/api/resources/presence) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="feaac-216">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="feaac-217">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-217">2 rps</span></span> |

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="feaac-218">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="feaac-218">Microsoft Teams service limits</span></span>

<span data-ttu-id="feaac-219">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="feaac-219">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="feaac-220">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="feaac-220">Teams request type</span></span>                                   | <span data-ttu-id="feaac-221">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="feaac-221">Limit per app per tenant</span></span>        | <span data-ttu-id="feaac-222">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="feaac-222">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="feaac-223">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="feaac-223">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="feaac-224">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="feaac-224">15000 requests every 10 seconds</span></span> | <span data-ttu-id="feaac-225">н/д</span><span class="sxs-lookup"><span data-stu-id="feaac-225">n/a</span></span> |
| <span data-ttu-id="feaac-226">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="feaac-226">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="feaac-227">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-227">60 rps</span></span>                          | <span data-ttu-id="feaac-228">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-228">600 rps</span></span> |
| <span data-ttu-id="feaac-229">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="feaac-229">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="feaac-230">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-230">30 rps</span></span>                         | <span data-ttu-id="feaac-231">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-231">300 rps</span></span>  |
| <span data-ttu-id="feaac-232">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="feaac-232">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="feaac-233">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-233">30 rps</span></span>                         | <span data-ttu-id="feaac-234">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-234">300 rps</span></span>  |
| <span data-ttu-id="feaac-235">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="feaac-235">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="feaac-236">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-236">15 rps</span></span>                         | <span data-ttu-id="feaac-237">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-237">150 rps</span></span>  |
| <span data-ttu-id="feaac-238">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="feaac-238">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="feaac-239">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-239">30 rps</span></span>                         | <span data-ttu-id="feaac-240">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-240">300 rps</span></span>  |
| <span data-ttu-id="feaac-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="feaac-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="feaac-242">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-242">6 rps</span></span> | <span data-ttu-id="feaac-243">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-243">150 rps</span></span>  | 
| <span data-ttu-id="feaac-244">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="feaac-244">GET channel message</span></span>  | <span data-ttu-id="feaac-245">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-245">5 rps</span></span> | <span data-ttu-id="feaac-246">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-246">100 rps</span></span> |
| <span data-ttu-id="feaac-247">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="feaac-247">GET 1:1/group chat message</span></span>  | <span data-ttu-id="feaac-248">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-248">3 rps</span></span> | <span data-ttu-id="feaac-249">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-249">30 rps</span></span> |
| <span data-ttu-id="feaac-250">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="feaac-250">POST channel message</span></span> | <span data-ttu-id="feaac-251">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-251">2 rps</span></span> | <span data-ttu-id="feaac-252">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-252">20 rps</span></span> |
| <span data-ttu-id="feaac-253">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="feaac-253">POST 1:1/group chat message</span></span> | <span data-ttu-id="feaac-254">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-254">2 rps</span></span> | <span data-ttu-id="feaac-255">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-255">20 rps</span></span> |
| <span data-ttu-id="feaac-256">GET /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="feaac-256">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="feaac-257">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-257">60 rps</span></span> | <span data-ttu-id="feaac-258">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-258">600 rps</span></span> |
| <span data-ttu-id="feaac-259">POST, PATCH, PUT /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="feaac-259">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="feaac-260">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-260">30 rps</span></span> | <span data-ttu-id="feaac-261">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-261">300 rps</span></span> |
| <span data-ttu-id="feaac-262">DELETE /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="feaac-262">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="feaac-263">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-263">15 rps</span></span> | <span data-ttu-id="feaac-264">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-264">150 rps</span></span> |

<span data-ttu-id="feaac-265">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="feaac-265">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="feaac-266">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="feaac-266">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="feaac-267">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="feaac-267">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="feaac-268">Ограничения в отношении защиты удостоверений и службы условного доступа</span><span class="sxs-lookup"><span data-stu-id="feaac-268">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="feaac-269">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="feaac-269">Request type</span></span> | <span data-ttu-id="feaac-270">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="feaac-270">Limit per tenant</span></span> |
| ------------ | ------- |
| <span data-ttu-id="feaac-271">Любое</span><span class="sxs-lookup"><span data-stu-id="feaac-271">Any</span></span> | <span data-ttu-id="feaac-272">1 запрос в секунду</span><span class="sxs-lookup"><span data-stu-id="feaac-272">1 request per second</span></span> |

<span data-ttu-id="feaac-273">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="feaac-273">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="feaac-274">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="feaac-274">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="feaac-275">**Примечание.** В настоящее время перечисленные выше ресурсы не возвращают заголовок `Retry-After` в ответах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="feaac-275">**Note:** at the moment the resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>
### <a name="insights-service-limits"></a><span data-ttu-id="feaac-276">Ограничения службы аналитики</span><span class="sxs-lookup"><span data-stu-id="feaac-276">Insights service limits</span></span>

<span data-ttu-id="feaac-277">Указанные ниже ограничения применяются к любому запросу в `me/insights` или `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="feaac-277">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="feaac-278">Ограничение</span><span class="sxs-lookup"><span data-stu-id="feaac-278">Limit</span></span>                                                      | <span data-ttu-id="feaac-279">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="feaac-279">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="feaac-280">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="feaac-280">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="feaac-281">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="feaac-281">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="feaac-282">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="feaac-282">4 concurrent requests</span></span>                                      | <span data-ttu-id="feaac-283">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="feaac-283">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="feaac-284">Ограничения службы отчетов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="feaac-284">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="feaac-285">Указанные ниже ограничения применяются к любому запросу в `/reports`.</span><span class="sxs-lookup"><span data-stu-id="feaac-285">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="feaac-286">Операция</span><span class="sxs-lookup"><span data-stu-id="feaac-286">Operation</span></span>                 | <span data-ttu-id="feaac-287">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="feaac-287">Limit per app per tenant</span></span>     | <span data-ttu-id="feaac-288">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="feaac-288">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="feaac-289">Любой запрос (CSV)</span><span class="sxs-lookup"><span data-stu-id="feaac-289">Any request (CSV)</span></span>         | <span data-ttu-id="feaac-290">14 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="feaac-290">14 requests per 10 minutes</span></span>   | <span data-ttu-id="feaac-291">40 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="feaac-291">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="feaac-292">Любой запрос (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="feaac-292">Any request (JSON, beta)</span></span>  | <span data-ttu-id="feaac-293">100 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="feaac-293">100 requests per 10 minutes</span></span>  | <span data-ttu-id="feaac-294">н/д</span><span class="sxs-lookup"><span data-stu-id="feaac-294">n/a</span></span>                        |

<span data-ttu-id="feaac-295">Указанные выше ограничения применяются по отдельности к каждому API отчетов.</span><span class="sxs-lookup"><span data-stu-id="feaac-295">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="feaac-296">Например, запрос на API отчетов об активности пользователей Microsoft Teams и запрос на доступ к отчету об активности пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.</span><span class="sxs-lookup"><span data-stu-id="feaac-296">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="feaac-297">Ограничения службы диспетчера приглашений</span><span class="sxs-lookup"><span data-stu-id="feaac-297">Invitation manager service limits</span></span>

<span data-ttu-id="feaac-298">Указанные ниже ограничения применяются к любому запросу в `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="feaac-298">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="feaac-299">Операция</span><span class="sxs-lookup"><span data-stu-id="feaac-299">Operation</span></span>                 | <span data-ttu-id="feaac-300">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="feaac-300">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="feaac-301">Любая операция</span><span class="sxs-lookup"><span data-stu-id="feaac-301">Any operation</span></span>             | <span data-ttu-id="feaac-302">150 запросов за 5 секунд</span><span class="sxs-lookup"><span data-stu-id="feaac-302">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="feaac-303">Ограничения службы для образования</span><span class="sxs-lookup"><span data-stu-id="feaac-303">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="feaac-304">Ограничения службы Excel</span><span class="sxs-lookup"><span data-stu-id="feaac-304">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="feaac-305">Ограничения службы журналов аудита удостоверения и доступа</span><span class="sxs-lookup"><span data-stu-id="feaac-305">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="feaac-306">Ограничения службы поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="feaac-306">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="feaac-307">Ограничения службы Intune</span><span class="sxs-lookup"><span data-stu-id="feaac-307">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="feaac-308">Ограничения службы Skype</span><span class="sxs-lookup"><span data-stu-id="feaac-308">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="feaac-309">Ограничения службы подписки</span><span class="sxs-lookup"><span data-stu-id="feaac-309">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
