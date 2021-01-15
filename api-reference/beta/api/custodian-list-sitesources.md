---
title: Список siteSources
description: Получите список объектов siteSource и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 46f7b5d82da5d3ac66820199dac02b2797394d21
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872592"
---
# <a name="list-sitesources"></a><span data-ttu-id="a37b7-103">Список siteSources</span><span class="sxs-lookup"><span data-stu-id="a37b7-103">List siteSources</span></span>

<span data-ttu-id="a37b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a37b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a37b7-105">Получите список объектов [siteSource](../resources/sitesource.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a37b7-105">Get a list of [siteSource](../resources/sitesource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a37b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a37b7-106">Permissions</span></span>

<span data-ttu-id="a37b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a37b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a37b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a37b7-109">Permission type</span></span>|<span data-ttu-id="a37b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a37b7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a37b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a37b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a37b7-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="a37b7-112">User.Read</span></span>|
|<span data-ttu-id="a37b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a37b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a37b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a37b7-114">Not supported.</span></span>|
|<span data-ttu-id="a37b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a37b7-115">Application</span></span>|<span data-ttu-id="a37b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a37b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a37b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a37b7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a37b7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a37b7-118">Optional query parameters</span></span>

<span data-ttu-id="a37b7-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a37b7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a37b7-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a37b7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a37b7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a37b7-121">Request headers</span></span>

|<span data-ttu-id="a37b7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a37b7-122">Name</span></span>|<span data-ttu-id="a37b7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a37b7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a37b7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a37b7-124">Authorization</span></span>|<span data-ttu-id="a37b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a37b7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a37b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a37b7-127">Request body</span></span>

<span data-ttu-id="a37b7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a37b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a37b7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a37b7-129">Response</span></span>

<span data-ttu-id="a37b7-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [siteSource](../resources/sitesource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a37b7-130">If successful, this method returns a `200 OK` response code and a collection of [siteSource](../resources/sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a37b7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a37b7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a37b7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a37b7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a37b7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a37b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
```
# <a name="c"></a>[<span data-ttu-id="a37b7-134">C#</span><span class="sxs-lookup"><span data-stu-id="a37b7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a37b7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a37b7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a37b7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a37b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a37b7-137">Java</span><span class="sxs-lookup"><span data-stu-id="a37b7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a37b7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a37b7-138">Response</span></span>

<span data-ttu-id="a37b7-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a37b7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
