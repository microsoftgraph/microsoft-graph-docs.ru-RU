---
title: Список групп
description: Список всех групп, доступных в организации, в том числе групп Microsoft 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ea8ed7de6dab441f6311a96a74e014ccd7e625f
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796908"
---
# <a name="list-groups"></a><span data-ttu-id="cbc0b-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="cbc0b-103">List groups</span></span>

<span data-ttu-id="cbc0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbc0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cbc0b-105">Список всех групп в организации, в том числе групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="cbc0b-106">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-106">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="cbc0b-107">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="cbc0b-107">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="cbc0b-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-108">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="cbc0b-109">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbc0b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbc0b-110">Permissions</span></span>
<span data-ttu-id="cbc0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc0b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbc0b-113">Permission type</span></span>      | <span data-ttu-id="cbc0b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbc0b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbc0b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbc0b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cbc0b-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbc0b-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cbc0b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbc0b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbc0b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-118">Not supported.</span></span>    |
|<span data-ttu-id="cbc0b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbc0b-119">Application</span></span> | <span data-ttu-id="cbc0b-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbc0b-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbc0b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbc0b-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cbc0b-122">Optional query parameters</span></span>
<span data-ttu-id="cbc0b-123">Чтобы показать список только групп Microsoft 365 (т. н. единых групп), примените фильтр для **groupTypes** :</span><span class="sxs-lookup"><span data-stu-id="cbc0b-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes** :</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="cbc0b-124">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName** , как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="cbc0b-125">Вы также можете использовать параметры запроса `$count` и `$search`, чтобы ограничить ответ.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="cbc0b-126">Параметр запроса `$search` поддерживает разметку только в полях **displayName** и **description** .</span><span class="sxs-lookup"><span data-stu-id="cbc0b-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="cbc0b-127">По умолчанию в других полях используется действие `$filter`.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="cbc0b-128">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="cbc0b-129">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="cbc0b-130">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cbc0b-130">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbc0b-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbc0b-131">Request headers</span></span>

| <span data-ttu-id="cbc0b-132">Имя</span><span class="sxs-lookup"><span data-stu-id="cbc0b-132">Name</span></span> | <span data-ttu-id="cbc0b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cbc0b-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="cbc0b-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbc0b-134">Authorization</span></span>  | <span data-ttu-id="cbc0b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbc0b-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="cbc0b-137">ConsistencyLevel</span></span> | <span data-ttu-id="cbc0b-138">необязательный.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-138">eventual.</span></span> <span data-ttu-id="cbc0b-139">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="cbc0b-140">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbc0b-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbc0b-141">Request body</span></span>
<span data-ttu-id="cbc0b-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbc0b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-143">Response</span></span>
<span data-ttu-id="cbc0b-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="cbc0b-145">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="cbc0b-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="cbc0b-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="cbc0b-147">Пример 1. Получение списка групп</span><span class="sxs-lookup"><span data-stu-id="cbc0b-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="cbc0b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-148">Request</span></span>

<span data-ttu-id="cbc0b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="cbc0b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-150">Response</span></span>

<span data-ttu-id="cbc0b-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-151">The following is an example of the response.</span></span>

><span data-ttu-id="cbc0b-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cbc0b-153">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-153">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}

```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="cbc0b-154">Пример 2. Получение отфильтрованного списка групп, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="cbc0b-154">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

<span data-ttu-id="cbc0b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-155">The following is an example of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="cbc0b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cbc0b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-157">Response</span></span>

<span data-ttu-id="cbc0b-158">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-158">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
  "@odata.count":2,
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "displayName": "Contoso Group 1"
    },
    {
      "id": "22222222-3333-4444-5555-666666666666",
      "displayName": "Contoso Group 2"
    }
  ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="cbc0b-159">Пример 3. Получение только количества групп</span><span class="sxs-lookup"><span data-stu-id="cbc0b-159">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="cbc0b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-160">Request</span></span>

<span data-ttu-id="cbc0b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
  }-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cbc0b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-162">Response</span></span>

<span data-ttu-id="cbc0b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="cbc0b-164">Пример 4. Использование параметров $filter и $top для получения группы с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="cbc0b-164">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cbc0b-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-165">Request</span></span>

<span data-ttu-id="cbc0b-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cbc0b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-167">Response</span></span>

<span data-ttu-id="cbc0b-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-168">The following is an example of the response.</span></span>

><span data-ttu-id="cbc0b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mailNickname":"a241"
    }
  ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="cbc0b-171">Пример 5. Использование параметра $search для получения групп с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="cbc0b-171">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cbc0b-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-172">Request</span></span>

<span data-ttu-id="cbc0b-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cbc0b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-174">Response</span></span>

<span data-ttu-id="cbc0b-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-175">The following is an example of the response.</span></span>

><span data-ttu-id="cbc0b-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="cbc0b-178">Пример 6. Использование параметра $search для получения групп с отображаемыми именами, содержащими буквы "Video", или описания, содержащего буквы "prod", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="cbc0b-178">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cbc0b-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc0b-179">Request</span></span>

<span data-ttu-id="cbc0b-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-180">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cbc0b-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc0b-181">Response</span></span>

<span data-ttu-id="cbc0b-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-182">The following is an example of the response.</span></span>

><span data-ttu-id="cbc0b-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbc0b-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    },
    {
      "description":"Video Production",
      "displayName":"Video Production",
      "mail":"videoprod@service.contoso.com",
      "mailNickname":"VideoProduction"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

