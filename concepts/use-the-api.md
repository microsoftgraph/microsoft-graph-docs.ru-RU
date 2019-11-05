---
title: Использование API Microsoft Graph
description: Microsoft Graph — это соответствующий ограничениям REST веб-API, обеспечивающий доступ к ресурсам службы Microsoft Cloud. После регистрации приложения и получения маркеров аутентификации для пользователя или службы можно отправлять запросы к API Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 0e4bba173c234201c3f3002e8917eaa74176a583
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37968550"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="d9acf-104">Использование API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d9acf-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="d9acf-p102">Microsoft Graph — это соответствующий ограничениям REST веб-API, обеспечивающий доступ к ресурсам службы Microsoft Cloud. После [регистрации приложения](auth-register-app-v2.md) и [получения маркеров аутентификации для пользователя](auth-v2-user.md) или [службы](auth-v2-service.md) можно отправлять запросы к API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d9acf-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="d9acf-107">**Важно!** Изменяется принцип применения политик условного доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d9acf-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="d9acf-108">Вам необходимо обновить свои приложения, чтобы они могли обрабатывать сценарии, в которых выполняется настройка политик условного доступа.</span><span class="sxs-lookup"><span data-stu-id="d9acf-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="d9acf-109">Дополнительные сведения и рекомендации см. в статье [Руководство для разработчиков по условному доступу в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="d9acf-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="d9acf-110">Для чтения или записи ресурса, например user или сообщения электронной почты, создайте запрос, показанный ниже.</span><span class="sxs-lookup"><span data-stu-id="d9acf-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="d9acf-111">Компоненты запроса:</span><span class="sxs-lookup"><span data-stu-id="d9acf-111">The components of a request include:</span></span>

* <span data-ttu-id="d9acf-112">[{Метод HTTP}](#http-methods) — метод HTTP, используемый в запросе для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d9acf-112">[{HTTP method}](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="d9acf-113">[{версия}](#version) — версия API Microsoft Graph, которую использует приложение.</span><span class="sxs-lookup"><span data-stu-id="d9acf-113">[{version}](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="d9acf-114">[{ресурс}](#resource) — ресурс Microsoft Graph, на который вы ссылаетесь.</span><span class="sxs-lookup"><span data-stu-id="d9acf-114">[{resource}](#resource) - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="d9acf-115">[{параметры-запроса}](#query-parameters) — необязательные параметры запроса OData или метода REST для изменения ответа.</span><span class="sxs-lookup"><span data-stu-id="d9acf-115">[{query-parameters}](#query-parameters) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="d9acf-116">После создания запроса возвращается ответ, который включает:</span><span class="sxs-lookup"><span data-stu-id="d9acf-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="d9acf-p104">Код состояния — код состояния HTTP, который указывает на результат операции. Сведения о кодах ошибок HTTP см. в разделе [Ошибки](errors.md).</span><span class="sxs-lookup"><span data-stu-id="d9acf-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="d9acf-p105">Ответ — запрошенные данные или результат операции. Для некоторых операций ответ может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="d9acf-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="d9acf-p106">`nextLink` — если найдено много данных, чтобы пролистать их все, используйте URL-адрес, возвращенный в свойстве `@odata.nextLink`. Дополнительные сведения см. в [этой статье](paging.md).</span><span class="sxs-lookup"><span data-stu-id="d9acf-p106">`nextLink` - If your request returns a lot of data, you need to page through it by using the URL returned in `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="d9acf-123">Методы HTTP</span><span class="sxs-lookup"><span data-stu-id="d9acf-123">HTTP methods</span></span>

<span data-ttu-id="d9acf-p107">Чтобы определить функцию запроса, Microsoft Graph использует метод HTTP. API поддерживает перечисленные ниже методы.</span><span class="sxs-lookup"><span data-stu-id="d9acf-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="d9acf-126">**Метод**</span><span class="sxs-lookup"><span data-stu-id="d9acf-126">**Method**</span></span> |<span data-ttu-id="d9acf-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9acf-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="d9acf-128">GET</span><span class="sxs-lookup"><span data-stu-id="d9acf-128">GET</span></span>    | <span data-ttu-id="d9acf-129">Чтение данных из ресурса.</span><span class="sxs-lookup"><span data-stu-id="d9acf-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="d9acf-130">POST</span><span class="sxs-lookup"><span data-stu-id="d9acf-130">POST</span></span>   | <span data-ttu-id="d9acf-131">Создание нового ресурса или выполнение действия.</span><span class="sxs-lookup"><span data-stu-id="d9acf-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="d9acf-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="d9acf-132">PATCH</span></span>  | <span data-ttu-id="d9acf-133">Обновление ресурса с использованием новых значений.</span><span class="sxs-lookup"><span data-stu-id="d9acf-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="d9acf-134">PUT</span><span class="sxs-lookup"><span data-stu-id="d9acf-134">PUT</span></span>    | <span data-ttu-id="d9acf-135">Замена ресурса новым.</span><span class="sxs-lookup"><span data-stu-id="d9acf-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="d9acf-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="d9acf-136">DELETE</span></span> | <span data-ttu-id="d9acf-137">Удаление ресурса.</span><span class="sxs-lookup"><span data-stu-id="d9acf-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="d9acf-138">Для CRUD-методов `GET` и `DELETE` указывать текст запроса не нужно.</span><span class="sxs-lookup"><span data-stu-id="d9acf-138">For the CRUD methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="d9acf-139">Для методов `POST`, `PATCH` и `PUT` текст запроса обычно указывается в формате JSON и содержит такие дополнительные сведения, как значения свойств ресурса.</span><span class="sxs-lookup"><span data-stu-id="d9acf-139">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="d9acf-140">Версия</span><span class="sxs-lookup"><span data-stu-id="d9acf-140">Version</span></span>

<span data-ttu-id="d9acf-141">Microsoft Graph в настоящее время поддерживает две версии: `v1.0` и `beta`.</span><span class="sxs-lookup"><span data-stu-id="d9acf-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="d9acf-p108">`v1.0` включает общедоступные API. Используйте версию 1.0 для всех рабочих приложений.</span><span class="sxs-lookup"><span data-stu-id="d9acf-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="d9acf-p109">`beta` содержит бета-версии API. Так как мы можем вносить в бета-версии API критические изменения, рекомендуем использовать их только для проверки разрабатываемых приложений. Не используйте бета-версии API в рабочих приложениях.</span><span class="sxs-lookup"><span data-stu-id="d9acf-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="d9acf-p110">Мы всегда рады отзывам о бета-версиях API. Чтобы оставить отзыв или предложить функцию, посетите нашу страницу [UserVoice](https://officespdev.uservoice.com/).</span><span class="sxs-lookup"><span data-stu-id="d9acf-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="d9acf-148">Дополнительные сведения о версиях API см. в статье [Управление версиями и поддержка](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="d9acf-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="d9acf-149">Ресурс</span><span class="sxs-lookup"><span data-stu-id="d9acf-149">Resource</span></span>

<span data-ttu-id="d9acf-150">Ресурс может быть объектом или сложным типом и обычно определяется с помощью свойств.</span><span class="sxs-lookup"><span data-stu-id="d9acf-150">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="d9acf-151">Объекты всегда содержат свойство **id**, что отличает их от сложных типов.</span><span class="sxs-lookup"><span data-stu-id="d9acf-151">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="d9acf-152">URL-адрес будет включать ресурс, с которым вы взаимодействуете в запросе, например `me`, **user**, **group**, **drive** и **site**.</span><span class="sxs-lookup"><span data-stu-id="d9acf-152">Your URL will include the resource you are interacting with in the request, such as `me`, **user**, **group**, **drive**, and **site**.</span></span> <span data-ttu-id="d9acf-153">Часто ресурсы верхнего уровня также включают _связи_, которые вы можете использовать для доступа к дополнительным ресурсам, например к ресурсам `me/messages` или `me/drive`.</span><span class="sxs-lookup"><span data-stu-id="d9acf-153">Often, top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="d9acf-154">Вы также можете взаимодействовать с ресурсами при помощи _методов_. Например, чтобы отправить электронное письмо, воспользуйтесь методом `me/sendMail`.</span><span class="sxs-lookup"><span data-stu-id="d9acf-154">You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`.</span></span> <span data-ttu-id="d9acf-155">Дополнительные сведения см. в статье [Доступ к данным и методам с помощью Microsoft Graph](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="d9acf-155">For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="d9acf-p113">Для доступа к каждому ресурсу могут потребоваться особые разрешения. Для создания и обновления ресурса часто требуется более высокий уровень разрешений, чем для чтения. Сведения о требуемых разрешениях см. в справочной статье о методе.</span><span class="sxs-lookup"><span data-stu-id="d9acf-p113">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="d9acf-159">Сведения о разрешениях см. в [справочнике по разрешениям](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9acf-159">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="d9acf-160">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d9acf-160">Query parameters</span></span>

<span data-ttu-id="d9acf-161">В качестве параметров запросов могут использоваться системные параметры запроса OData или другие строки, поддерживаемые методом для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d9acf-161">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="d9acf-162">Вы можете использовать необязательные системные параметры запроса OData, чтобы изменять свойства, включаемые в ответ, находить элементы, соответствующие пользовательскому запросу, и указывать дополнительные параметры для метода.</span><span class="sxs-lookup"><span data-stu-id="d9acf-162">You can use optional OData system query options to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="d9acf-163">Например, если добавить указанный ниже параметр `filter`, будут возвращаться только сообщения, у которых свойство `emailAddress` имеет значение `jon@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="d9acf-163">For example, adding the following `filter` parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="d9acf-164">Дополнительные сведения о параметрах запроса OData см. в статье [Настройка ответов с помощью параметров запроса](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="d9acf-164">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="d9acf-165">Помимо параметров запроса OData, некоторые методы требуют указание значений параметров в составе URL-адреса запроса.</span><span class="sxs-lookup"><span data-stu-id="d9acf-165">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="d9acf-166">Например, вы можете получить коллекцию событий, произошедших в течение периода времени в календаре пользователя, запросив связь **calendarView** объекта **user** и указав в качестве параметров запроса значения периода `startDateTime` и `endDateTime`.</span><span class="sxs-lookup"><span data-stu-id="d9acf-166">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="next-steps"></a><span data-ttu-id="d9acf-167">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d9acf-167">Next steps</span></span>

<span data-ttu-id="d9acf-p115">Все готово для настройки Microsoft Graph. Чтобы узнать больше, перейдите в [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer) и опробуйте запросы, воспользуйтесь [кратким руководством](https://developer.microsoft.com/graph/quick-start) или начните с одного из [пакетов SDK или примеров кода](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="d9acf-p115">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
