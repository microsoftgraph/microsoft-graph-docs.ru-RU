---
title: 'servicePrincipal: дельты'
description: Get вновь созданных, обновлении или удалении субъектов-служб без необходимости выполнения полного чтения коллекции всей ресурсов. Для получения дополнительных сведений в разделе с помощью запроса дельты.
ms.openlocfilehash: 27653df1444ca83ef819d51813a813b169f3ad7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079590"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="72fa2-104">servicePrincipal: дельты</span><span class="sxs-lookup"><span data-stu-id="72fa2-104">servicePrincipal: delta</span></span>

> <span data-ttu-id="72fa2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72fa2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72fa2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72fa2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72fa2-107">Get вновь созданных, обновлении или удалении субъектов-служб без необходимости выполнения полного чтения коллекции всей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="72fa2-107">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="72fa2-108">Для получения дополнительных сведений в разделе [С помощью запроса дельты](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="72fa2-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="72fa2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72fa2-109">Permissions</span></span>

<span data-ttu-id="72fa2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72fa2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="72fa2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72fa2-112">Permission type</span></span>      | <span data-ttu-id="72fa2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72fa2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72fa2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72fa2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="72fa2-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72fa2-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72fa2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72fa2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72fa2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72fa2-117">Not supported.</span></span>    |
|<span data-ttu-id="72fa2-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="72fa2-118">Application</span></span> | <span data-ttu-id="72fa2-119">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="72fa2-119">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72fa2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72fa2-120">HTTP request</span></span>

<span data-ttu-id="72fa2-121">Чтобы начать отслеживание изменений, внесите запроса, включая функцию дельты на servicePrincipal ресурсов.</span><span class="sxs-lookup"><span data-stu-id="72fa2-121">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="72fa2-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="72fa2-122">Query parameters</span></span>

<span data-ttu-id="72fa2-123">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="72fa2-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="72fa2-124">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="72fa2-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="72fa2-125">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="72fa2-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="72fa2-126">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="72fa2-126">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="72fa2-127">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="72fa2-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="72fa2-128">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="72fa2-128">Query parameter</span></span>      | <span data-ttu-id="72fa2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="72fa2-129">Type</span></span>   |<span data-ttu-id="72fa2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="72fa2-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="72fa2-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="72fa2-131">$deltatoken</span></span> | <span data-ttu-id="72fa2-132">строка</span><span class="sxs-lookup"><span data-stu-id="72fa2-132">string</span></span> | <span data-ttu-id="72fa2-133">[Состояние токен](/graph/delta-query-overview) , возвращенный в `deltaLink` URL-адрес предыдущей вызов функции **дельты** для одной коллекции ресурсов, указывающее, завершения этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="72fa2-133">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="72fa2-134">Сохранить и применить весь `deltaLink` URL-адрес, включая этот маркер в первый запрос следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="72fa2-134">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="72fa2-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="72fa2-135">$skiptoken</span></span> | <span data-ttu-id="72fa2-136">строка</span><span class="sxs-lookup"><span data-stu-id="72fa2-136">string</span></span> | <span data-ttu-id="72fa2-137">[Состояние токен](/graph/delta-query-overview) , возвращенный в `nextLink` URL-адрес предыдущей вызов функции **дельты** , показывающее, есть дополнительные изменения в отслеживаются в одном семействе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="72fa2-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="72fa2-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72fa2-138">Optional query parameters</span></span>

<span data-ttu-id="72fa2-139">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72fa2-139">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="72fa2-p107">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="72fa2-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="72fa2-142">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="72fa2-142">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="72fa2-143">Поддерживаются только `$filter` выражение — для отслеживания изменений для конкретных ресурсы по идентификатору: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="72fa2-143">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="72fa2-144">Число идентификаторы, которые можно задать ограничивается Максимальная длина URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="72fa2-144">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="72fa2-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72fa2-145">Request headers</span></span>
| <span data-ttu-id="72fa2-146">Имя</span><span class="sxs-lookup"><span data-stu-id="72fa2-146">Name</span></span>       | <span data-ttu-id="72fa2-147">Описание</span><span class="sxs-lookup"><span data-stu-id="72fa2-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72fa2-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="72fa2-148">Authorization</span></span>  | <span data-ttu-id="72fa2-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="72fa2-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="72fa2-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72fa2-150">Content-Type</span></span>  | <span data-ttu-id="72fa2-151">application/json</span><span class="sxs-lookup"><span data-stu-id="72fa2-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="72fa2-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72fa2-152">Request body</span></span>
<span data-ttu-id="72fa2-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72fa2-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="72fa2-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="72fa2-154">Response</span></span>

<span data-ttu-id="72fa2-155">Успешно завершена, этот метод возвращает `200 OK` кода и [servicePrincipal](../resources/serviceprincipal.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="72fa2-155">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="72fa2-156">Ответ также содержит URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="72fa2-156">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="72fa2-157">Если `nextLink` возвращается URL-адрес, существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="72fa2-157">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="72fa2-158">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="72fa2-158">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="72fa2-159">Если `deltaLink` возвращается URL-адрес, нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="72fa2-159">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="72fa2-160">Сохранение и использование `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="72fa2-160">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="72fa2-161">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="72fa2-161">See:</span></span></br>
- <span data-ttu-id="72fa2-162">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="72fa2-162">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="72fa2-163">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="72fa2-163">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="72fa2-164">Пример</span><span class="sxs-lookup"><span data-stu-id="72fa2-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72fa2-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="72fa2-165">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```

##### <a name="response"></a><span data-ttu-id="72fa2-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="72fa2-166">Response</span></span>
<span data-ttu-id="72fa2-p112">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72fa2-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->