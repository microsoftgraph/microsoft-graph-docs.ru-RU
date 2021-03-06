---
title: Get userSource
description: Ознакомьтесь с свойствами и отношениями объекта userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01ad2f83682ac786f35f423fa387293face51114
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515998"
---
# <a name="get-usersource"></a><span data-ttu-id="f62d1-103">Get userSource</span><span class="sxs-lookup"><span data-stu-id="f62d1-103">Get userSource</span></span>

<span data-ttu-id="f62d1-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f62d1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f62d1-105">Ознакомьтесь с свойствами и отношениями [объекта userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="f62d1-105">Read the properties and relationships of a [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f62d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f62d1-106">Permissions</span></span>

<span data-ttu-id="f62d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f62d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f62d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f62d1-109">Permission type</span></span>|<span data-ttu-id="f62d1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f62d1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f62d1-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f62d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f62d1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f62d1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f62d1-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f62d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f62d1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f62d1-114">Not supported.</span></span>|
|<span data-ttu-id="f62d1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f62d1-115">Application</span></span>|<span data-ttu-id="f62d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f62d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f62d1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f62d1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f62d1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f62d1-118">Optional query parameters</span></span>

<span data-ttu-id="f62d1-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f62d1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f62d1-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f62d1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f62d1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f62d1-121">Request headers</span></span>

|<span data-ttu-id="f62d1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f62d1-122">Name</span></span>|<span data-ttu-id="f62d1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f62d1-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f62d1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f62d1-124">Authorization</span></span>|<span data-ttu-id="f62d1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f62d1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f62d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f62d1-127">Request body</span></span>

<span data-ttu-id="f62d1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f62d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f62d1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f62d1-129">Response</span></span>

<span data-ttu-id="f62d1-130">В случае успеха этот метод возвращает код отклика и `200 OK` [объект microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f62d1-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f62d1-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f62d1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f62d1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f62d1-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f62d1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f62d1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="f62d1-134">C#</span><span class="sxs-lookup"><span data-stu-id="f62d1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f62d1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f62d1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f62d1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f62d1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f62d1-137">Java</span><span class="sxs-lookup"><span data-stu-id="f62d1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f62d1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f62d1-138">Response</span></span>

<span data-ttu-id="f62d1-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f62d1-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/userSources",
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
```
