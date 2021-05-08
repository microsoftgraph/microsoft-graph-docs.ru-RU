---
title: Обновление параметров
description: Обновление свойств объекта параметров.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bbaf760948fc8ee7079e1c746405afddcd73a2b5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240836"
---
# <a name="update-settings"></a><span data-ttu-id="21f09-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="21f09-103">Update settings</span></span>

<span data-ttu-id="21f09-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="21f09-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21f09-105">Обновление свойств объекта [параметров.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="21f09-105">Update the properties of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21f09-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21f09-106">Permissions</span></span>

<span data-ttu-id="21f09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21f09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21f09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21f09-109">Permission type</span></span>|<span data-ttu-id="21f09-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21f09-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21f09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21f09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21f09-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21f09-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="21f09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21f09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21f09-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21f09-114">Not supported.</span></span>|
|<span data-ttu-id="21f09-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21f09-115">Application</span></span>|<span data-ttu-id="21f09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21f09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21f09-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21f09-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="21f09-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21f09-118">Request headers</span></span>

|<span data-ttu-id="21f09-119">Имя</span><span class="sxs-lookup"><span data-stu-id="21f09-119">Name</span></span>|<span data-ttu-id="21f09-120">Описание</span><span class="sxs-lookup"><span data-stu-id="21f09-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="21f09-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21f09-121">Authorization</span></span>|<span data-ttu-id="21f09-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21f09-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="21f09-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21f09-124">Content-Type</span></span>|<span data-ttu-id="21f09-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21f09-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21f09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21f09-127">Request body</span></span>

<span data-ttu-id="21f09-128">В теле запроса поставляем представление JSON объекта [параметров.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="21f09-128">In the request body, supply a JSON representation of the [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="21f09-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="21f09-129">Response</span></span>

<span data-ttu-id="21f09-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21f09-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="21f09-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="21f09-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21f09-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="21f09-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="21f09-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="21f09-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_settings"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings
Content-Type: application/json
Content-length: 350

{
    "redundancyDetection": {
        "isEnabled": false,
        "similarityThreshold": 70,
        "minWords": 12,
        "maxWords": 400000
    },
    "topicModeling": {
        "isEnabled": false,
        "ignoreNumbers": false,
        "topicCount": 50,
        "dynamicallyAdjustTopicCount": false
    },
    "ocr": {
        "isEnabled": true,
        "maxImageSize": 12000
    }
}
```
# <a name="c"></a>[<span data-ttu-id="21f09-134">C#</span><span class="sxs-lookup"><span data-stu-id="21f09-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21f09-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21f09-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21f09-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21f09-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21f09-137">Java</span><span class="sxs-lookup"><span data-stu-id="21f09-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21f09-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="21f09-138">Response</span></span>

<span data-ttu-id="21f09-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21f09-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
cache-control: no-cache
client-request-id: e9fc7554-ca5e-0928-fc09-9c5825820c88
content-length: 0
request-id: 1f53bd55-f099-46cb-91df-8f5d466aba3a
```
