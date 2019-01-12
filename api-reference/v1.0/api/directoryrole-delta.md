---
title: 'directoryRole: дельты'
description: Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов. Для получения дополнительных сведений в разделе с помощью запроса дельты.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6da3e8c4cf92edbf79df1b082675c36d54e81292
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923841"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="ba925-104">directoryRole: дельты</span><span class="sxs-lookup"><span data-stu-id="ba925-104">directoryRole: delta</span></span>

<span data-ttu-id="ba925-105">Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ba925-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="ba925-106">Для получения дополнительных сведений в разделе [С помощью запроса дельты](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="ba925-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba925-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba925-107">Permissions</span></span>

<span data-ttu-id="ba925-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba925-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ba925-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba925-110">Permission type</span></span>      | <span data-ttu-id="ba925-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba925-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba925-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba925-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba925-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba925-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba925-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba925-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba925-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba925-115">Not supported.</span></span>    |
|<span data-ttu-id="ba925-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba925-116">Application</span></span> | <span data-ttu-id="ba925-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba925-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba925-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba925-118">HTTP request</span></span>

<span data-ttu-id="ba925-119">Чтобы начать отслеживание изменений, внесите запроса, включая функцию **дельты** на [directoryRole](../resources/directoryrole.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ba925-119">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="ba925-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ba925-120">Query parameters</span></span>

<span data-ttu-id="ba925-121">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="ba925-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="ba925-122">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="ba925-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="ba925-123">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="ba925-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="ba925-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="ba925-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="ba925-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="ba925-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="ba925-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="ba925-126">Query parameter</span></span>      | <span data-ttu-id="ba925-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ba925-127">Type</span></span>   |<span data-ttu-id="ba925-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ba925-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba925-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="ba925-129">$deltatoken</span></span> | <span data-ttu-id="ba925-130">строка</span><span class="sxs-lookup"><span data-stu-id="ba925-130">string</span></span> | <span data-ttu-id="ba925-131">[Состояние токен](/graph/delta-query-overview) , возвращенный в `deltaLink` URL-адрес предыдущей вызов функции **дельты** для одной коллекции ресурсов, указывающее, завершения этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="ba925-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="ba925-132">Сохранить и применить весь `deltaLink` URL-адрес, включая этот маркер в первый запрос следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="ba925-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="ba925-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="ba925-133">$skiptoken</span></span> | <span data-ttu-id="ba925-134">строка</span><span class="sxs-lookup"><span data-stu-id="ba925-134">string</span></span> | <span data-ttu-id="ba925-135">[Состояние токен](/graph/delta-query-overview) , возвращенный в `nextLink` URL-адрес предыдущей вызов функции **дельты** , показывающее, есть дополнительные изменения в отслеживаются в одном семействе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ba925-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="ba925-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="ba925-136">OData query parameters</span></span>

<span data-ttu-id="ba925-137">Этот метод поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ba925-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="ba925-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="ba925-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="ba925-140">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="ba925-140">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="ba925-141">Поддерживаются только `$filter` выражение — для отслеживания изменений для конкретных ресурсы по идентификатору: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="ba925-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="ba925-142">Число идентификаторы, которые можно задать ограничивается Максимальная длина URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="ba925-142">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba925-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba925-143">Request headers</span></span>

| <span data-ttu-id="ba925-144">Имя</span><span class="sxs-lookup"><span data-stu-id="ba925-144">Name</span></span>       | <span data-ttu-id="ba925-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ba925-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ba925-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba925-146">Authorization</span></span>  | <span data-ttu-id="ba925-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="ba925-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="ba925-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba925-148">Content-Type</span></span>  | <span data-ttu-id="ba925-149">application/json</span><span class="sxs-lookup"><span data-stu-id="ba925-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba925-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba925-150">Request body</span></span>

<span data-ttu-id="ba925-151">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba925-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="ba925-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba925-152">Response</span></span>

<span data-ttu-id="ba925-153">Успешно завершена, этот метод возвращает `200 OK` кода и [directoryRole](../resources/directoryrole.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ba925-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="ba925-154">Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ba925-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="ba925-155">Если `nextLink` возвращается URL-адрес, существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="ba925-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="ba925-156">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="ba925-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="ba925-157">Если `deltaLink` возвращается URL-адрес, нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="ba925-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="ba925-158">Сохранение `deltaLink` URL-адрес и его применения в следующем вызове **дельты** сведения об изменениях в ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="ba925-158">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="ba925-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ba925-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ba925-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba925-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="ba925-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba925-161">Response</span></span>

<span data-ttu-id="ba925-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba925-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

### <a name="see-also"></a><span data-ttu-id="ba925-164">См. также</span><span class="sxs-lookup"><span data-stu-id="ba925-164">See also</span></span>

- <span data-ttu-id="ba925-165">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview) для получения дополнительных сведений</span><span class="sxs-lookup"><span data-stu-id="ba925-165">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="ba925-166">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="ba925-166">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
