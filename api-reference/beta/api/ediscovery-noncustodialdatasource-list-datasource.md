---
title: List dataSource
description: Получите ресурсы dataSource из свойства навигации dataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 60cec935db8e451efa6e855c56b71eb026ca4f99
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080863"
---
# <a name="list-datasource"></a><span data-ttu-id="5c49f-103">List dataSource</span><span class="sxs-lookup"><span data-stu-id="5c49f-103">List dataSource</span></span>

<span data-ttu-id="5c49f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5c49f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c49f-105">Получите список dataSources, связанных с источником данных, не связанных с хранением.</span><span class="sxs-lookup"><span data-stu-id="5c49f-105">Get the list of dataSources associated with a non-custodial data source.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c49f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c49f-106">Permissions</span></span>

<span data-ttu-id="5c49f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c49f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c49f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c49f-109">Permission type</span></span>|<span data-ttu-id="5c49f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c49f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c49f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c49f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c49f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c49f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5c49f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c49f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c49f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c49f-114">Not supported.</span></span>|
|<span data-ttu-id="5c49f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c49f-115">Application</span></span>|<span data-ttu-id="5c49f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c49f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c49f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c49f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/dataSource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c49f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c49f-118">Optional query parameters</span></span>

<span data-ttu-id="5c49f-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5c49f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c49f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c49f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c49f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c49f-121">Request headers</span></span>

|<span data-ttu-id="5c49f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5c49f-122">Name</span></span>|<span data-ttu-id="5c49f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5c49f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c49f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c49f-124">Authorization</span></span>|<span data-ttu-id="5c49f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c49f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c49f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c49f-127">Request body</span></span>

<span data-ttu-id="5c49f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c49f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c49f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c49f-129">Response</span></span>

<span data-ttu-id="5c49f-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c49f-130">If successful, this method returns a `200 OK` response code and a collection of [dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c49f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c49f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c49f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c49f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/datasource
```

### <a name="response"></a><span data-ttu-id="5c49f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c49f-133">Response</span></span>

<span data-ttu-id="5c49f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c49f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources('8e402dd7f3c94a3abc086e5d07db1c6d')/dataSource/$entity",
        "@odata.type": "#microsoft.graph.ediscovery.userSource",
        "displayName": "Adele Vance",
        "createdDateTime": "2021-02-17T19:41:22.5902664Z",
        "id": "8e402dd7f3c94a3abc086e5d07db1c6d",
        "email": "AdeleV@contoso.com",
        "includedSources": "mailbox",
        "createdBy": {
            "user": {
                "id": "ediscovery admin",
                "displayName": "c1db6f13-332a-4d84-b111-914383ff9fc9"
            }
        }
      }
  ]

}
```
