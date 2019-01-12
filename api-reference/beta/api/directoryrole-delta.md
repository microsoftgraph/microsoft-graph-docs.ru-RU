---
title: 'directoryRole: дельты'
description: Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов. Для получения дополнительных сведений в разделе с помощью запроса дельты.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c5f17ed70426d8102870537354edf3cea9a723b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916749"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="05869-104">directoryRole: дельты</span><span class="sxs-lookup"><span data-stu-id="05869-104">directoryRole: delta</span></span>

> <span data-ttu-id="05869-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05869-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05869-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05869-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05869-107">Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="05869-107">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="05869-108">Для получения дополнительных сведений в разделе [С помощью запроса дельты](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="05869-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="05869-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05869-109">Permissions</span></span>

<span data-ttu-id="05869-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05869-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05869-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05869-112">Permission type</span></span>      | <span data-ttu-id="05869-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05869-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05869-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05869-114">Delegated (work or school account)</span></span> | <span data-ttu-id="05869-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05869-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05869-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05869-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05869-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05869-117">Not supported.</span></span>    |
|<span data-ttu-id="05869-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05869-118">Application</span></span> | <span data-ttu-id="05869-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05869-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05869-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05869-120">HTTP request</span></span>

<span data-ttu-id="05869-121">Чтобы начать отслеживание изменений, внесите запроса, включая функцию дельты на directoryRole ресурсов.</span><span class="sxs-lookup"><span data-stu-id="05869-121">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

### <a name="query-parameters"></a><span data-ttu-id="05869-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="05869-122">Query parameters</span></span>

<span data-ttu-id="05869-123">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="05869-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="05869-124">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="05869-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="05869-125">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="05869-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="05869-126">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="05869-126">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="05869-127">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="05869-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="05869-128">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="05869-128">Query parameter</span></span>      | <span data-ttu-id="05869-129">Тип</span><span class="sxs-lookup"><span data-stu-id="05869-129">Type</span></span>   |<span data-ttu-id="05869-130">Описание</span><span class="sxs-lookup"><span data-stu-id="05869-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05869-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="05869-131">$deltatoken</span></span> | <span data-ttu-id="05869-132">строка</span><span class="sxs-lookup"><span data-stu-id="05869-132">string</span></span> | <span data-ttu-id="05869-133">[Состояние токен](/graph/delta-query-overview) , возвращенный в `deltaLink` URL-адрес предыдущей вызов функции **дельты** для одной коллекции ресурсов, указывающее, завершения этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="05869-133">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="05869-134">Сохранить и применить весь `deltaLink` URL-адрес, включая этот маркер в первый запрос следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="05869-134">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="05869-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="05869-135">$skiptoken</span></span> | <span data-ttu-id="05869-136">строка</span><span class="sxs-lookup"><span data-stu-id="05869-136">string</span></span> | <span data-ttu-id="05869-137">[Состояние токен](/graph/delta-query-overview) , возвращенный в `nextLink` URL-адрес предыдущей вызов функции **дельты** , показывающее, есть дополнительные изменения в отслеживаются в одном семействе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="05869-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="05869-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05869-138">Optional query parameters</span></span>

<span data-ttu-id="05869-139">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05869-139">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="05869-p107">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="05869-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="05869-142">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="05869-142">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="05869-143">Поддерживаются только `$filter` выражение — для отслеживания изменений для конкретных ресурсы по идентификатору: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="05869-143">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="05869-144">Число идентификаторы, которые можно задать ограничивается Максимальная длина URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="05869-144">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="05869-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05869-145">Request headers</span></span>
| <span data-ttu-id="05869-146">Имя</span><span class="sxs-lookup"><span data-stu-id="05869-146">Name</span></span>       | <span data-ttu-id="05869-147">Описание</span><span class="sxs-lookup"><span data-stu-id="05869-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="05869-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="05869-148">Authorization</span></span>  | <span data-ttu-id="05869-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="05869-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="05869-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05869-150">Content-Type</span></span>  | <span data-ttu-id="05869-151">application/json</span><span class="sxs-lookup"><span data-stu-id="05869-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="05869-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05869-152">Request body</span></span>
<span data-ttu-id="05869-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05869-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="05869-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="05869-154">Response</span></span>

<span data-ttu-id="05869-155">Успешно завершена, этот метод возвращает `200 OK` кода и [directoryRole](../resources/directoryrole.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="05869-155">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="05869-156">Ответ также содержит URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="05869-156">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="05869-157">Если `nextLink` возвращается URL-адрес, существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="05869-157">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="05869-158">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="05869-158">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="05869-159">Если `deltaLink` возвращается URL-адрес, нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="05869-159">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="05869-160">Сохранение и использование `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="05869-160">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="05869-161">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="05869-161">See:</span></span></br>
- <span data-ttu-id="05869-162">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="05869-162">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="05869-163">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="05869-163">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="05869-164">Пример</span><span class="sxs-lookup"><span data-stu-id="05869-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05869-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="05869-165">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="05869-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="05869-166">Response</span></span>
<span data-ttu-id="05869-p112">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05869-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
