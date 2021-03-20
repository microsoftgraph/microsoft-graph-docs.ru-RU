---
title: Теги списка
description: Получите список ресурсов тегов из дела об обнаружении электронных источников.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f22f34bcb619580476d468cf52b48c2ec5adb792
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946374"
---
# <a name="list-tags"></a><span data-ttu-id="f22bb-103">Теги списка</span><span class="sxs-lookup"><span data-stu-id="f22bb-103">List tags</span></span>

<span data-ttu-id="f22bb-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f22bb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f22bb-105">Извлечение списка [объектов тегов](../resources/ediscovery-tag.md) из дела об обнаружении [электронных данных.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="f22bb-105">Retrieve a list of [tag](../resources/ediscovery-tag.md) objects from an eDiscovery [case](../resources/ediscovery-case.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f22bb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f22bb-106">Permissions</span></span>

<span data-ttu-id="f22bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f22bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f22bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f22bb-109">Permission type</span></span>|<span data-ttu-id="f22bb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f22bb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f22bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f22bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f22bb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22bb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f22bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f22bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f22bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f22bb-114">Not supported.</span></span>|
|<span data-ttu-id="f22bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f22bb-115">Application</span></span>|<span data-ttu-id="f22bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f22bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f22bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f22bb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f22bb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f22bb-118">Optional query parameters</span></span>

<span data-ttu-id="f22bb-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f22bb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f22bb-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f22bb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f22bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f22bb-121">Request headers</span></span>

|<span data-ttu-id="f22bb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f22bb-122">Name</span></span>|<span data-ttu-id="f22bb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f22bb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f22bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f22bb-124">Authorization</span></span>|<span data-ttu-id="f22bb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f22bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f22bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f22bb-127">Request body</span></span>

<span data-ttu-id="f22bb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f22bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f22bb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f22bb-129">Response</span></span>

<span data-ttu-id="f22bb-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f22bb-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f22bb-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f22bb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f22bb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f22bb-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f22bb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f22bb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tag_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
```
# <a name="c"></a>[<span data-ttu-id="f22bb-134">C#</span><span class="sxs-lookup"><span data-stu-id="f22bb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tag-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f22bb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f22bb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tag-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f22bb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f22bb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tag-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f22bb-137">Java</span><span class="sxs-lookup"><span data-stu-id="f22bb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tag-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f22bb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f22bb-138">Response</span></span>

<span data-ttu-id="f22bb-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f22bb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags",
    "value": [
        {
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
            "parent": null,
            "childTags": []
        },
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
            "parent": {
                "displayName": null,
                "createdBy": null,
                "description": null,
                "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                "childSelectability": "One",
                "id": "e54b3f535b434a9a8743b84e34c00504"
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
            "parent": {
                "displayName": null,
                "createdBy": null,
                "description": null,
                "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                "childSelectability": "One",
                "id": "e54b3f535b434a9a8743b84e34c00504"
            },
            "childTags": []
        }
    ]
}
```
