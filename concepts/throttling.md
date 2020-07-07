---
title: Руководство по регулированию Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5561e8a28440f05adcd074b6cd7d4d61edbb2852
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050787"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="644ac-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="644ac-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="644ac-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="644ac-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="644ac-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="644ac-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="644ac-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="644ac-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="644ac-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="644ac-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="644ac-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="644ac-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="644ac-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="644ac-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="644ac-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="644ac-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="644ac-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="644ac-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="644ac-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="644ac-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="644ac-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="644ac-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="644ac-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="644ac-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="644ac-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="644ac-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="644ac-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="644ac-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="644ac-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="644ac-119">Common throttling scenarios</span></span>

<span data-ttu-id="644ac-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="644ac-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="644ac-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="644ac-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="644ac-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="644ac-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="644ac-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="644ac-123">Best practices to handle throttling</span></span>

<span data-ttu-id="644ac-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="644ac-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="644ac-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="644ac-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="644ac-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="644ac-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="644ac-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="644ac-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="644ac-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="644ac-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="644ac-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="644ac-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="644ac-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="644ac-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="644ac-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="644ac-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="644ac-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="644ac-132">Retry the request.</span></span>
3. <span data-ttu-id="644ac-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="644ac-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="644ac-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="644ac-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="644ac-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="644ac-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="644ac-136">User</span><span class="sxs-lookup"><span data-stu-id="644ac-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="644ac-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="644ac-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="644ac-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="644ac-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="644ac-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="644ac-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="644ac-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="644ac-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="644ac-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="644ac-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="644ac-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="644ac-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="644ac-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="644ac-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="644ac-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="644ac-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="644ac-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="644ac-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="644ac-146">Report</span><span class="sxs-lookup"><span data-stu-id="644ac-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="644ac-147">Subscription</span><span class="sxs-lookup"><span data-stu-id="644ac-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="644ac-148">Популярные</span><span class="sxs-lookup"><span data-stu-id="644ac-148">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="644ac-149">Использованная аналитика</span><span class="sxs-lookup"><span data-stu-id="644ac-149">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="644ac-150">Общая информация</span><span class="sxs-lookup"><span data-stu-id="644ac-150">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="644ac-151">Параметры пользователя</span><span class="sxs-lookup"><span data-stu-id="644ac-151">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="644ac-152">Отправлен</span><span class="sxs-lookup"><span data-stu-id="644ac-152">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="644ac-153">Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="644ac-153">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="644ac-154">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="644ac-154">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="644ac-155">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="644ac-155">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="644ac-156">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="644ac-156">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="644ac-157">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="644ac-157">Best practices to avoid throttling</span></span>

<span data-ttu-id="644ac-158">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="644ac-158">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="644ac-159">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="644ac-159">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="644ac-160">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="644ac-160">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="644ac-161">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="644ac-161">Service-specific limits</span></span>

