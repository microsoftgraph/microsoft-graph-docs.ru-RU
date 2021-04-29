---
title: Получение параметров
description: Ознакомьтесь с свойствами и отношениями объекта параметров.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1d4db6227db2793211f900adce5bbe2ca6a68efa
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080824"
---
# <a name="get-settings"></a><span data-ttu-id="26b61-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="26b61-103">Get settings</span></span>

<span data-ttu-id="26b61-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="26b61-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b61-105">Ознакомьтесь с свойствами и отношениями объекта [параметров.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="26b61-105">Read the properties and relationships of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26b61-106">Permissions</span></span>

<span data-ttu-id="26b61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b61-109">Permission type</span></span>|<span data-ttu-id="26b61-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b61-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26b61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26b61-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b61-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="26b61-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b61-114">Not supported.</span></span>|
|<span data-ttu-id="26b61-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b61-115">Application</span></span>|<span data-ttu-id="26b61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26b61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b61-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26b61-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26b61-118">Optional query parameters</span></span>

<span data-ttu-id="26b61-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="26b61-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="26b61-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="26b61-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="26b61-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26b61-121">Request headers</span></span>

|<span data-ttu-id="26b61-122">Имя</span><span class="sxs-lookup"><span data-stu-id="26b61-122">Name</span></span>|<span data-ttu-id="26b61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="26b61-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26b61-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26b61-124">Authorization</span></span>|<span data-ttu-id="26b61-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b61-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b61-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26b61-127">Request body</span></span>

<span data-ttu-id="26b61-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26b61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b61-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b61-129">Response</span></span>

<span data-ttu-id="26b61-130">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [параметров](../resources/ediscovery-settings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26b61-130">If successful, this method returns a `200 OK` response code and a [settings](../resources/ediscovery-settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26b61-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="26b61-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26b61-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b61-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/settings
```

### <a name="response"></a><span data-ttu-id="26b61-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b61-133">Response</span></span>

<span data-ttu-id="26b61-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26b61-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
