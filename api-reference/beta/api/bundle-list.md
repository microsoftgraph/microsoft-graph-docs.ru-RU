---
author: JeremyKelley
ms.author: jeremyke
title: Пакеты списков
description: Список пакетов на диске пользователя
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5cae51aea05795279217040236d489b892722f5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317993"
---
# <a name="list-bundles"></a><span data-ttu-id="e690f-103">Пакеты списков</span><span class="sxs-lookup"><span data-stu-id="e690f-103">List bundles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e690f-104">Получение списка всех [][пакетов] пакетов на диске пользователя.</span><span class="sxs-lookup"><span data-stu-id="e690f-104">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e690f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e690f-105">Permissions</span></span>

<span data-ttu-id="e690f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e690f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e690f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e690f-108">Permission type</span></span>      | <span data-ttu-id="e690f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e690f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e690f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e690f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e690f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e690f-111">Not supported.</span></span>                             |
|<span data-ttu-id="e690f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e690f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e690f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e690f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e690f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e690f-114">Application</span></span>          | <span data-ttu-id="e690f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e690f-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="e690f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e690f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e690f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e690f-117">Optional query parameters</span></span>

<span data-ttu-id="e690f-118">Этот метод поддерживает [параметры запросов OData][] для фильтрации и формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="e690f-118">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="e690f-119">Вы не можете использовать `expand=children` параметр запроса при перечислении пакетов.</span><span class="sxs-lookup"><span data-stu-id="e690f-119">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e690f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e690f-120">Request headers</span></span>

| <span data-ttu-id="e690f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e690f-121">Name</span></span>          | <span data-ttu-id="e690f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e690f-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="e690f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e690f-123">Authorization</span></span> | <span data-ttu-id="e690f-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="e690f-124">Bearer \{token\}.</span></span> <span data-ttu-id="e690f-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e690f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e690f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e690f-126">Request body</span></span>

<span data-ttu-id="e690f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e690f-127">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="e690f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e690f-128">Response</span></span>

<span data-ttu-id="e690f-129">В случае успешного выполнения этот запрос возвращает список элементов пакета, определенных для диска.</span><span class="sxs-lookup"><span data-stu-id="e690f-129">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="e690f-130">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="e690f-130">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="e690f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e690f-131">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="e690f-132">Пример 1: список всех пакетов на диске</span><span class="sxs-lookup"><span data-stu-id="e690f-132">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="e690f-133">Чтобы запросить перечисление всех пакетов, определенных на диске, можно выполнить запрос к коллекции **пакетов** без каких-либо параметров.</span><span class="sxs-lookup"><span data-stu-id="e690f-133">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="e690f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e690f-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e690f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e690f-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e690f-136">C#</span><span class="sxs-lookup"><span data-stu-id="e690f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e690f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e690f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e690f-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e690f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e690f-139">Java</span><span class="sxs-lookup"><span data-stu-id="e690f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-all-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e690f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e690f-140">Response</span></span>

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

<span data-ttu-id="e690f-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e690f-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e690f-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e690f-142">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="e690f-143">Пример 2: список всех фотоальбомов на диске</span><span class="sxs-lookup"><span data-stu-id="e690f-143">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="e690f-144">Чтобы отфильтровать список пакетов, возвращенных из запроса в коллекцию пакетов, можно использовать параметр строки `filter` запроса, чтобы указать тип возвращаемого пакета, проверяя наличие аспекта в пакете:</span><span class="sxs-lookup"><span data-stu-id="e690f-144">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="e690f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e690f-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e690f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e690f-146">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e690f-147">C#</span><span class="sxs-lookup"><span data-stu-id="e690f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e690f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e690f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e690f-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e690f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e690f-150">Java</span><span class="sxs-lookup"><span data-stu-id="e690f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-album-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e690f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e690f-151">Response</span></span>

<span data-ttu-id="e690f-152">Ответ на конечную точку GET to to-Arrays — это массив ресурсов [driveItem][] с [пакетом][].</span><span class="sxs-lookup"><span data-stu-id="e690f-152">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="e690f-153">Так как все пакеты являются элементами, можно использовать все стандартные операции с элементами.</span><span class="sxs-lookup"><span data-stu-id="e690f-153">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

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

<span data-ttu-id="e690f-154">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e690f-154">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e690f-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e690f-155">All the properties will be returned from an actual call.</span></span>


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
