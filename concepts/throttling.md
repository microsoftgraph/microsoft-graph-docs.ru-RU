---
title: Руководство по регулированию Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7678b364855381eaf5a138b42d6172a6cbd233f4
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989935"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="b25ec-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b25ec-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="b25ec-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="b25ec-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="b25ec-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="b25ec-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="b25ec-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="b25ec-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="b25ec-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="b25ec-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="b25ec-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="b25ec-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="b25ec-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="b25ec-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="b25ec-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="b25ec-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="b25ec-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="b25ec-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="b25ec-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="b25ec-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="b25ec-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="b25ec-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="b25ec-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="b25ec-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="b25ec-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="b25ec-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="b25ec-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="b25ec-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="b25ec-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="b25ec-119">Common throttling scenarios</span></span>

<span data-ttu-id="b25ec-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="b25ec-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="b25ec-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="b25ec-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="b25ec-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="b25ec-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="b25ec-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="b25ec-123">Best practices to handle throttling</span></span>

<span data-ttu-id="b25ec-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="b25ec-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="b25ec-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="b25ec-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="b25ec-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="b25ec-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="b25ec-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="b25ec-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="b25ec-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="b25ec-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="b25ec-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="b25ec-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="b25ec-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="b25ec-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="b25ec-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="b25ec-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="b25ec-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="b25ec-132">Retry the request.</span></span>
3. <span data-ttu-id="b25ec-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="b25ec-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="b25ec-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="b25ec-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="b25ec-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="b25ec-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="b25ec-136">User</span><span class="sxs-lookup"><span data-stu-id="b25ec-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="b25ec-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="b25ec-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="b25ec-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="b25ec-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="b25ec-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="b25ec-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="b25ec-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="b25ec-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="b25ec-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="b25ec-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="b25ec-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="b25ec-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="b25ec-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="b25ec-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="b25ec-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="b25ec-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="b25ec-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b25ec-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="b25ec-146">Subscription</span><span class="sxs-lookup"><span data-stu-id="b25ec-146">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="b25ec-147">Отправлен</span><span class="sxs-lookup"><span data-stu-id="b25ec-147">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="b25ec-148">Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="b25ec-148">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="b25ec-149">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="b25ec-149">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="b25ec-150">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="b25ec-150">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="b25ec-151">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="b25ec-151">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="b25ec-152">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="b25ec-152">Best practices to avoid throttling</span></span>

<span data-ttu-id="b25ec-153">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="b25ec-153">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="b25ec-154">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="b25ec-154">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="b25ec-155">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="b25ec-155">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="b25ec-156">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="b25ec-156">Service-specific limits</span></span>

<span data-ttu-id="b25ec-157">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b25ec-157">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="b25ec-158">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="b25ec-158">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="b25ec-159">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="b25ec-159">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="b25ec-160">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="b25ec-160">Outlook service limits</span></span>

