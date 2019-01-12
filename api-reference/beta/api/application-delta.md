---
title: 'приложение: дельты'
description: Get вновь созданных, обновлении или удалении приложения без необходимости выполнять полное чтение всего ресурсов коллекция. Для получения дополнительных сведений в разделе с помощью запроса дельты.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4479048865d50cb0887d938708cb44ff62a4a9b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917197"
---
# <a name="application-delta"></a><span data-ttu-id="da2e4-104">приложение: дельты</span><span class="sxs-lookup"><span data-stu-id="da2e4-104">application: delta</span></span>

> <span data-ttu-id="da2e4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da2e4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da2e4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da2e4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da2e4-107">Get вновь созданных, обновлении или удалении приложения без необходимости выполнять полное чтение всего ресурсов коллекция.</span><span class="sxs-lookup"><span data-stu-id="da2e4-107">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="da2e4-108">Для получения дополнительных сведений в разделе [С помощью запроса дельты](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="da2e4-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="da2e4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da2e4-109">Permissions</span></span>

<span data-ttu-id="da2e4-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="da2e4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da2e4-112">Permission type</span></span>      | <span data-ttu-id="da2e4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da2e4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da2e4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da2e4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="da2e4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da2e4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da2e4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da2e4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da2e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da2e4-117">Not supported.</span></span>    |
|<span data-ttu-id="da2e4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da2e4-118">Application</span></span> | <span data-ttu-id="da2e4-119">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da2e4-119">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da2e4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da2e4-120">HTTP request</span></span>

<span data-ttu-id="da2e4-121">Чтобы начать отслеживание изменений, выполнение запроса, включая функцию дельты на ресурс приложения.</span><span class="sxs-lookup"><span data-stu-id="da2e4-121">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="da2e4-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="da2e4-122">Query parameters</span></span>

<span data-ttu-id="da2e4-123">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="da2e4-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="da2e4-124">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="da2e4-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="da2e4-125">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="da2e4-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="da2e4-126">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="da2e4-126">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="da2e4-127">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="da2e4-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="da2e4-128">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="da2e4-128">Query parameter</span></span>      | <span data-ttu-id="da2e4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="da2e4-129">Type</span></span>   |<span data-ttu-id="da2e4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="da2e4-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da2e4-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="da2e4-131">$deltatoken</span></span> | <span data-ttu-id="da2e4-132">строка</span><span class="sxs-lookup"><span data-stu-id="da2e4-132">string</span></span> | <span data-ttu-id="da2e4-133">[Состояние токен](/graph/delta-query-overview) , возвращенный в `deltaLink` URL-адрес предыдущей вызов функции **дельты** для одной коллекции ресурсов, указывающее, завершения этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="da2e4-133">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="da2e4-134">Сохранить и применить весь `deltaLink` URL-адрес, включая этот маркер в первый запрос следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="da2e4-134">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="da2e4-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="da2e4-135">$skiptoken</span></span> | <span data-ttu-id="da2e4-136">строка</span><span class="sxs-lookup"><span data-stu-id="da2e4-136">string</span></span> | <span data-ttu-id="da2e4-137">[Состояние токен](/graph/delta-query-overview) , возвращенный в `nextLink` URL-адрес предыдущей вызов функции **дельты** , показывающее, есть дополнительные изменения в отслеживаются в одном семействе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="da2e4-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="da2e4-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da2e4-138">Optional query parameters</span></span>

<span data-ttu-id="da2e4-139">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da2e4-139">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="da2e4-p107">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="da2e4-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="da2e4-142">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="da2e4-142">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="da2e4-143">Поддерживаются только `$filter` выражение — для отслеживания изменений для конкретных ресурсы по идентификатору: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="da2e4-143">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="da2e4-144">Число идентификаторы, которые можно задать ограничивается Максимальная длина URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="da2e4-144">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="da2e4-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da2e4-145">Request headers</span></span>
| <span data-ttu-id="da2e4-146">Имя</span><span class="sxs-lookup"><span data-stu-id="da2e4-146">Name</span></span>       | <span data-ttu-id="da2e4-147">Описание</span><span class="sxs-lookup"><span data-stu-id="da2e4-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da2e4-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2e4-148">Authorization</span></span>  | <span data-ttu-id="da2e4-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="da2e4-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="da2e4-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da2e4-150">Content-Type</span></span>  | <span data-ttu-id="da2e4-151">application/json</span><span class="sxs-lookup"><span data-stu-id="da2e4-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="da2e4-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="da2e4-152">Request body</span></span>
<span data-ttu-id="da2e4-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da2e4-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="da2e4-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="da2e4-154">Response</span></span>

<span data-ttu-id="da2e4-155">Успешно завершена, этот метод возвращает `200 OK` кодов и [приложений](../resources/application.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="da2e4-155">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="da2e4-156">Ответ также содержит URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="da2e4-156">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="da2e4-157">Если `nextLink` возвращается URL-адрес, существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="da2e4-157">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="da2e4-158">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="da2e4-158">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="da2e4-159">Если `deltaLink` возвращается URL-адрес, нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="da2e4-159">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="da2e4-160">Сохранение и использование `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="da2e4-160">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="da2e4-161">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="da2e4-161">See:</span></span></br>
- <span data-ttu-id="da2e4-162">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="da2e4-162">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="da2e4-163">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="da2e4-163">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="da2e4-164">Пример</span><span class="sxs-lookup"><span data-stu-id="da2e4-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da2e4-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="da2e4-165">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a><span data-ttu-id="da2e4-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2e4-166">Response</span></span>
<span data-ttu-id="da2e4-p112">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da2e4-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
