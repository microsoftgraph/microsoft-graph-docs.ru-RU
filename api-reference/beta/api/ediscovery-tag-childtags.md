---
title: Список childTags
description: Получите список объектов child [tag], связанных с тегом.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c8bc0511f45ff5caa0e7c8534859121831d28499
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776475"
---
# <a name="list-childtags"></a><span data-ttu-id="e03dc-103">Список childTags</span><span class="sxs-lookup"><span data-stu-id="e03dc-103">List childTags</span></span>

<span data-ttu-id="e03dc-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e03dc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e03dc-105">Получите список объектов детских [тегов,](../resources/ediscovery-tag.md) связанных с тегом.</span><span class="sxs-lookup"><span data-stu-id="e03dc-105">Get a list of child [tag](../resources/ediscovery-tag.md) objects associated with a tag.</span></span>

## <a name="permissions"></a><span data-ttu-id="e03dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e03dc-106">Permissions</span></span>

<span data-ttu-id="e03dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e03dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e03dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e03dc-109">Permission type</span></span>|<span data-ttu-id="e03dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e03dc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e03dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e03dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e03dc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e03dc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e03dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e03dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e03dc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03dc-114">Not supported.</span></span>|
|<span data-ttu-id="e03dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e03dc-115">Application</span></span>|<span data-ttu-id="e03dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e03dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e03dc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}/childTags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e03dc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e03dc-118">Optional query parameters</span></span>

<span data-ttu-id="e03dc-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e03dc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e03dc-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e03dc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e03dc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e03dc-121">Request headers</span></span>

|<span data-ttu-id="e03dc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e03dc-122">Name</span></span>|<span data-ttu-id="e03dc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e03dc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e03dc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e03dc-124">Authorization</span></span>|<span data-ttu-id="e03dc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e03dc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e03dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e03dc-127">Request body</span></span>

<span data-ttu-id="e03dc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e03dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e03dc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e03dc-129">Response</span></span>

<span data-ttu-id="e03dc-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e03dc-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e03dc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e03dc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e03dc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e03dc-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e03dc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e03dc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504/childTags
```
# <a name="c"></a>[<span data-ttu-id="e03dc-134">C#</span><span class="sxs-lookup"><span data-stu-id="e03dc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e03dc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e03dc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e03dc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e03dc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e03dc-137">Java</span><span class="sxs-lookup"><span data-stu-id="e03dc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e03dc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e03dc-138">Response</span></span>

<span data-ttu-id="e03dc-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e03dc-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.tag)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.ediscovery.tag)",
    "value": [
        {
            "displayName": "Yes",
            "description": "The document is responsive",
            "lastModifiedDateTime": "2021-01-11T19:32:22.4091161Z",
            "childSelectability": "One",
            "id": "081ff31e7324423186e01b549efe7033",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "childTags": []
        },
        {
            "displayName": "No",
            "description": "The document is not responsive",
            "lastModifiedDateTime": "2021-01-11T19:32:21.5693878Z",
            "childSelectability": "One",
            "id": "61624e6c96a64ccea40e0d2c48e23e16",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "childTags": []
        }
    ]
}
```