<span data-ttu-id="b25ec-161">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b25ec-161">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="b25ec-162">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="b25ec-162">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="b25ec-163">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b25ec-163">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="b25ec-164">Следующие пределы применяются к общедоступному облаку, а также к [облачным облачным развертываниям](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="b25ec-164">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="b25ec-165">Ограничение</span><span class="sxs-lookup"><span data-stu-id="b25ec-165">Limit</span></span>                                                      | <span data-ttu-id="b25ec-166">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="b25ec-166">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="b25ec-167">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="b25ec-167">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="b25ec-168">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="b25ec-168">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="b25ec-169">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="b25ec-169">4 concurrent requests</span></span>                                      | <span data-ttu-id="b25ec-170">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="b25ec-170">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="b25ec-171">Отправка 15 Мбит (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="b25ec-171">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="b25ec-172">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="b25ec-172">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="b25ec-173">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="b25ec-173">Outlook service resources</span></span>

<span data-ttu-id="b25ec-174">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="b25ec-174">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="b25ec-175">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="b25ec-175">Calendar API resources</span></span>

- [<span data-ttu-id="b25ec-176">event</span><span class="sxs-lookup"><span data-stu-id="b25ec-176">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="b25ec-177">eventMessage</span><span class="sxs-lookup"><span data-stu-id="b25ec-177">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="b25ec-178">calendar</span><span class="sxs-lookup"><span data-stu-id="b25ec-178">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="b25ec-179">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="b25ec-179">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="b25ec-180">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="b25ec-180">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="b25ec-181">attachment</span><span class="sxs-lookup"><span data-stu-id="b25ec-181">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="b25ec-182">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="b25ec-182">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="b25ec-183">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="b25ec-183">Mail API resources</span></span>

- [<span data-ttu-id="b25ec-184">message</span><span class="sxs-lookup"><span data-stu-id="b25ec-184">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="b25ec-185">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b25ec-185">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="b25ec-186">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="b25ec-186">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="b25ec-187">messageRule</span><span class="sxs-lookup"><span data-stu-id="b25ec-187">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="b25ec-188">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="b25ec-188">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="b25ec-189">attachment</span><span class="sxs-lookup"><span data-stu-id="b25ec-189">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="b25ec-190">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="b25ec-190">Personal contacts API resources</span></span>

- [<span data-ttu-id="b25ec-191">contact</span><span class="sxs-lookup"><span data-stu-id="b25ec-191">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="b25ec-192">contactFolder</span><span class="sxs-lookup"><span data-stu-id="b25ec-192">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="b25ec-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="b25ec-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="b25ec-194">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="b25ec-194">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="b25ec-195">person</span><span class="sxs-lookup"><span data-stu-id="b25ec-195">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="b25ec-196">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="b25ec-196">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="b25ec-197">outlookTask</span><span class="sxs-lookup"><span data-stu-id="b25ec-197">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="b25ec-198">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b25ec-198">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="b25ec-199">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="b25ec-199">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="b25ec-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="b25ec-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="b25ec-201">attachment</span><span class="sxs-lookup"><span data-stu-id="b25ec-201">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="b25ec-202">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b25ec-202">Microsoft Teams service limits</span></span>

<span data-ttu-id="b25ec-203">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="b25ec-203">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="b25ec-204">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="b25ec-204">Teams request type</span></span>                                   | <span data-ttu-id="b25ec-205">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="b25ec-205">Limit per app per tenant</span></span>        | <span data-ttu-id="b25ec-206">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="b25ec-206">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="b25ec-207">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b25ec-207">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="b25ec-208">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="b25ec-208">15000 requests every 10 seconds</span></span> | <span data-ttu-id="b25ec-209">н/д</span><span class="sxs-lookup"><span data-stu-id="b25ec-209">n/a</span></span> |
| <span data-ttu-id="b25ec-210">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="b25ec-210">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="b25ec-211">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-211">60 rps</span></span>                          | <span data-ttu-id="b25ec-212">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-212">600 rps</span></span> |
| <span data-ttu-id="b25ec-213">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="b25ec-213">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="b25ec-214">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-214">30 rps</span></span>                         | <span data-ttu-id="b25ec-215">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-215">300 rps</span></span>  |
| <span data-ttu-id="b25ec-216">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="b25ec-216">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="b25ec-217">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-217">30 rps</span></span>                         | <span data-ttu-id="b25ec-218">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-218">300 rps</span></span>  |
| <span data-ttu-id="b25ec-219">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="b25ec-219">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="b25ec-220">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-220">15 rps</span></span>                         | <span data-ttu-id="b25ec-221">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-221">150 rps</span></span>  |
| <span data-ttu-id="b25ec-222">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="b25ec-222">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="b25ec-223">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-223">30 rps</span></span>                         | <span data-ttu-id="b25ec-224">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-224">300 rps</span></span>  |
| <span data-ttu-id="b25ec-225">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="b25ec-225">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="b25ec-226">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-226">6 rps</span></span> | <span data-ttu-id="b25ec-227">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-227">150 rps</span></span>  | 
| <span data-ttu-id="b25ec-228">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="b25ec-228">GET channel message</span></span>  | <span data-ttu-id="b25ec-229">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-229">5 rps</span></span> | <span data-ttu-id="b25ec-230">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-230">100 rps</span></span> |
| <span data-ttu-id="b25ec-231">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="b25ec-231">GET 1:1/group chat message</span></span>  | <span data-ttu-id="b25ec-232">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-232">3 rps</span></span> | <span data-ttu-id="b25ec-233">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-233">30 rps</span></span> |
| <span data-ttu-id="b25ec-234">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="b25ec-234">POST channel message</span></span> | <span data-ttu-id="b25ec-235">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-235">2 rps</span></span> | <span data-ttu-id="b25ec-236">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-236">20 rps</span></span> |
| <span data-ttu-id="b25ec-237">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="b25ec-237">POST 1:1/group chat message</span></span> | <span data-ttu-id="b25ec-238">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-238">2 rps</span></span> | <span data-ttu-id="b25ec-239">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="b25ec-239">20 rps</span></span> |

<span data-ttu-id="b25ec-240">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="b25ec-240">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="b25ec-241">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="b25ec-241">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="b25ec-242">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="b25ec-242">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="b25ec-243">Пределы службы диспетчера приглашений</span><span class="sxs-lookup"><span data-stu-id="b25ec-243">Invitation manager service limits</span></span>

<span data-ttu-id="b25ec-244">Указанные ниже ограничения применяются к любому запросу в `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="b25ec-244">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="b25ec-245">Операция</span><span class="sxs-lookup"><span data-stu-id="b25ec-245">Operation</span></span>                 | <span data-ttu-id="b25ec-246">Максимальное количество для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="b25ec-246">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="b25ec-247">Любая операция</span><span class="sxs-lookup"><span data-stu-id="b25ec-247">Any operation</span></span>             | <span data-ttu-id="b25ec-248">150 запросов в течение 5 секунд</span><span class="sxs-lookup"><span data-stu-id="b25ec-248">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a><span data-ttu-id="b25ec-249">Пределы службы образования</span><span class="sxs-lookup"><span data-stu-id="b25ec-249">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="b25ec-250">Пределы для служб Excel</span><span class="sxs-lookup"><span data-stu-id="b25ec-250">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="b25ec-251">Пределы службы журналов аудита удостоверений и доступа</span><span class="sxs-lookup"><span data-stu-id="b25ec-251">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="b25ec-252">Пределы службы поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="b25ec-252">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="b25ec-253">Пределы службы Intune</span><span class="sxs-lookup"><span data-stu-id="b25ec-253">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="b25ec-254">Пределы для служб Skype</span><span class="sxs-lookup"><span data-stu-id="b25ec-254">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="b25ec-255">Пределы для службы подписки</span><span class="sxs-lookup"><span data-stu-id="b25ec-255">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
