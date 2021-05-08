---
title: Получение параметров
description: Ознакомьтесь с свойствами и отношениями объекта параметров.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a119efd1541aef242bbe0d8ece72593d1871f012
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240880"
---
# <a name="get-settings"></a><span data-ttu-id="8c4e8-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="8c4e8-103">Get settings</span></span>

<span data-ttu-id="8c4e8-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8c4e8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c4e8-105">Ознакомьтесь с свойствами и отношениями объекта [параметров.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="8c4e8-105">Read the properties and relationships of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c4e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c4e8-106">Permissions</span></span>

<span data-ttu-id="8c4e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c4e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c4e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c4e8-109">Permission type</span></span>|<span data-ttu-id="8c4e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c4e8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c4e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c4e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c4e8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c4e8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8c4e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c4e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c4e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-114">Not supported.</span></span>|
|<span data-ttu-id="8c4e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c4e8-115">Application</span></span>|<span data-ttu-id="8c4e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c4e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c4e8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c4e8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c4e8-118">Optional query parameters</span></span>

<span data-ttu-id="8c4e8-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c4e8-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c4e8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c4e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c4e8-121">Request headers</span></span>

|<span data-ttu-id="8c4e8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8c4e8-122">Name</span></span>|<span data-ttu-id="8c4e8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8c4e8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c4e8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c4e8-124">Authorization</span></span>|<span data-ttu-id="8c4e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c4e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c4e8-127">Request body</span></span>

<span data-ttu-id="8c4e8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c4e8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c4e8-129">Response</span></span>

<span data-ttu-id="8c4e8-130">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [параметров](../resources/ediscovery-settings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-130">If successful, this method returns a `200 OK` response code and a [settings](../resources/ediscovery-settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c4e8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c4e8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c4e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c4e8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c4e8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c4e8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/settings
```
# <a name="c"></a>[<span data-ttu-id="8c4e8-134">C#</span><span class="sxs-lookup"><span data-stu-id="8c4e8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c4e8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c4e8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c4e8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c4e8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c4e8-137">Java</span><span class="sxs-lookup"><span data-stu-id="8c4e8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c4e8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c4e8-138">Response</span></span>

<span data-ttu-id="8c4e8-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c4e8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.settings"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/settings/$entity",
    "id": "5b840b94-f821-4c4a-8cad-3a90062bf51a",
    "redundancyDetection": {
        "isEnabled": true,
        "similarityThreshold": 65,
        "minWords": 10,
        "maxWords": 500000
    },
    "topicModeling": {
        "isEnabled": true,
        "ignoreNumbers": true,
        "topicCount": 100,
        "dynamicallyAdjustTopicCount": true
    },
    "ocr": {
        "isEnabled": false,
        "maxImageSize": 24576,
        "timeout": "PT1M"
    }
}
```
