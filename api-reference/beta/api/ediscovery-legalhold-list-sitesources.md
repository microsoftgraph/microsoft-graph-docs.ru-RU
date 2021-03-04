---
title: Список legalHold siteSources
description: Получите список objecs siteSource, связанных с юридическим удержанием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2e3be09db4a31a4bb8a3edf86194712f3aa4416c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447005"
---
# <a name="list-legalhold-sitesources"></a><span data-ttu-id="89a57-103">Список legalHold siteSources</span><span class="sxs-lookup"><span data-stu-id="89a57-103">List legalHold siteSources</span></span>

<span data-ttu-id="89a57-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="89a57-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89a57-105">Получите список [objecs siteSource,](../resources/ediscovery-sitesource.md) связанных с юридическим удержанием.</span><span class="sxs-lookup"><span data-stu-id="89a57-105">Get the list of [siteSource](../resources/ediscovery-sitesource.md) objecs associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="89a57-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89a57-106">Permissions</span></span>

<span data-ttu-id="89a57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions- reference).</span><span class="sxs-lookup"><span data-stu-id="89a57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions- reference).</span></span>

|<span data-ttu-id="89a57-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89a57-109">Permission type</span></span>|<span data-ttu-id="89a57-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89a57-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89a57-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89a57-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89a57-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89a57-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="89a57-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89a57-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89a57-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89a57-114">Not supported.</span></span>|
|<span data-ttu-id="89a57-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89a57-115">Application</span></span>|<span data-ttu-id="89a57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89a57-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89a57-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89a57-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89a57-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89a57-118">Optional query parameters</span></span>

<span data-ttu-id="89a57-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="89a57-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="89a57-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="89a57-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89a57-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89a57-121">Request headers</span></span>

|<span data-ttu-id="89a57-122">Имя</span><span class="sxs-lookup"><span data-stu-id="89a57-122">Name</span></span>|<span data-ttu-id="89a57-123">Описание</span><span class="sxs-lookup"><span data-stu-id="89a57-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89a57-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89a57-124">Authorization</span></span>|<span data-ttu-id="89a57-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89a57-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89a57-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89a57-127">Request body</span></span>

<span data-ttu-id="89a57-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89a57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89a57-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="89a57-129">Response</span></span>

<span data-ttu-id="89a57-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="89a57-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89a57-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="89a57-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89a57-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89a57-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources
```

### <a name="response"></a><span data-ttu-id="89a57-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="89a57-133">Response</span></span>

<span data-ttu-id="89a57-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="89a57-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "43aab990-183e-4593-b772-578bb129e89b",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        },
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "e87b37ac-fad4-471b-9dd8-0e16000a3554",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
