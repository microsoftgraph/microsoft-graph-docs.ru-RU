---
author: swapnil1993
title: List contentTypes
description: Список типов контента на сайте или в списке
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 20d2b451a607a899f7873ba5be5aad671faad972
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770501"
---
# <a name="list-contenttypes"></a><span data-ttu-id="f6e69-103">List contentTypes</span><span class="sxs-lookup"><span data-stu-id="f6e69-103">List contentTypes</span></span>
<span data-ttu-id="f6e69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6e69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f6e69-105">Получить коллекцию типов [контента][contentType] на [сайте][] или в [списке][]</span><span class="sxs-lookup"><span data-stu-id="f6e69-105">Get the collection of [content types][contentType] in a [site][] or a [list][]</span></span>

## <a name="permissions"></a><span data-ttu-id="f6e69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6e69-106">Permissions</span></span>

<span data-ttu-id="f6e69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="f6e69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6e69-109">Permission type</span></span>      | <span data-ttu-id="f6e69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6e69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6e69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6e69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6e69-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f6e69-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="f6e69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6e69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6e69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6e69-114">Not supported.</span></span>    |
|<span data-ttu-id="f6e69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6e69-115">Application</span></span> | <span data-ttu-id="f6e69-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f6e69-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6e69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6e69-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes
GET /sites/{site-id}/lists/{list-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6e69-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6e69-118">Optional query parameters</span></span>

<span data-ttu-id="f6e69-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f6e69-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f6e69-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f6e69-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6e69-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6e69-121">Request headers</span></span>
|<span data-ttu-id="f6e69-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f6e69-122">Name</span></span>|<span data-ttu-id="f6e69-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f6e69-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6e69-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6e69-124">Authorization</span></span>|<span data-ttu-id="f6e69-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6e69-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6e69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6e69-127">Request body</span></span>
<span data-ttu-id="f6e69-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6e69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6e69-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6e69-129">Response</span></span>

<span data-ttu-id="f6e69-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [contentType](../resources/contenttype.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6e69-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6e69-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f6e69-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6e69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6e69-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f6e69-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6e69-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes
```
# <a name="c"></a>[<span data-ttu-id="f6e69-134">C#</span><span class="sxs-lookup"><span data-stu-id="f6e69-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-contenttypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6e69-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6e69-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-contenttypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6e69-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6e69-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-contenttypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6e69-137">Java</span><span class="sxs-lookup"><span data-stu-id="f6e69-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-contenttypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6e69-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6e69-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[list]: ../resources/list.md
