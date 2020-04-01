---
title: 'orgContact: Delta'
description: Получите только что созданные, обновленные или удаленные организационные контакты, не требуя полного чтения всей коллекции.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48732e9d0b0e45405c3f9e167c05d5c5adef8426
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082197"
---
# <a name="orgcontact-delta"></a><span data-ttu-id="b5ada-103">orgContact: Delta</span><span class="sxs-lookup"><span data-stu-id="b5ada-103">orgContact: delta</span></span>

<span data-ttu-id="b5ada-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5ada-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5ada-105">Получите только что созданные, обновленные или удаленные организационные контакты, не требуя полного чтения всей коллекции.</span><span class="sxs-lookup"><span data-stu-id="b5ada-105">Get newly created, updated, or deleted organizational contacts without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="b5ada-106">Подробные сведения можно найти в разделе [Отслеживание изменений](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="b5ada-106">See [change tracking](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5ada-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5ada-107">Permissions</span></span>

<span data-ttu-id="b5ada-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5ada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5ada-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5ada-110">Permission type</span></span>      | <span data-ttu-id="b5ada-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5ada-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5ada-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5ada-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5ada-113">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b5ada-113">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5ada-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5ada-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5ada-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5ada-115">Not supported.</span></span>  |
|<span data-ttu-id="b5ada-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5ada-116">Application</span></span> | <span data-ttu-id="b5ada-117">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b5ada-117">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5ada-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5ada-118">HTTP request</span></span>

<span data-ttu-id="b5ada-119">Чтобы начать отслеживание изменений, необходимо создать запрос, включающий функцию Delta в ресурсе Contacts.</span><span class="sxs-lookup"><span data-stu-id="b5ada-119">To begin tracking changes, you make a request including the delta function on the contacts resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b5ada-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b5ada-120">Query parameters</span></span>

<span data-ttu-id="b5ada-121">Отслеживание изменений в контактах Организации приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="b5ada-121">Tracking changes in organizational contacts incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b5ada-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="b5ada-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b5ada-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="b5ada-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="b5ada-124">Необходимо указать только один из параметров запроса на передний план.</span><span class="sxs-lookup"><span data-stu-id="b5ada-124">You only need to specify any query parameters once up front.</span></span>

<span data-ttu-id="b5ada-125">В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="b5ada-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="b5ada-126">Этот URL-адрес уже включает в себя зашифрованные параметры.</span><span class="sxs-lookup"><span data-stu-id="b5ada-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="b5ada-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="b5ada-127">Query parameter</span></span>      | <span data-ttu-id="b5ada-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b5ada-128">Type</span></span>   |<span data-ttu-id="b5ada-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b5ada-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b5ada-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b5ada-130">$deltatoken</span></span> | <span data-ttu-id="b5ada-131">string</span><span class="sxs-lookup"><span data-stu-id="b5ada-131">string</span></span> | <span data-ttu-id="b5ada-132">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции контактов Организации, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="b5ada-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same organization contact collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="b5ada-133">Сохраните и примените весь `deltaLink` URL-адрес, включая этот маркер, в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="b5ada-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b5ada-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b5ada-134">$skiptoken</span></span> | <span data-ttu-id="b5ada-135">строка</span><span class="sxs-lookup"><span data-stu-id="b5ada-135">string</span></span> | <span data-ttu-id="b5ada-136">[Маркер состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая на то, что в коллекции контактов организации имеются дальнейшие изменения, которые необходимо отслеживать.</span><span class="sxs-lookup"><span data-stu-id="b5ada-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same organization contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="b5ada-137">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="b5ada-137">OData query parameters</span></span>

<span data-ttu-id="b5ada-138">Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5ada-138">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="b5ada-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="b5ada-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="b5ada-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="b5ada-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="b5ada-142">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="b5ada-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="b5ada-143">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="b5ada-143">You can filter multiple objects.</span></span> <span data-ttu-id="b5ada-144">Например, `https://graph.microsoft.com/v1.0/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="b5ada-144">For example, `https://graph.microsoft.com/v1.0/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="b5ada-145">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="b5ada-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5ada-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5ada-146">Request headers</span></span>
| <span data-ttu-id="b5ada-147">Имя</span><span class="sxs-lookup"><span data-stu-id="b5ada-147">Name</span></span>       | <span data-ttu-id="b5ada-148">Описание</span><span class="sxs-lookup"><span data-stu-id="b5ada-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5ada-149">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5ada-149">Authorization</span></span>  | <span data-ttu-id="b5ada-150">Носитель &lt;токен&gt;.</span><span class="sxs-lookup"><span data-stu-id="b5ada-150">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="b5ada-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5ada-151">Required.</span></span>|
| <span data-ttu-id="b5ada-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="b5ada-152">Prefer</span></span> | <span data-ttu-id="b5ada-153">return=minimal</span><span class="sxs-lookup"><span data-stu-id="b5ada-153">return=minimal</span></span> <br><br><span data-ttu-id="b5ada-154">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="b5ada-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="b5ada-155">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b5ada-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5ada-156">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5ada-156">Request body</span></span>
<span data-ttu-id="b5ada-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5ada-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5ada-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5ada-158">Response</span></span>

<span data-ttu-id="b5ada-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [orgContact](../resources/orgcontact.md) коллекции AB в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5ada-159">If successful, this method returns a `200 OK` response code and ab [orgContact](../resources/orgcontact.md) collection object in the response body.</span></span> <span data-ttu-id="b5ada-160">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b5ada-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="b5ada-161">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="b5ada-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="b5ada-162">Это указывает на то, что в сеансе можно получить дополнительные страницы данных.</span><span class="sxs-lookup"><span data-stu-id="b5ada-162">This indicates that there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="b5ada-163">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b5ada-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="b5ada-164">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="b5ada-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="b5ada-165">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="b5ada-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="b5ada-166">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="b5ada-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="b5ada-167">Это указывает на то, что больше нет данных о существующем состоянии ресурса, который необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="b5ada-167">This indicates that there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="b5ada-168">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="b5ada-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="b5ada-169">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b5ada-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="b5ada-170">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="b5ada-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="b5ada-171">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b5ada-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="b5ada-172">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="b5ada-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="b5ada-173">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="b5ada-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="b5ada-174">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="b5ada-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="b5ada-175">Если раньше свойство не было задано, оно не будет включено в ответ.</span><span class="sxs-lookup"><span data-stu-id="b5ada-175">If the property has never been set before, it will not be included in the response at all.</span></span>


> <span data-ttu-id="b5ada-176">**Примечание:** Таким образом, невозможно определить, изменяется ли свойство, изучив ответ.</span><span class="sxs-lookup"><span data-stu-id="b5ada-176">**Note:** With this behavior, it is not possible to tell whether a property is changing by looking at the response.</span></span> <span data-ttu-id="b5ada-177">Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств, как показано в [примере 2](#example-2-selecting-three-properties).</span><span class="sxs-lookup"><span data-stu-id="b5ada-177">Also, the delta responses tend to be large because they contain all property values,as shown in [Example 2](#example-2-selecting-three-properties).</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="b5ada-178">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="b5ada-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="b5ada-179">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="b5ada-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="b5ada-180">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="b5ada-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="b5ada-181">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="b5ada-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="b5ada-182">Если свойство не изменилось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="b5ada-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="b5ada-183">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="b5ada-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="b5ada-184">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="b5ada-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="b5ada-185">Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на порядок выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="b5ada-185">The header only affects the set of properties included in the response and it does not affect how the delta query is run.</span></span> <span data-ttu-id="b5ada-186">См. [пример 3](#example-3-alternative-minimal-response-behavior).</span><span class="sxs-lookup"><span data-stu-id="b5ada-186">See [Example 3](#example-3-alternative-minimal-response-behavior).</span></span>

## <a name="examples"></a><span data-ttu-id="b5ada-187">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5ada-187">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="b5ada-188">Пример 1. Свойства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b5ada-188">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="b5ada-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ada-189">Request</span></span>

<span data-ttu-id="b5ada-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5ada-190">The following is an example of the request.</span></span> <span data-ttu-id="b5ada-191">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5ada-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="b5ada-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ada-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgContact_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta
```
# <a name="c"></a>[<span data-ttu-id="b5ada-193">C#</span><span class="sxs-lookup"><span data-stu-id="b5ada-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5ada-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5ada-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5ada-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5ada-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5ada-196">Java</span><span class="sxs-lookup"><span data-stu-id="b5ada-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5ada-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ada-197">Response</span></span>

<span data-ttu-id="b5ada-198">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="b5ada-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="b5ada-p120">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5ada-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "id": "string (identifier)",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mailNickname": "mailNickname-value",
      "surname": "surname-value"
    }
  ]
}
```

### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="b5ada-201">Пример 2. Выбор трех свойств</span><span class="sxs-lookup"><span data-stu-id="b5ada-201">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="b5ada-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ada-202">Request</span></span>

<span data-ttu-id="b5ada-203">В следующем примере показан исходный запрос с выбором трех свойств для отслеживания изменений с поведением отклика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5ada-203">The next example shows the initial request selecting three properties for change tracking, with default response behavior.</span></span>


# <a name="http"></a>[<span data-ttu-id="b5ada-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ada-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta?$select=displayName,jobTitle,mail
```
# <a name="c"></a>[<span data-ttu-id="b5ada-205">C#</span><span class="sxs-lookup"><span data-stu-id="b5ada-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5ada-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5ada-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5ada-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5ada-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5ada-208">Java</span><span class="sxs-lookup"><span data-stu-id="b5ada-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5ada-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ada-209">Response</span></span>

<span data-ttu-id="b5ada-210">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="b5ada-210">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b5ada-211">Обратите внимание, что все три свойства включаются в отклик, и неизвестно, какие из них изменились с момента получения `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b5ada-211">Note that all three properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mail": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="b5ada-212">Пример 3. Альтернативное поведение минимального отклика</span><span class="sxs-lookup"><span data-stu-id="b5ada-212">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="b5ada-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ada-213">Request</span></span>

<span data-ttu-id="b5ada-214">В следующем примере показан исходный запрос с выбором трех свойств для отслеживания изменений с альтернативным поведением отклика с минимальными результатами.</span><span class="sxs-lookup"><span data-stu-id="b5ada-214">The next example shows the initial request selecting three properties for change tracking, with alternative minimal response behavior.</span></span>


# <a name="http"></a>[<span data-ttu-id="b5ada-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ada-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta?$select=displayName,jobTitle,mail
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="b5ada-216">C#</span><span class="sxs-lookup"><span data-stu-id="b5ada-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5ada-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5ada-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5ada-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5ada-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5ada-219">Java</span><span class="sxs-lookup"><span data-stu-id="b5ada-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5ada-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ada-220">Response</span></span>

<span data-ttu-id="b5ada-221">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="b5ada-221">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="b5ada-222">Обратите внимание, что свойство `mail` не включено, то есть оно не изменилось с последнего разностного запроса; `displayName` и `jobTitle` включены, то есть их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="b5ada-222">Note that the `mail` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a><span data-ttu-id="b5ada-223">См. также</span><span class="sxs-lookup"><span data-stu-id="b5ada-223">See also</span></span>

- <span data-ttu-id="b5ada-224">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="b5ada-224">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

<!-- uuid: 3B5A9A7C-6324-432F-8C66-AC4883DD71EF
2020-03-20 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
