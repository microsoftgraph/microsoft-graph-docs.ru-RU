---
title: Get legalHold
description: Ознакомьтесь с свойствами и отношениями объекта legalHold.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f2d276a85a6f95b845acef48fc3e823cb08be79b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447008"
---
# <a name="get-legalhold"></a><span data-ttu-id="75f2e-103">Get legalHold</span><span class="sxs-lookup"><span data-stu-id="75f2e-103">Get legalHold</span></span>

<span data-ttu-id="75f2e-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="75f2e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f2e-105">Ознакомьтесь с свойствами и отношениями объекта [legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="75f2e-105">Read the properties and relationships of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75f2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75f2e-106">Permissions</span></span>

<span data-ttu-id="75f2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75f2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75f2e-109">Permission type</span></span>|<span data-ttu-id="75f2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75f2e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75f2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75f2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75f2e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f2e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="75f2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75f2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75f2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f2e-114">Not supported.</span></span>|
|<span data-ttu-id="75f2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75f2e-115">Application</span></span>|<span data-ttu-id="75f2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75f2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75f2e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75f2e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75f2e-118">Optional query parameters</span></span>

<span data-ttu-id="75f2e-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="75f2e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="75f2e-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75f2e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="75f2e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75f2e-121">Request headers</span></span>

|<span data-ttu-id="75f2e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="75f2e-122">Name</span></span>|<span data-ttu-id="75f2e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="75f2e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75f2e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75f2e-124">Authorization</span></span>|<span data-ttu-id="75f2e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75f2e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75f2e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75f2e-127">Request body</span></span>

<span data-ttu-id="75f2e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75f2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75f2e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f2e-129">Response</span></span>

<span data-ttu-id="75f2e-130">В случае успеха этот метод возвращает код ответа и `200 OK` [объект microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75f2e-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75f2e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="75f2e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75f2e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f2e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

### <a name="response"></a><span data-ttu-id="75f2e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f2e-133">Response</span></span>

<span data-ttu-id="75f2e-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75f2e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.ediscovery.legalHold",
    "id": "700cd868-d868-700c-68d8-0c7068d80c70",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "isEnabled": "Boolean",
    "status": "String",
    "contentQuery": "String",
    "errors": [
      "String"
    ],
    "displayName": "String",
    "createdDateTime": "String (timestamp)"
  }
}
```
