---
title: Список хранителя userSources
description: Получите список объектов userSource и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3876e362365d00e62209bb8d9c852b0bbaddb756
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946199"
---
# <a name="list-custodian-usersources"></a><span data-ttu-id="6a935-103">Список хранителя userSources</span><span class="sxs-lookup"><span data-stu-id="6a935-103">List custodian userSources</span></span>

<span data-ttu-id="6a935-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6a935-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a935-105">Получите список объектов [userSource](../resources/ediscovery-usersource.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="6a935-105">Get a list of the [userSource](../resources/ediscovery-usersource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a935-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a935-106">Permissions</span></span>

<span data-ttu-id="6a935-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a935-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a935-109">Permission type</span></span>|<span data-ttu-id="6a935-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a935-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a935-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a935-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a935-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a935-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6a935-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a935-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a935-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a935-114">Not supported.</span></span>|
|<span data-ttu-id="6a935-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a935-115">Application</span></span>|<span data-ttu-id="6a935-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a935-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a935-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a935-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a935-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a935-118">Optional query parameters</span></span>

<span data-ttu-id="6a935-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6a935-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6a935-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6a935-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a935-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a935-121">Request headers</span></span>

|<span data-ttu-id="6a935-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6a935-122">Name</span></span>|<span data-ttu-id="6a935-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6a935-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a935-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a935-124">Authorization</span></span>|<span data-ttu-id="6a935-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a935-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a935-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a935-127">Request body</span></span>

<span data-ttu-id="6a935-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a935-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a935-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a935-129">Response</span></span>

<span data-ttu-id="6a935-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6a935-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a935-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a935-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a935-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a935-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a935-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a935-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
```
# <a name="c"></a>[<span data-ttu-id="6a935-134">C#</span><span class="sxs-lookup"><span data-stu-id="6a935-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a935-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a935-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a935-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a935-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a935-137">Java</span><span class="sxs-lookup"><span data-stu-id="6a935-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a935-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a935-138">Response</span></span>

<span data-ttu-id="6a935-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6a935-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/userSources",
    "value": [
        {
            "displayName": "Megan Bowen",
            "createdDateTime": "2020-08-21T13:20:01.3430206Z",
            "id": "46384443-4137-3032-3437-363939433735",
            "email": "megan@contoso.com",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "Adele Vance"
                }
            }
        }
    ]
}
```
