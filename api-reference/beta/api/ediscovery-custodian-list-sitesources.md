---
title: Список хранителя сайтовSources
description: Получите список объектов siteSource и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c51de320f3d89d37b8c0e5d38d86ea93b61f5703
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447065"
---
# <a name="list-custodian-sitesources"></a><span data-ttu-id="c0b14-103">Список хранителя сайтовSources</span><span class="sxs-lookup"><span data-stu-id="c0b14-103">List custodian siteSources</span></span>

<span data-ttu-id="c0b14-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c0b14-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0b14-105">Получите список [объектов siteSource](../resources/ediscovery-sitesource.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="c0b14-105">Get a list of [siteSource](../resources/ediscovery-sitesource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0b14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0b14-106">Permissions</span></span>

<span data-ttu-id="c0b14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0b14-109">Permission type</span></span>|<span data-ttu-id="c0b14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0b14-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0b14-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0b14-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b14-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c0b14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0b14-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b14-114">Not supported.</span></span>|
|<span data-ttu-id="c0b14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0b14-115">Application</span></span>|<span data-ttu-id="c0b14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b14-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0b14-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0b14-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0b14-118">Optional query parameters</span></span>

<span data-ttu-id="c0b14-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c0b14-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c0b14-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c0b14-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0b14-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0b14-121">Request headers</span></span>

|<span data-ttu-id="c0b14-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c0b14-122">Name</span></span>|<span data-ttu-id="c0b14-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c0b14-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0b14-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0b14-124">Authorization</span></span>|<span data-ttu-id="c0b14-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0b14-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b14-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0b14-127">Request body</span></span>

<span data-ttu-id="c0b14-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0b14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0b14-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0b14-129">Response</span></span>

<span data-ttu-id="c0b14-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c0b14-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0b14-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0b14-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0b14-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0b14-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
```

### <a name="response"></a><span data-ttu-id="c0b14-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0b14-133">Response</span></span>

<span data-ttu-id="c0b14-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0b14-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
