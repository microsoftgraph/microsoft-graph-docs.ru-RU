---
title: Использование API Microsoft Graph
description: Microsoft Graph — это соответствующий ограничениям REST веб-API, обеспечивающий доступ к ресурсам службы Microsoft Cloud. После регистрации приложения и получения маркеров аутентификации для пользователя или службы можно отправлять запросы к API Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e5a70d69d872d57963f658e7ff2d9e5fa088d3e9
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679542"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="71150-104">Использование API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="71150-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="71150-p102">Microsoft Graph — это соответствующий ограничениям REST веб-API, обеспечивающий доступ к ресурсам службы Microsoft Cloud. После [регистрации приложения](auth-register-app-v2.md) и [получения маркеров аутентификации для пользователя](auth-v2-user.md) или [службы](auth-v2-service.md) можно отправлять запросы к API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="71150-107">**Важно!** Изменяется принцип применения политик условного доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="71150-108">Вам необходимо обновить свои приложения, чтобы они могли обрабатывать сценарии, в которых выполняется настройка политик условного доступа.</span><span class="sxs-lookup"><span data-stu-id="71150-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="71150-109">Дополнительные сведения и рекомендации см. в статье [Руководство для разработчиков по условному доступу в Azure Active Directory](/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="71150-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

## <a name="odata-namespace"></a><span data-ttu-id="71150-110">Пространство имен OData</span><span class="sxs-lookup"><span data-stu-id="71150-110">OData namespace</span></span>

