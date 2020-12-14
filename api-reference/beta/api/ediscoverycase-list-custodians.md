---
title: Список хранителей
description: Получите список объектов хранителя и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: d1d387e396b8ed413cb6796c6df95058363b7e6d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657172"
---
# <a name="list-custodians"></a><span data-ttu-id="c31f7-103">Список хранителей</span><span class="sxs-lookup"><span data-stu-id="c31f7-103">List custodians</span></span>

<span data-ttu-id="c31f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c31f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c31f7-105">Получите список объектов [хранителя](../resources/custodian.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="c31f7-105">Get a list of the [custodian](../resources/custodian.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c31f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c31f7-106">Permissions</span></span>

<span data-ttu-id="c31f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c31f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c31f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c31f7-109">Permission type</span></span>|<span data-ttu-id="c31f7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c31f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c31f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c31f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c31f7-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c31f7-112">User.Read</span></span>|
|<span data-ttu-id="c31f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c31f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c31f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c31f7-114">Not supported.</span></span>|
|<span data-ttu-id="c31f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c31f7-115">Application</span></span>|<span data-ttu-id="c31f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c31f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c31f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c31f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c31f7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c31f7-118">Optional query parameters</span></span>

<span data-ttu-id="c31f7-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c31f7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c31f7-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c31f7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c31f7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c31f7-121">Request headers</span></span>

|<span data-ttu-id="c31f7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c31f7-122">Name</span></span>|<span data-ttu-id="c31f7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c31f7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c31f7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c31f7-124">Authorization</span></span>|<span data-ttu-id="c31f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c31f7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c31f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c31f7-127">Request body</span></span>

<span data-ttu-id="c31f7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c31f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c31f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c31f7-129">Response</span></span>

<span data-ttu-id="c31f7-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [custodian](../resources/custodian.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c31f7-130">If successful, this method returns a `200 OK` response code and a collection of [custodian](../resources/custodian.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c31f7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c31f7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c31f7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c31f7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c31f7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c31f7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
```
# <a name="c"></a>[<span data-ttu-id="c31f7-134">C#</span><span class="sxs-lookup"><span data-stu-id="c31f7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c31f7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c31f7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c31f7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c31f7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c31f7-137">Java</span><span class="sxs-lookup"><span data-stu-id="c31f7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c31f7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c31f7-138">Response</span></span>

<span data-ttu-id="c31f7-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c31f7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.custodian)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians",
    "value": [
        {
            "email": "meganb@contoso.com",
            "applyHoldToSources": false,
            "status": "released",
            "createdDateTime": "2020-10-27T15:55:43.4971108Z",
            "lastModifiedDateTime": "2020-10-30T05:34:00.947558Z",
            "releasedDateTime": "2020-10-27T15:55:58.2338864Z",
            "acknowledgedDateTime": null,
            "id": "fd03ce02ecde42a58d24fcbc9ebbea3e",
            "displayName": "Megan Bowen"
        },
        {
            "email": "AdeleV@contoso.com",
            "applyHoldToSources": true,
            "status": "active",
            "createdDateTime": "2020-08-21T13:20:02.0117254Z",
            "lastModifiedDateTime": "2020-10-27T15:14:14.1244649Z",
            "releasedDateTime": null,
            "acknowledgedDateTime": null,
            "id": "2192ca408ea2410eba3bec8ae873be6b",
            "displayName": "Adele Vance"
        }
    ]
}
```
