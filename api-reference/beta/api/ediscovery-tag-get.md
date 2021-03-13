---
title: Получить тег
description: Ознакомьтесь с свойствами и отношениями объекта тегов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c856ccc0c405c50062aaa6befcebc6292a3322e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775285"
---
# <a name="get-tag"></a><span data-ttu-id="7169d-103">Получить тег</span><span class="sxs-lookup"><span data-stu-id="7169d-103">Get tag</span></span>

<span data-ttu-id="7169d-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7169d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7169d-105">Ознакомьтесь с свойствами и отношениями объекта [тегов.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="7169d-105">Read the properties and relationships of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7169d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7169d-106">Permissions</span></span>

<span data-ttu-id="7169d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7169d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7169d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7169d-109">Permission type</span></span>|<span data-ttu-id="7169d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7169d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7169d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7169d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7169d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7169d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7169d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7169d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7169d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7169d-114">Not supported.</span></span>|
|<span data-ttu-id="7169d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7169d-115">Application</span></span>|<span data-ttu-id="7169d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7169d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7169d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7169d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7169d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7169d-118">Optional query parameters</span></span>

<span data-ttu-id="7169d-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7169d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7169d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7169d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7169d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7169d-121">Request headers</span></span>

|<span data-ttu-id="7169d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7169d-122">Name</span></span>|<span data-ttu-id="7169d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7169d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7169d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7169d-124">Authorization</span></span>|<span data-ttu-id="7169d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7169d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7169d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7169d-127">Request body</span></span>

<span data-ttu-id="7169d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7169d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7169d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7169d-129">Response</span></span>

<span data-ttu-id="7169d-130">В случае успешного решения этот метод возвращает код ответа и `200 OK` [объект microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7169d-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7169d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7169d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7169d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7169d-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7169d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7169d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
```
# <a name="c"></a>[<span data-ttu-id="7169d-134">C#</span><span class="sxs-lookup"><span data-stu-id="7169d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7169d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7169d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7169d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7169d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7169d-137">Java</span><span class="sxs-lookup"><span data-stu-id="7169d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7169d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7169d-138">Response</span></span>

<span data-ttu-id="7169d-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7169d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/tags/$entity",
    "displayName": "Responsiveness",
    "description": "Indicates the responsiveness of the document",
    "lastModifiedDateTime": "2021-01-11T19:32:23.1903658Z",
    "childSelectability": "One",
    "id": "e54b3f535b434a9a8743b84e34c00504",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalName": "admin@contoso.com"
        }
    },
    "childTags": []
}
```
