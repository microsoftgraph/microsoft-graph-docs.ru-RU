---
title: 'directoryRole: дельты'
description: Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов. Для получения дополнительных сведений в разделе с помощью запроса дельты.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bd84e593b4bf26a1cbdd41bf62624b0013f8d807
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508260"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="8d3fd-104">directoryRole: дельты</span><span class="sxs-lookup"><span data-stu-id="8d3fd-104">directoryRole: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d3fd-105">Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="8d3fd-106">Для получения дополнительных сведений в разделе [С помощью запроса дельты](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="8d3fd-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d3fd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3fd-107">Permissions</span></span>

<span data-ttu-id="8d3fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8d3fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3fd-110">Permission type</span></span>      | <span data-ttu-id="8d3fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d3fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d3fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d3fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d3fd-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d3fd-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d3fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d3fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-115">Not supported.</span></span>    |
|<span data-ttu-id="8d3fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d3fd-116">Application</span></span> | <span data-ttu-id="8d3fd-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d3fd-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d3fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d3fd-118">HTTP request</span></span>

<span data-ttu-id="8d3fd-119">Чтобы начать отслеживание изменений, внесите запроса, включая функцию дельты на directoryRole ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-119">To begin tracking changes, you make a request including the delta function on the directoryRole resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

### <a name="query-parameters"></a><span data-ttu-id="8d3fd-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8d3fd-120">Query parameters</span></span>

<span data-ttu-id="8d3fd-121">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="8d3fd-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="8d3fd-122">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="8d3fd-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="8d3fd-123">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="8d3fd-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="8d3fd-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="8d3fd-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="8d3fd-126">Query parameter</span></span>      | <span data-ttu-id="8d3fd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8d3fd-127">Type</span></span>   |<span data-ttu-id="8d3fd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3fd-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d3fd-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="8d3fd-129">$deltatoken</span></span> | <span data-ttu-id="8d3fd-130">string</span><span class="sxs-lookup"><span data-stu-id="8d3fd-130">string</span></span> | <span data-ttu-id="8d3fd-131">[Состояние токен](/graph/delta-query-overview) , возвращенный в `deltaLink` URL-адрес предыдущей вызов функции **дельты** для одной коллекции ресурсов, указывающее, завершения этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="8d3fd-132">Сохранить и применить весь `deltaLink` URL-адрес, включая этот маркер в первый запрос следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="8d3fd-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="8d3fd-133">$skiptoken</span></span> | <span data-ttu-id="8d3fd-134">строка</span><span class="sxs-lookup"><span data-stu-id="8d3fd-134">string</span></span> | <span data-ttu-id="8d3fd-135">[Состояние токен](/graph/delta-query-overview) , возвращенный в `nextLink` URL-адрес предыдущей вызов функции **дельты** , показывающее, есть дополнительные изменения в отслеживаются в одном семействе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8d3fd-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d3fd-136">Optional query parameters</span></span>

<span data-ttu-id="8d3fd-137">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="8d3fd-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="8d3fd-140">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="8d3fd-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="8d3fd-141">Поддерживаются только `$filter` выражение — для отслеживания изменений для конкретных ресурсы по идентификатору: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="8d3fd-142">Число идентификаторы, которые можно задать ограничивается Максимальная длина URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="8d3fd-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d3fd-143">Request headers</span></span>
| <span data-ttu-id="8d3fd-144">Имя</span><span class="sxs-lookup"><span data-stu-id="8d3fd-144">Name</span></span>       | <span data-ttu-id="8d3fd-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3fd-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d3fd-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d3fd-146">Authorization</span></span>  | <span data-ttu-id="8d3fd-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="8d3fd-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="8d3fd-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d3fd-148">Content-Type</span></span>  | <span data-ttu-id="8d3fd-149">application/json</span><span class="sxs-lookup"><span data-stu-id="8d3fd-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d3fd-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d3fd-150">Request body</span></span>
<span data-ttu-id="8d3fd-151">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="8d3fd-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d3fd-152">Response</span></span>

<span data-ttu-id="8d3fd-153">Успешно завершена, этот метод возвращает `200 OK` кода и [directoryRole](../resources/directoryrole.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="8d3fd-154">Ответ также содержит URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="8d3fd-155">Если `nextLink` возвращается URL-адрес, существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="8d3fd-156">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="8d3fd-157">Если `deltaLink` возвращается URL-адрес, нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="8d3fd-158">Сохранение и использование `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="8d3fd-159">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="8d3fd-159">See:</span></span></br>
- <span data-ttu-id="8d3fd-160">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="8d3fd-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="8d3fd-161">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="8d3fd-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="8d3fd-162">Пример</span><span class="sxs-lookup"><span data-stu-id="8d3fd-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d3fd-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3fd-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="8d3fd-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3fd-164">Response</span></span>
<span data-ttu-id="8d3fd-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d3fd-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
