---
title: Список sourceCollections
description: Получите список ресурсов sourceCollections из объекта case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 801a526ef92cdffb5e262a830b5708db3a11e0ca
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080304"
---
# <a name="list-sourcecollections"></a><span data-ttu-id="8998b-103">Список sourceCollections</span><span class="sxs-lookup"><span data-stu-id="8998b-103">List sourceCollections</span></span>

<span data-ttu-id="8998b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8998b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8998b-105">Получите список [sourceCollections из](../resources/ediscovery-sourcecollection.md) объекта [case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="8998b-105">Get the list of [sourceCollections](../resources/ediscovery-sourcecollection.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8998b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8998b-106">Permissions</span></span>

<span data-ttu-id="8998b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8998b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8998b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8998b-109">Permission type</span></span>|<span data-ttu-id="8998b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8998b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8998b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8998b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8998b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8998b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8998b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8998b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8998b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8998b-114">Not supported.</span></span>|
|<span data-ttu-id="8998b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8998b-115">Application</span></span>|<span data-ttu-id="8998b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8998b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8998b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8998b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8998b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8998b-118">Optional query parameters</span></span>

<span data-ttu-id="8998b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8998b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8998b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8998b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8998b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8998b-121">Request headers</span></span>

|<span data-ttu-id="8998b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8998b-122">Name</span></span>|<span data-ttu-id="8998b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8998b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8998b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8998b-124">Authorization</span></span>|<span data-ttu-id="8998b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8998b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8998b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8998b-127">Request body</span></span>

<span data-ttu-id="8998b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8998b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8998b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8998b-129">Response</span></span>

<span data-ttu-id="8998b-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8998b-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8998b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8998b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8998b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8998b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8998b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8998b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections
```
# <a name="c"></a>[<span data-ttu-id="8998b-134">C#</span><span class="sxs-lookup"><span data-stu-id="8998b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8998b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8998b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8998b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8998b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8998b-137">Java</span><span class="sxs-lookup"><span data-stu-id="8998b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8998b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8998b-138">Response</span></span>

> <span data-ttu-id="8998b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8998b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.sourceCollection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/sourceCollections",
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2020-12-31T18:54:28.80694Z",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "contentQuery": "subject:'Quarterly Financials'",
            "dataSourceScopes": "allTenantMailboxes",
            "id": "fe5ef84e9c8c45819c056f6eb261718e",
            "displayName": "Quarterly Financials",
            "createdDateTime": "2020-12-11T22:56:14.2329133Z"
        }
    ]
}
```
