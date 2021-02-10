---
title: Get userSource
description: Чтение свойств и связей объекта userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9e93c53aa0c11baede8f956764b9d5de3d1f9bf7
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177076"
---
# <a name="get-usersource"></a><span data-ttu-id="5f50b-103">Get userSource</span><span class="sxs-lookup"><span data-stu-id="5f50b-103">Get userSource</span></span>

<span data-ttu-id="5f50b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f50b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f50b-105">Чтение свойств и связей объекта [userSource.](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="5f50b-105">Read the properties and relationships of a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f50b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f50b-106">Permissions</span></span>

<span data-ttu-id="5f50b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f50b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f50b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f50b-109">Permission type</span></span>|<span data-ttu-id="5f50b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f50b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f50b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f50b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f50b-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="5f50b-112">User.Read</span></span>|
|<span data-ttu-id="5f50b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f50b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f50b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f50b-114">Not supported.</span></span>|
|<span data-ttu-id="5f50b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f50b-115">Application</span></span>|<span data-ttu-id="5f50b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f50b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f50b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f50b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f50b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f50b-118">Optional query parameters</span></span>

<span data-ttu-id="5f50b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5f50b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f50b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5f50b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f50b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f50b-121">Request headers</span></span>

|<span data-ttu-id="5f50b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5f50b-122">Name</span></span>|<span data-ttu-id="5f50b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5f50b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f50b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f50b-124">Authorization</span></span>|<span data-ttu-id="5f50b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f50b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f50b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f50b-127">Request body</span></span>

<span data-ttu-id="5f50b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f50b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f50b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f50b-129">Response</span></span>

<span data-ttu-id="5f50b-130">В случае успеха этот метод возвращает код отклика и объект `200 OK` [userSource](../resources/usersource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f50b-130">If successful, this method returns a `200 OK` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f50b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f50b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f50b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f50b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5f50b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f50b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="5f50b-134">C#</span><span class="sxs-lookup"><span data-stu-id="5f50b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f50b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f50b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f50b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f50b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f50b-137">Java</span><span class="sxs-lookup"><span data-stu-id="5f50b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f50b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f50b-138">Response</span></span>

<span data-ttu-id="5f50b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5f50b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
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
