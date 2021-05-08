---
title: 'параметры: resetToDefault'
description: Сбрасывает параметры случая к значениям по умолчанию.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3bc0cbcad51243e7f264ce69e92370cba864df54
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239701"
---
# <a name="settings-resettodefault"></a><span data-ttu-id="40966-103">параметры: resetToDefault</span><span class="sxs-lookup"><span data-stu-id="40966-103">settings: resetToDefault</span></span>

<span data-ttu-id="40966-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="40966-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40966-105">Сброс параметров дела в значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="40966-105">Reset the case settings to the default values.</span></span>

## <a name="permissions"></a><span data-ttu-id="40966-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40966-106">Permissions</span></span>

<span data-ttu-id="40966-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40966-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40966-109">Permission type</span></span>|<span data-ttu-id="40966-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40966-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40966-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40966-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40966-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40966-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="40966-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40966-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40966-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40966-114">Not supported.</span></span>|
|<span data-ttu-id="40966-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40966-115">Application</span></span>|<span data-ttu-id="40966-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40966-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40966-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40966-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

## <a name="request-headers"></a><span data-ttu-id="40966-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40966-118">Request headers</span></span>

|<span data-ttu-id="40966-119">Имя</span><span class="sxs-lookup"><span data-stu-id="40966-119">Name</span></span>|<span data-ttu-id="40966-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40966-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40966-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40966-121">Authorization</span></span>|<span data-ttu-id="40966-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40966-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40966-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40966-124">Request body</span></span>

<span data-ttu-id="40966-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40966-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40966-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="40966-126">Response</span></span>

<span data-ttu-id="40966-127">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="40966-127">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="40966-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="40966-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40966-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="40966-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="40966-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="40966-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "settings_resettodefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```
# <a name="c"></a>[<span data-ttu-id="40966-131">C#</span><span class="sxs-lookup"><span data-stu-id="40966-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/settings-resettodefault-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40966-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40966-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/settings-resettodefault-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40966-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40966-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/settings-resettodefault-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40966-134">Java</span><span class="sxs-lookup"><span data-stu-id="40966-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/settings-resettodefault-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40966-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40966-135">Response</span></span>

<span data-ttu-id="40966-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="40966-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
