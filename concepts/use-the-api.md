---
title: Использование API Microsoft Graph
description: Microsoft Graph — это соответствующий ограничениям REST веб-API, обеспечивающий доступ к ресурсам службы Microsoft Cloud. После регистрации приложения и получения маркеров аутентификации для пользователя или службы можно отправлять запросы к API Microsoft Graph.
ms.openlocfilehash: 1a9d9bcefdfb302a9de602aa15aa642a0c57a793
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092702"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="3d4b4-104">Использование API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3d4b4-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="3d4b4-p102">Microsoft Graph — это соответствующий ограничениям REST веб-API, обеспечивающий доступ к ресурсам службы Microsoft Cloud. После [регистрации приложения](auth-register-app-v2.md) и [получения маркеров аутентификации для пользователя](auth-v2-user.md) или [службы](auth-v2-service.md) можно отправлять запросы к API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="3d4b4-107">**Важно!** Изменяется принцип применения политик условного доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="3d4b4-108">Вам необходимо обновить свои приложения, чтобы они могли обрабатывать сценарии, в которых выполняется настройка политик условного доступа.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="3d4b4-109">Дополнительные сведения и рекомендации см. в статье [Руководство для разработчиков по условному доступу в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="3d4b4-110">Для чтения или записи ресурса, например user или сообщения электронной почты, создайте запрос, показанный ниже.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

<span data-ttu-id="3d4b4-111">Компоненты запроса:</span><span class="sxs-lookup"><span data-stu-id="3d4b4-111">The components of a request include:</span></span>

