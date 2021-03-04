---
title: Хранители списка
description: Получите список объектов хранителя и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c1f9bd5ffd6c046cd3403fb4ece6e7c23cc2a66a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447179"
---
# <a name="list-custodians"></a><span data-ttu-id="22d24-103">Хранители списка</span><span class="sxs-lookup"><span data-stu-id="22d24-103">List custodians</span></span>

<span data-ttu-id="22d24-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="22d24-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d24-105">Получите список объектов [хранителя](../resources/ediscovery-custodian.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="22d24-105">Get a list of the [custodian](../resources/ediscovery-custodian.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="22d24-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22d24-106">Permissions</span></span>

<span data-ttu-id="22d24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d24-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d24-109">Permission type</span></span>|<span data-ttu-id="22d24-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d24-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d24-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22d24-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d24-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="22d24-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d24-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d24-114">Not supported.</span></span>|
|<span data-ttu-id="22d24-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22d24-115">Application</span></span>|<span data-ttu-id="22d24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d24-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d24-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22d24-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22d24-118">Optional query parameters</span></span>

<span data-ttu-id="22d24-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="22d24-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="22d24-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="22d24-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22d24-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22d24-121">Request headers</span></span>

|<span data-ttu-id="22d24-122">Имя</span><span class="sxs-lookup"><span data-stu-id="22d24-122">Name</span></span>|<span data-ttu-id="22d24-123">Описание</span><span class="sxs-lookup"><span data-stu-id="22d24-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22d24-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22d24-124">Authorization</span></span>|<span data-ttu-id="22d24-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d24-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d24-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22d24-127">Request body</span></span>

<span data-ttu-id="22d24-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22d24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22d24-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d24-129">Response</span></span>

<span data-ttu-id="22d24-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="22d24-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22d24-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="22d24-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22d24-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d24-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
```

### <a name="response"></a><span data-ttu-id="22d24-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d24-133">Response</span></span>

<span data-ttu-id="22d24-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22d24-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.custodian)"
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
