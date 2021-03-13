---
title: Список legalHold userSources
description: Получите ресурсы userSource из свойства навигации userSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 447b33207596e2d438ae635e5e8050e63a4076a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773034"
---
# <a name="list-legalhold-usersources"></a><span data-ttu-id="3482a-103">Список legalHold userSources</span><span class="sxs-lookup"><span data-stu-id="3482a-103">List legalHold userSources</span></span>

<span data-ttu-id="3482a-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3482a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3482a-105">Получите список [объектов userSource,](../resources/ediscovery-usersource.md) связанных с юридическим удержанием.</span><span class="sxs-lookup"><span data-stu-id="3482a-105">Get the list of [userSource](../resources/ediscovery-usersource.md) objects associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="3482a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3482a-106">Permissions</span></span>

<span data-ttu-id="3482a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3482a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3482a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3482a-109">Permission type</span></span>|<span data-ttu-id="3482a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3482a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3482a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3482a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3482a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3482a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3482a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3482a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3482a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3482a-114">Not supported.</span></span>|
|<span data-ttu-id="3482a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3482a-115">Application</span></span>|<span data-ttu-id="3482a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3482a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3482a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3482a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3482a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3482a-118">Optional query parameters</span></span>

<span data-ttu-id="3482a-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3482a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3482a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3482a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3482a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3482a-121">Request headers</span></span>

|<span data-ttu-id="3482a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3482a-122">Name</span></span>|<span data-ttu-id="3482a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3482a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3482a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3482a-124">Authorization</span></span>|<span data-ttu-id="3482a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3482a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3482a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3482a-127">Request body</span></span>

<span data-ttu-id="3482a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3482a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3482a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3482a-129">Response</span></span>

<span data-ttu-id="3482a-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3482a-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3482a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3482a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3482a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3482a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3482a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3482a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/userSources
```
# <a name="c"></a>[<span data-ttu-id="3482a-134">C#</span><span class="sxs-lookup"><span data-stu-id="3482a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3482a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3482a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3482a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3482a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3482a-137">Java</span><span class="sxs-lookup"><span data-stu-id="3482a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3482a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3482a-138">Response</span></span>

<span data-ttu-id="3482a-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3482a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalholds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "2f279b24-2142-435d-97c5-0d42220ba453",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