<span data-ttu-id="644ac-162">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="644ac-162">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="644ac-163">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="644ac-163">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="644ac-164">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="644ac-164">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="644ac-165">**Примечание:** В этом разделе термин " *клиент* " относится к организации Microsoft 365, в которой установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="644ac-165">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="644ac-166">Это может быть тот же клиент, что и в том случае, когда приложение было создано, в случае одного клиентского приложения, или оно может отличаться в случае [приложения с несколькими клиентами](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="644ac-166">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="644ac-167">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="644ac-167">Outlook service limits</span></span>

<span data-ttu-id="644ac-168">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="644ac-168">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="644ac-169">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="644ac-169">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="644ac-170">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="644ac-170">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="644ac-171">Следующие пределы применяются к общедоступному облаку, а также к [облачным облачным развертываниям](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="644ac-171">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="644ac-172">Ограничение</span><span class="sxs-lookup"><span data-stu-id="644ac-172">Limit</span></span>                                                      | <span data-ttu-id="644ac-173">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="644ac-173">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="644ac-174">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="644ac-174">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="644ac-175">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="644ac-175">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="644ac-176">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="644ac-176">4 concurrent requests</span></span>                                      | <span data-ttu-id="644ac-177">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="644ac-177">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="644ac-178">Загрузка 15 мегабайт (МБ) (исправление, POST, PUT) за 30-секундный период</span><span class="sxs-lookup"><span data-stu-id="644ac-178">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="644ac-179">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="644ac-179">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="644ac-180">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="644ac-180">Outlook service resources</span></span>

<span data-ttu-id="644ac-181">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="644ac-181">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="644ac-182">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="644ac-182">Calendar API resources</span></span>

- [<span data-ttu-id="644ac-183">event</span><span class="sxs-lookup"><span data-stu-id="644ac-183">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="644ac-184">eventMessage</span><span class="sxs-lookup"><span data-stu-id="644ac-184">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="644ac-185">calendar</span><span class="sxs-lookup"><span data-stu-id="644ac-185">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="644ac-186">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="644ac-186">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="644ac-187">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="644ac-187">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="644ac-188">attachment</span><span class="sxs-lookup"><span data-stu-id="644ac-188">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="644ac-189">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="644ac-189">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="644ac-190">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="644ac-190">Mail API resources</span></span>

- [<span data-ttu-id="644ac-191">message</span><span class="sxs-lookup"><span data-stu-id="644ac-191">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="644ac-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="644ac-192">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="644ac-193">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="644ac-193">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="644ac-194">messageRule</span><span class="sxs-lookup"><span data-stu-id="644ac-194">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="644ac-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="644ac-195">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="644ac-196">attachment</span><span class="sxs-lookup"><span data-stu-id="644ac-196">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="644ac-197">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="644ac-197">Personal contacts API resources</span></span>

- [<span data-ttu-id="644ac-198">contact</span><span class="sxs-lookup"><span data-stu-id="644ac-198">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="644ac-199">contactFolder</span><span class="sxs-lookup"><span data-stu-id="644ac-199">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="644ac-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="644ac-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="644ac-201">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="644ac-201">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="644ac-202">person</span><span class="sxs-lookup"><span data-stu-id="644ac-202">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="644ac-203">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="644ac-203">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="644ac-204">outlookTask</span><span class="sxs-lookup"><span data-stu-id="644ac-204">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="644ac-205">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="644ac-205">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="644ac-206">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="644ac-206">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="644ac-207">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="644ac-207">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="644ac-208">attachment</span><span class="sxs-lookup"><span data-stu-id="644ac-208">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="644ac-209">Пределы облачных служб связи</span><span class="sxs-lookup"><span data-stu-id="644ac-209">Cloud communication service limits</span></span>

| <span data-ttu-id="644ac-210">Ресурс</span><span class="sxs-lookup"><span data-stu-id="644ac-210">Resource</span></span>      | <span data-ttu-id="644ac-211">Максимальное число приложений для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="644ac-211">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="644ac-212">Звонки</span><span class="sxs-lookup"><span data-stu-id="644ac-212">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="644ac-213">10 000 звонков/мес и 100 одновременные вызовы</span><span class="sxs-lookup"><span data-stu-id="644ac-213">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="644ac-214">Сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="644ac-214">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="644ac-215">2000 собраний и пользователей в месяц</span><span class="sxs-lookup"><span data-stu-id="644ac-215">2000 meetings/user each month</span></span> |
| <span data-ttu-id="644ac-216">[Присутствие](/graph/api/resources/presence) (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="644ac-216">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="644ac-217">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-217">2 rps</span></span> |

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="644ac-218">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="644ac-218">Microsoft Teams service limits</span></span>

<span data-ttu-id="644ac-219">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="644ac-219">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="644ac-220">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="644ac-220">Teams request type</span></span>                                   | <span data-ttu-id="644ac-221">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="644ac-221">Limit per app per tenant</span></span>        | <span data-ttu-id="644ac-222">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="644ac-222">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="644ac-223">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="644ac-223">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="644ac-224">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="644ac-224">15000 requests every 10 seconds</span></span> | <span data-ttu-id="644ac-225">н/д</span><span class="sxs-lookup"><span data-stu-id="644ac-225">n/a</span></span> |
| <span data-ttu-id="644ac-226">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="644ac-226">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="644ac-227">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-227">60 rps</span></span>                          | <span data-ttu-id="644ac-228">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-228">600 rps</span></span> |
| <span data-ttu-id="644ac-229">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="644ac-229">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="644ac-230">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-230">30 rps</span></span>                         | <span data-ttu-id="644ac-231">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-231">300 rps</span></span>  |
| <span data-ttu-id="644ac-232">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="644ac-232">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="644ac-233">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-233">30 rps</span></span>                         | <span data-ttu-id="644ac-234">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-234">300 rps</span></span>  |
| <span data-ttu-id="644ac-235">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="644ac-235">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="644ac-236">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-236">15 rps</span></span>                         | <span data-ttu-id="644ac-237">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-237">150 rps</span></span>  |
| <span data-ttu-id="644ac-238">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="644ac-238">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="644ac-239">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-239">30 rps</span></span>                         | <span data-ttu-id="644ac-240">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-240">300 rps</span></span>  |
| <span data-ttu-id="644ac-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="644ac-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="644ac-242">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-242">6 rps</span></span> | <span data-ttu-id="644ac-243">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-243">150 rps</span></span>  | 
| <span data-ttu-id="644ac-244">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="644ac-244">GET channel message</span></span>  | <span data-ttu-id="644ac-245">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-245">5 rps</span></span> | <span data-ttu-id="644ac-246">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-246">100 rps</span></span> |
| <span data-ttu-id="644ac-247">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="644ac-247">GET 1:1/group chat message</span></span>  | <span data-ttu-id="644ac-248">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-248">3 rps</span></span> | <span data-ttu-id="644ac-249">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-249">30 rps</span></span> |
| <span data-ttu-id="644ac-250">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="644ac-250">POST channel message</span></span> | <span data-ttu-id="644ac-251">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-251">2 rps</span></span> | <span data-ttu-id="644ac-252">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-252">20 rps</span></span> |
| <span data-ttu-id="644ac-253">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="644ac-253">POST 1:1/group chat message</span></span> | <span data-ttu-id="644ac-254">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-254">2 rps</span></span> | <span data-ttu-id="644ac-255">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-255">20 rps</span></span> |
| <span data-ttu-id="644ac-256">ПОЛУЧЕНИЕ/Teams/ ```{team-id}``` /счедуле и всех API по этому пути</span><span class="sxs-lookup"><span data-stu-id="644ac-256">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="644ac-257">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-257">60 rps</span></span> | <span data-ttu-id="644ac-258">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-258">600 rps</span></span> |
| <span data-ttu-id="644ac-259">POST, PATCH, PUT/Teams/ ```{team-id}``` /счедуле и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="644ac-259">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="644ac-260">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-260">30 rps</span></span> | <span data-ttu-id="644ac-261">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-261">300 rps</span></span> |
| <span data-ttu-id="644ac-262">Удалите/Teams/ ```{team-id}``` /счедуле и все API, расположенные по этому пути</span><span class="sxs-lookup"><span data-stu-id="644ac-262">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="644ac-263">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-263">15 rps</span></span> | <span data-ttu-id="644ac-264">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="644ac-264">150 rps</span></span> |

<span data-ttu-id="644ac-265">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="644ac-265">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="644ac-266">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="644ac-266">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="644ac-267">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="644ac-267">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="644ac-268">Пределы службы аналитики</span><span class="sxs-lookup"><span data-stu-id="644ac-268">Insights service limits</span></span>

<span data-ttu-id="644ac-269">Следующие пределы применяются к запросам на `me/insights` или `users/{id}/insights` .</span><span class="sxs-lookup"><span data-stu-id="644ac-269">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="644ac-270">Ограничение</span><span class="sxs-lookup"><span data-stu-id="644ac-270">Limit</span></span>                                                      | <span data-ttu-id="644ac-271">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="644ac-271">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="644ac-272">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="644ac-272">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="644ac-273">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="644ac-273">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="644ac-274">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="644ac-274">4 concurrent requests</span></span>                                      | <span data-ttu-id="644ac-275">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="644ac-275">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="644ac-276">Пределы службы отчетов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="644ac-276">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="644ac-277">Указанные ниже ограничения применяются к любому запросу в `/reports`.</span><span class="sxs-lookup"><span data-stu-id="644ac-277">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="644ac-278">Операция</span><span class="sxs-lookup"><span data-stu-id="644ac-278">Operation</span></span>                 | <span data-ttu-id="644ac-279">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="644ac-279">Limit per app per tenant</span></span>     | <span data-ttu-id="644ac-280">Максимальное количество для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="644ac-280">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="644ac-281">Любой запрос (CSV)</span><span class="sxs-lookup"><span data-stu-id="644ac-281">Any request (CSV)</span></span>         | <span data-ttu-id="644ac-282">14 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="644ac-282">14 requests per 10 minutes</span></span>   | <span data-ttu-id="644ac-283">40 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="644ac-283">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="644ac-284">Любой запрос (JSON, бета-версия)</span><span class="sxs-lookup"><span data-stu-id="644ac-284">Any request (JSON, beta)</span></span>  | <span data-ttu-id="644ac-285">100 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="644ac-285">100 requests per 10 minutes</span></span>  | <span data-ttu-id="644ac-286">н/д</span><span class="sxs-lookup"><span data-stu-id="644ac-286">n/a</span></span>                        |

<span data-ttu-id="644ac-287">Предыдущие пределы применяются по отдельности к каждому API отчетов.</span><span class="sxs-lookup"><span data-stu-id="644ac-287">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="644ac-288">Например, запрос к API отчетов об активности пользователей Microsoft Teams и запрос на отчеты об активности пользователей в Outlook в течение 10 минут будут считаться 1 запросом из 14 для каждого API, а не 2 запросами из 14.</span><span class="sxs-lookup"><span data-stu-id="644ac-288">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="644ac-289">Пределы службы диспетчера приглашений</span><span class="sxs-lookup"><span data-stu-id="644ac-289">Invitation manager service limits</span></span>

<span data-ttu-id="644ac-290">Указанные ниже ограничения применяются к любому запросу в `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="644ac-290">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="644ac-291">Операция</span><span class="sxs-lookup"><span data-stu-id="644ac-291">Operation</span></span>                 | <span data-ttu-id="644ac-292">Максимальное количество для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="644ac-292">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="644ac-293">Любая операция</span><span class="sxs-lookup"><span data-stu-id="644ac-293">Any operation</span></span>             | <span data-ttu-id="644ac-294">150 запросов в течение 5 секунд</span><span class="sxs-lookup"><span data-stu-id="644ac-294">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a><span data-ttu-id="644ac-295">Пределы службы образования</span><span class="sxs-lookup"><span data-stu-id="644ac-295">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="644ac-296">Пределы для служб Excel</span><span class="sxs-lookup"><span data-stu-id="644ac-296">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="644ac-297">Пределы службы журналов аудита удостоверений и доступа</span><span class="sxs-lookup"><span data-stu-id="644ac-297">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="644ac-298">Пределы службы поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="644ac-298">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="644ac-299">Пределы службы Intune</span><span class="sxs-lookup"><span data-stu-id="644ac-299">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="644ac-300">Пределы для служб Skype</span><span class="sxs-lookup"><span data-stu-id="644ac-300">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="644ac-301">Пределы для службы подписки</span><span class="sxs-lookup"><span data-stu-id="644ac-301">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