* <span data-ttu-id="3d4b4-112">[Метод HTTP](#http-methods) — метод HTTP, используемый в запросе для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="3d4b4-113">[`{version}`](#version) — версия API Microsoft Graph, которую использует приложение.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-113">[`{version}`](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="3d4b4-114">[`{resource}`](#resource) — ресурс Microsoft Graph, на который вы ссылаетесь.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-114">[`{resource}`](#resource) - The resource in Microsoft Graph that you're referencing.</span></span>
* <span data-ttu-id="3d4b4-115">[query-parameters](#query-parameters-optional) — необязательный набор параметров для изменения запроса или ответа.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-115">[query-parameters](#query-parameters-optional) - An optional set of parameters to modify the request or response.</span></span>

<span data-ttu-id="3d4b4-116">После создания запроса возвращается ответ, который включает:</span><span class="sxs-lookup"><span data-stu-id="3d4b4-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="3d4b4-p104">Код состояния — код состояния HTTP, который указывает на результат операции. Сведения о кодах ошибок HTTP см. в разделе [Ошибки](errors.md).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="3d4b4-p105">Ответ — запрошенные данные или результат операции. Для некоторых операций ответ может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="3d4b4-p106">Ссылка **Далее** — если найдено много данных, чтобы пролистать их все, щелкайте **Далее**. Дополнительные сведения см. в [этой статье](paging.md).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p106">**Next** link - If your request returns a lot of data, you need to page through it by choosing **Next**. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="3d4b4-123">Методы HTTP</span><span class="sxs-lookup"><span data-stu-id="3d4b4-123">HTTP methods</span></span>

<span data-ttu-id="3d4b4-p107">Чтобы определить функцию запроса, Microsoft Graph использует метод HTTP. API поддерживает перечисленные ниже методы.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="3d4b4-126">**Метод**</span><span class="sxs-lookup"><span data-stu-id="3d4b4-126">**Method**</span></span> |<span data-ttu-id="3d4b4-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d4b4-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="3d4b4-128">GET</span><span class="sxs-lookup"><span data-stu-id="3d4b4-128">GET</span></span>    | <span data-ttu-id="3d4b4-129">Чтение данных из ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="3d4b4-130">POST</span><span class="sxs-lookup"><span data-stu-id="3d4b4-130">POST</span></span>   | <span data-ttu-id="3d4b4-131">Создание нового ресурса или выполнение действия.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="3d4b4-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="3d4b4-132">PATCH</span></span>  | <span data-ttu-id="3d4b4-133">Обновление ресурса с использованием новых значений.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="3d4b4-134">PUT</span><span class="sxs-lookup"><span data-stu-id="3d4b4-134">PUT</span></span>    | <span data-ttu-id="3d4b4-135">Замена ресурса новым.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="3d4b4-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="3d4b4-136">DELETE</span></span> | <span data-ttu-id="3d4b4-137">Удаление ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="3d4b4-138">Для методов **GET** и **DELETE** указывать текст запроса не нужно.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-138">For the methods **GET** and **DELETE**, no request body is required.</span></span>
* <span data-ttu-id="3d4b4-139">Для методов **POST**, **PATCH** и **PUT** текст запроса обычно указывается в формате JSON и содержит такие дополнительные сведения, как значения свойств ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-139">The **POST**, **PATCH**, and **PUT** methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="3d4b4-140">Версия</span><span class="sxs-lookup"><span data-stu-id="3d4b4-140">Version</span></span>

<span data-ttu-id="3d4b4-141">Microsoft Graph в настоящее время поддерживает две версии: `v1.0` и `beta`.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="3d4b4-p108">`v1.0` включает общедоступные API. Используйте версию 1.0 для всех рабочих приложений.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="3d4b4-p109">`beta` содержит бета-версии API. Так как мы можем вносить в бета-версии API критические изменения, рекомендуем использовать их только для проверки разрабатываемых приложений. Не используйте бета-версии API в рабочих приложениях.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="3d4b4-p110">Мы всегда рады отзывам о бета-версиях API. Чтобы оставить отзыв или предложить функцию, посетите нашу страницу [UserVoice](https://officespdev.uservoice.com/).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="3d4b4-148">Дополнительные сведения о версиях API см. в статье [Управление версиями и поддержка](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="3d4b4-149">Resource</span><span class="sxs-lookup"><span data-stu-id="3d4b4-149">Resource</span></span>

<span data-ttu-id="3d4b4-p111">URL-адрес будет включать ресурсы, с которыми вы взаимодействуете в запросе, например `me`, `users`, `groups`, `drives` и `sites`. Каждый из ресурсов верхнего уровня также включает **отношения**, которые можно использовать для доступа к дополнительным ресурсам, например `me/messages` или `me/drive`. Работать с ресурсами можно также с помощью **методов**. Например, для отправки сообщения электронной почты используйте `me/sendMail`.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p111">Your URL will include the resource or resources you are interacting with in the request, such as `me`, `users`, `groups`, `drives`, and `sites`. Each of the top-level resources also include **relationships**, which you can use to access additional resources, like `me/messages` or `me/drive`. You can also interact with resources using **methods**; for example, to send an email, use `me/sendMail`.</span></span>

<span data-ttu-id="3d4b4-153">Дополнительные сведения о том, как переходить по связям и методам ресурсов, см. в статье [Обход Microsoft Graph](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-153">For more information about how to navigate resource relationships and methods, see [Traverse the graph](traverse-the-graph.md).</span></span> 

<span data-ttu-id="3d4b4-p112">Для доступа к каждому ресурсу могут потребоваться особые разрешения. Для создания и обновления ресурса часто требуется более высокий уровень разрешений, чем для чтения. Сведения о требуемых разрешениях см. в справочной статье о методе.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p112">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="3d4b4-157">Сведения о разрешениях см. в [справочнике по разрешениям](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-157">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters-optional"></a><span data-ttu-id="3d4b4-158">Параметры запросов (необязательные)</span><span class="sxs-lookup"><span data-stu-id="3d4b4-158">Query parameters (optional)</span></span>

<span data-ttu-id="3d4b4-p113">Для настройки ответа в приложении Microsoft Graph можно использовать дополнительные параметры запроса. Используйте параметры запроса, чтобы изменять свойства, включаемые в ответ, находить элементы, соответствующие пользовательскому запросу, и указывать дополнительные параметры для метода.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p113">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="3d4b4-161">Например, если добавить указанный ниже параметр фильтрации, будут возвращаться только сообщения, у которых свойство `emailAddress` имеет значение `jon@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="3d4b4-161">For example, adding the following filter parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="3d4b4-162">Дополнительные сведения о параметрах запроса, см. в статье [Настройка ответов](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-162">For more information about query parameters, see [Customize responses](query-parameters.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="3d4b4-163">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3d4b4-163">Next steps</span></span>

<span data-ttu-id="3d4b4-p114">Все готово для настройки Microsoft Graph. Чтобы узнать больше, перейдите в [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer) и опробуйте запросы, воспользуйтесь [кратким руководством](https://developer.microsoft.com/graph/quick-start) или начните с одного из [пакетов SDK или примеров кода](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="3d4b4-p114">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