<span data-ttu-id="71150-111">API Microsoft Graph определяет большую часть своих ресурсов, методов и перечислений в пространстве имен OData, `microsoft.graph`, в [метаданных Microsoft Graph](traverse-the-graph.md#microsoft-graph-api-metadata).</span><span class="sxs-lookup"><span data-stu-id="71150-111">The Microsoft Graph API defines most of its resources, methods, and enumerations in the OData namespace, `microsoft.graph`, in the [Microsoft Graph metadata](traverse-the-graph.md#microsoft-graph-api-metadata).</span></span> <span data-ttu-id="71150-112">Небольшое число наборов API определено во вложенных пространствах имен, например [API записей звонков](/graph/api/resources/callrecords-api-overview), определяющий такие ресурсы, как [callRecord](/graph/api/resources/callrecords-callrecord) в `microsoft.graph.callRecords`.</span><span class="sxs-lookup"><span data-stu-id="71150-112">A small number of API sets are defined in their sub-namespaces, such as the [call records API](/graph/api/resources/callrecords-api-overview) which defines resources like [callRecord](/graph/api/resources/callrecords-callrecord) in `microsoft.graph.callRecords`.</span></span> 

<span data-ttu-id="71150-113">Если явно не указано в соответствующем разделе, предполагается, что типы, методы и перечисления являются частью пространства имен `microsoft.graph`.</span><span class="sxs-lookup"><span data-stu-id="71150-113">Unless explicitly specified in the corresponding topic, assume types, methods, and enumerations are part of the `microsoft.graph` namespace.</span></span>

## <a name="call-a-rest-api-method"></a><span data-ttu-id="71150-114">Вызов метода API REST</span><span class="sxs-lookup"><span data-stu-id="71150-114">Call a REST API method</span></span>

<span data-ttu-id="71150-115">Для чтения или записи ресурса, например пользователя или сообщения электронной почты, создайте запрос, показанный ниже:</span><span class="sxs-lookup"><span data-stu-id="71150-115">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="71150-116">Компоненты запроса:</span><span class="sxs-lookup"><span data-stu-id="71150-116">The components of a request include:</span></span>

* <span data-ttu-id="71150-117">[{Метод HTTP}](#http-methods) — метод HTTP, используемый в запросе для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-117">[{HTTP method}](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="71150-118">[{версия}](#version) — версия API Microsoft Graph, которую использует приложение.</span><span class="sxs-lookup"><span data-stu-id="71150-118">[{version}](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="71150-119">[{ресурс}](#resource) — ресурс Microsoft Graph, на который вы ссылаетесь.</span><span class="sxs-lookup"><span data-stu-id="71150-119">[{resource}](#resource) - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="71150-120">[{параметры-запроса}](#query-parameters) — необязательные параметры запроса OData или метода REST для изменения ответа.</span><span class="sxs-lookup"><span data-stu-id="71150-120">[{query-parameters}](#query-parameters) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="71150-121">После создания запроса возвращается ответ, который включает:</span><span class="sxs-lookup"><span data-stu-id="71150-121">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="71150-p105">Код состояния — код состояния HTTP, который указывает на результат операции. Сведения о кодах ошибок HTTP см. в разделе [Ошибки](errors.md).</span><span class="sxs-lookup"><span data-stu-id="71150-p105">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="71150-p106">Ответ — запрошенные данные или результат операции. Для некоторых операций ответ может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="71150-p106">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="71150-p107">`nextLink` — если найдено много данных, чтобы пролистать их все, используйте URL-адрес, возвращенный в свойстве `@odata.nextLink`. Дополнительные сведения см. в [этой статье](paging.md).</span><span class="sxs-lookup"><span data-stu-id="71150-p107">`nextLink` - If your request returns a lot of data, you need to page through it by using the URL returned in `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="71150-128">Методы HTTP</span><span class="sxs-lookup"><span data-stu-id="71150-128">HTTP methods</span></span>

<span data-ttu-id="71150-p108">Чтобы определить функцию запроса, Microsoft Graph использует метод HTTP. API поддерживает перечисленные ниже методы.</span><span class="sxs-lookup"><span data-stu-id="71150-p108">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>

|<span data-ttu-id="71150-131">**Метод**</span><span class="sxs-lookup"><span data-stu-id="71150-131">**Method**</span></span> |<span data-ttu-id="71150-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71150-132">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="71150-133">GET</span><span class="sxs-lookup"><span data-stu-id="71150-133">GET</span></span>    | <span data-ttu-id="71150-134">Чтение данных из ресурса.</span><span class="sxs-lookup"><span data-stu-id="71150-134">Read data from a resource.</span></span>                   |
| <span data-ttu-id="71150-135">POST</span><span class="sxs-lookup"><span data-stu-id="71150-135">POST</span></span>   | <span data-ttu-id="71150-136">Создание нового ресурса или выполнение действия.</span><span class="sxs-lookup"><span data-stu-id="71150-136">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="71150-137">PATCH</span><span class="sxs-lookup"><span data-stu-id="71150-137">PATCH</span></span>  | <span data-ttu-id="71150-138">Обновление ресурса с использованием новых значений.</span><span class="sxs-lookup"><span data-stu-id="71150-138">Update a resource with new values.</span></span>           |
| <span data-ttu-id="71150-139">PUT</span><span class="sxs-lookup"><span data-stu-id="71150-139">PUT</span></span>    | <span data-ttu-id="71150-140">Замена ресурса новым.</span><span class="sxs-lookup"><span data-stu-id="71150-140">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="71150-141">DELETE</span><span class="sxs-lookup"><span data-stu-id="71150-141">DELETE</span></span> | <span data-ttu-id="71150-142">Удаление ресурса.</span><span class="sxs-lookup"><span data-stu-id="71150-142">Remove a resource.</span></span>                           |

* <span data-ttu-id="71150-143">Для CRUD-методов `GET` и `DELETE` указывать текст запроса не нужно.</span><span class="sxs-lookup"><span data-stu-id="71150-143">For the CRUD methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="71150-144">Для методов `POST`, `PATCH` и `PUT` текст запроса обычно указывается в формате JSON и содержит такие дополнительные сведения, как значения свойств ресурса.</span><span class="sxs-lookup"><span data-stu-id="71150-144">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="71150-145">Версия</span><span class="sxs-lookup"><span data-stu-id="71150-145">Version</span></span>

<span data-ttu-id="71150-146">Microsoft Graph в настоящее время поддерживает две версии: `v1.0` и `beta`.</span><span class="sxs-lookup"><span data-stu-id="71150-146">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="71150-p109">`v1.0` включает общедоступные API. Используйте версию 1.0 для всех рабочих приложений.</span><span class="sxs-lookup"><span data-stu-id="71150-p109">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="71150-p110">`beta` содержит бета-версии API. Так как мы можем вносить в бета-версии API критические изменения, рекомендуем использовать их только для проверки разрабатываемых приложений. Не используйте бета-версии API в рабочих приложениях.</span><span class="sxs-lookup"><span data-stu-id="71150-p110">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="71150-151">Мы всегда рады отзывам о бета-версиях API.</span><span class="sxs-lookup"><span data-stu-id="71150-151">We are always looking for feedback on our beta APIs.</span></span> <span data-ttu-id="71150-152">Чтобы оставить отзыв или запросить какие-либо функции, посетите наш [форум с идеями для платформы разработчиков Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span><span class="sxs-lookup"><span data-stu-id="71150-152">To provide feedback or request features, see our [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span>

<span data-ttu-id="71150-153">Дополнительные сведения о версиях API см. в статье [Управление версиями и поддержка](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="71150-153">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="71150-154">Ресурс</span><span class="sxs-lookup"><span data-stu-id="71150-154">Resource</span></span>

<span data-ttu-id="71150-155">Ресурс может быть объектом или сложным типом и обычно определяется с помощью свойств.</span><span class="sxs-lookup"><span data-stu-id="71150-155">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="71150-156">Объекты всегда содержат свойство **id**, что отличает их от сложных типов.</span><span class="sxs-lookup"><span data-stu-id="71150-156">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="71150-157">URL-адрес будет включать ресурс, с которым вы взаимодействуете в запросе, например `me`, **user**, **group**, **drive** и **site**.</span><span class="sxs-lookup"><span data-stu-id="71150-157">Your URL will include the resource you are interacting with in the request, such as `me`, **user**, **group**, **drive**, and **site**.</span></span> <span data-ttu-id="71150-158">Часто ресурсы верхнего уровня также включают _связи_, которые вы можете использовать для доступа к дополнительным ресурсам, например к ресурсам `me/messages` или `me/drive`.</span><span class="sxs-lookup"><span data-stu-id="71150-158">Often, top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="71150-159">Вы также можете взаимодействовать с ресурсами при помощи _методов_. Например, чтобы отправить электронное письмо, воспользуйтесь методом `me/sendMail`.</span><span class="sxs-lookup"><span data-stu-id="71150-159">You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`.</span></span> <span data-ttu-id="71150-160">Дополнительные сведения см. в статье [Доступ к данным и методам с помощью Microsoft Graph](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="71150-160">For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="71150-p114">Для доступа к каждому ресурсу могут потребоваться особые разрешения. Для создания и обновления ресурса часто требуется более высокий уровень разрешений, чем для чтения. Сведения о требуемых разрешениях см. в справочной статье о методе.</span><span class="sxs-lookup"><span data-stu-id="71150-p114">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="71150-164">Сведения о разрешениях см. в [справочнике по разрешениям](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71150-164">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="71150-165">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="71150-165">Query parameters</span></span>

<span data-ttu-id="71150-166">В качестве параметров запросов могут использоваться системные параметры запроса OData или другие строки, поддерживаемые методом для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71150-166">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="71150-167">Вы можете использовать необязательные системные параметры запроса OData, чтобы изменять свойства, включаемые в ответ, находить элементы, соответствующие пользовательскому запросу, и указывать дополнительные параметры для метода.</span><span class="sxs-lookup"><span data-stu-id="71150-167">You can use optional OData system query options to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="71150-168">Например, если добавить указанный ниже параметр `filter`, будут возвращаться только сообщения, у которых свойство `emailAddress` имеет значение `jon@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="71150-168">For example, adding the following `filter` parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="71150-169">Дополнительные сведения о параметрах запроса OData см. в статье [Настройка ответов с помощью параметров запроса](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="71150-169">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="71150-170">Помимо параметров запроса OData, некоторые методы требуют указание значений параметров в составе URL-адреса запроса.</span><span class="sxs-lookup"><span data-stu-id="71150-170">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="71150-171">Например, вы можете получить коллекцию событий, произошедших в течение периода времени в календаре пользователя, запросив связь **calendarView** объекта **user** и указав в качестве параметров запроса значения периода `startDateTime` и `endDateTime`.</span><span class="sxs-lookup"><span data-stu-id="71150-171">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="tools-for-interacting-with-microsoft-graph"></a><span data-ttu-id="71150-172">Инструменты для взаимодействия с Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="71150-172">Tools for interacting with Microsoft Graph</span></span>

### <a name="graph-explorer"></a><span data-ttu-id="71150-173">Песочница Graph</span><span class="sxs-lookup"><span data-stu-id="71150-173">Graph Explorer</span></span>

<span data-ttu-id="71150-174">Песочница Graph — это веб-инструмент, который можно использовать для создания и тестирования запросов с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-174">Graph Explorer is a web-based tool that you can use to build and test requests using Microsoft Graph APIs.</span></span> <span data-ttu-id="71150-175">Песочница Graph доступна по адресу: `https://developer.microsoft.com/graph/graph-explorer`.</span><span class="sxs-lookup"><span data-stu-id="71150-175">You can access Graph Explorer at: `https://developer.microsoft.com/graph/graph-explorer`.</span></span>

<span data-ttu-id="71150-p117">Вы можете получить доступ к демонстрационным данным без входа или войти в свой клиент. Чтобы отправить запрос, выполните следующее:</span><span class="sxs-lookup"><span data-stu-id="71150-p117">You can either access demo data without signing in, or you can sign in to a tenant of your own. Use the following steps to build the request:</span></span>

1. <span data-ttu-id="71150-178">Выберите метод HTTP.</span><span class="sxs-lookup"><span data-stu-id="71150-178">Select the HTTP method.</span></span>
2. <span data-ttu-id="71150-179">Выберите версию API, которую нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="71150-179">Select the version of API that you want to use.</span></span>
3. <span data-ttu-id="71150-180">Введите запрос в текстовое поле запроса.</span><span class="sxs-lookup"><span data-stu-id="71150-180">Type the query in the request text box.</span></span>
4. <span data-ttu-id="71150-181">Нажмите **Запуск запроса**.</span><span class="sxs-lookup"><span data-stu-id="71150-181">Select **Run Query**.</span></span> 

<span data-ttu-id="71150-182">В следующем примере показан запрос, возвращающий сведения о пользователях в демонстрационном клиенте:</span><span class="sxs-lookup"><span data-stu-id="71150-182">The following example shows a request that returns information about users in the demo tenant:</span></span>

![Снимок экрана: песочница Graph с выделенным запросом пользователя GET](./images/graph-explorer.png)

<span data-ttu-id="71150-184">Примеры запросов представлены в песочнице Graph, чтобы вы могли быстрее запускать распространенные запросы.</span><span class="sxs-lookup"><span data-stu-id="71150-184">Sample queries are provided in Graph Explorer to enable you to more quickly run common requests.</span></span> <span data-ttu-id="71150-185">Чтобы просмотреть доступные примеры, выберите **Показать другие примеры**.</span><span class="sxs-lookup"><span data-stu-id="71150-185">To see the samples that are available, select **show more samples**.</span></span> <span data-ttu-id="71150-186">Выберите **Вкл** для набора примеров, который вы хотите просмотреть, и после закрытия окна выбора должен появиться список готовых запросов.</span><span class="sxs-lookup"><span data-stu-id="71150-186">Select **On** for the set of samples that you want to see, and then after closing the selection window, you should see a list of predefined requests.</span></span>

<span data-ttu-id="71150-187">После отправки запроса отображается код состояния и сообщение, а запрос выводится на вкладке **Просмотр отклика**.</span><span class="sxs-lookup"><span data-stu-id="71150-187">A status code and message are displayed after a request is sent and the response is shown in the **Response Preview** tab.</span></span>

### <a name="postman"></a><span data-ttu-id="71150-188">Postman</span><span class="sxs-lookup"><span data-stu-id="71150-188">Postman</span></span>

<span data-ttu-id="71150-189">Postman — это инструмент, который можно использовать для создания и тестирования запросов с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-189">Postman is a tool that you can use to build and test requests using the Microsoft Graph APIs.</span></span> <span data-ttu-id="71150-190">Вы можете скачать Postman по адресу: `https://www.getpostman.com/`.</span><span class="sxs-lookup"><span data-stu-id="71150-190">You can download Postman at: `https://www.getpostman.com/`.</span></span> <span data-ttu-id="71150-191">Чтобы взаимодействовать с Microsoft Graph в Postman, используйте коллекцию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-191">To interact with Microsoft Graph in Postman, you use the Microsoft Graph collection.</span></span>

<span data-ttu-id="71150-192">Дополнительные сведения см. в статье [Использование Postman с API Microsoft Graph](./use-postman.md).</span><span class="sxs-lookup"><span data-stu-id="71150-192">For more information, see [Use Postman with the Microsoft Graph API](./use-postman.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="71150-193">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="71150-193">Next steps</span></span>

<span data-ttu-id="71150-194">Все готово для настройки Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71150-194">You're ready to get up and running with Microsoft Graph.</span></span> <span data-ttu-id="71150-195">Воспользуйтесь [кратким руководством по началу работы](https://developer.microsoft.com/graph/quick-start) или начните использовать один из наших [пакетов SDK и примеров кода](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="71150-195">Try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>