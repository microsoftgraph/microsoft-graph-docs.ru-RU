---
author: JeremyKelley
ms.author: jeremyke
title: Пакеты списков
description: Список пакетов на диске пользователя
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 52d03febbb44448081c1a9f69066254e639d361b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441048"
---
# <a name="list-bundles"></a><span data-ttu-id="1f73d-103">Пакеты списков</span><span class="sxs-lookup"><span data-stu-id="1f73d-103">List bundles</span></span>

<span data-ttu-id="1f73d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f73d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f73d-105">Получение списка всех[пакетов] [пакетов на]диске пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f73d-105">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f73d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f73d-106">Permissions</span></span>

<span data-ttu-id="1f73d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f73d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f73d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f73d-109">Permission type</span></span>      | <span data-ttu-id="1f73d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f73d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f73d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f73d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f73d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f73d-112">Not supported.</span></span>                             |
|<span data-ttu-id="1f73d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f73d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f73d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f73d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f73d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f73d-115">Application</span></span>          | <span data-ttu-id="1f73d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f73d-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="1f73d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f73d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f73d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f73d-118">Optional query parameters</span></span>

<span data-ttu-id="1f73d-119">Этот метод поддерживает [параметры запросов OData][] для фильтрации и формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="1f73d-119">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="1f73d-120">Вы не можете использовать `expand=children` параметр запроса при перечислении пакетов.</span><span class="sxs-lookup"><span data-stu-id="1f73d-120">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f73d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f73d-121">Request headers</span></span>

| <span data-ttu-id="1f73d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1f73d-122">Name</span></span>          | <span data-ttu-id="1f73d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1f73d-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="1f73d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f73d-124">Authorization</span></span> | <span data-ttu-id="1f73d-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="1f73d-125">Bearer \{token\}.</span></span> <span data-ttu-id="1f73d-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="1f73d-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f73d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f73d-127">Request body</span></span>

<span data-ttu-id="1f73d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f73d-128">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f73d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f73d-129">Response</span></span>

<span data-ttu-id="1f73d-130">В случае успешного выполнения этот запрос возвращает список элементов пакета, определенных для диска.</span><span class="sxs-lookup"><span data-stu-id="1f73d-130">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="1f73d-131">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="1f73d-131">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="1f73d-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f73d-132">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="1f73d-133">Пример 1: список всех пакетов на диске</span><span class="sxs-lookup"><span data-stu-id="1f73d-133">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="1f73d-134">Чтобы запросить перечисление всех пакетов, определенных на диске, можно выполнить запрос к коллекции **пакетов** без каких-либо параметров.</span><span class="sxs-lookup"><span data-stu-id="1f73d-134">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="1f73d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f73d-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f73d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f73d-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="c"></a>[<span data-ttu-id="1f73d-137">C#</span><span class="sxs-lookup"><span data-stu-id="1f73d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f73d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f73d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f73d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f73d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f73d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f73d-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "0120310201abd",
      "name": "Family shared files",
      "bundle": {
        "childCount": 1
      }
    }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="1f73d-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f73d-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f73d-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f73d-142">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="1f73d-143">Пример 2: список всех фотоальбомов на диске</span><span class="sxs-lookup"><span data-stu-id="1f73d-143">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="1f73d-144">Чтобы отфильтровать список пакетов, возвращенных из запроса в коллекцию пакетов, можно использовать параметр строки `filter` запроса, чтобы указать тип возвращаемого пакета, проверяя наличие аспекта в пакете:</span><span class="sxs-lookup"><span data-stu-id="1f73d-144">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="1f73d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f73d-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f73d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f73d-146">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="1f73d-147">C#</span><span class="sxs-lookup"><span data-stu-id="1f73d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f73d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f73d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f73d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f73d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f73d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f73d-150">Response</span></span>

<span data-ttu-id="1f73d-151">Ответ на конечную точку GET to to-Arrays — это массив ресурсов [driveItem][] с [пакетом][].</span><span class="sxs-lookup"><span data-stu-id="1f73d-151">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="1f73d-152">Так как все пакеты являются элементами, можно использовать все стандартные операции с элементами.</span><span class="sxs-lookup"><span data-stu-id="1f73d-152">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "120301010abcd",
      "name": "Seattle Center event",
      "bundle": {
        "childCount": 4,
        "album": { }
      },
      "tags": [
        {
          "name": "outside",
          "autoTagged": { }
        }
      ]
    }
  ]
}
```

<span data-ttu-id="1f73d-153">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f73d-153">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f73d-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f73d-154">All the properties will be returned from an actual call.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[Параметры запроса OData]: /graph/query-parameters
[OData Query Parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "List the bundles in a drive.",
  "keywords": "list,bundle,collection",
  "section": "documentation",
  "tocPath": "Bundles/List"
} -->
