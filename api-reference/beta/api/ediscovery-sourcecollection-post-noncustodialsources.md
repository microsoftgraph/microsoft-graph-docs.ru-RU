---
title: Добавление noncustodialDataSource
description: Добавьте noncustodialSources, разместив их в коллекции noncustodialSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 399d20f5bc046d141e8652001fe964460c2b414c
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080854"
---
# <a name="add-noncustodialdatasource"></a><span data-ttu-id="6e409-103">Добавление noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="6e409-103">Add noncustodialDataSource</span></span>

<span data-ttu-id="6e409-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6e409-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e409-105">Добавьте noncustodialSources в [sourceCollection.](../api/ediscovery-sourcecollection-get.md)</span><span class="sxs-lookup"><span data-stu-id="6e409-105">Add noncustodialSources to a [sourceCollection](../api/ediscovery-sourcecollection-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e409-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e409-106">Permissions</span></span>

<span data-ttu-id="6e409-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e409-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e409-109">Permission type</span></span>|<span data-ttu-id="6e409-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e409-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e409-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e409-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e409-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e409-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6e409-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e409-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e409-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e409-114">Not supported.</span></span>|
|<span data-ttu-id="6e409-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e409-115">Application</span></span>|<span data-ttu-id="6e409-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e409-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e409-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e409-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6e409-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e409-118">Request headers</span></span>

|<span data-ttu-id="6e409-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6e409-119">Name</span></span>|<span data-ttu-id="6e409-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6e409-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e409-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e409-121">Authorization</span></span>|<span data-ttu-id="6e409-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e409-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6e409-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e409-124">Content-Type</span></span>|<span data-ttu-id="6e409-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e409-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e409-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e409-127">Request body</span></span>

<span data-ttu-id="6e409-128">В теле запроса подарят представление JSON объекта [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="6e409-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="6e409-129">В следующей таблице показаны свойства, необходимые при создании [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="6e409-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="6e409-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e409-130">Property</span></span>|<span data-ttu-id="6e409-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e409-131">Type</span></span>|<span data-ttu-id="6e409-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e409-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e409-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="6e409-133">@odata.id</span></span>|<span data-ttu-id="6e409-134">String</span><span class="sxs-lookup"><span data-stu-id="6e409-134">String</span></span>|<span data-ttu-id="6e409-135">Строка, определяемая объектом custodial.</span><span class="sxs-lookup"><span data-stu-id="6e409-135">String that defines the custodial object.</span></span> <span data-ttu-id="6e409-136">См. пример, который следует.</span><span class="sxs-lookup"><span data-stu-id="6e409-136">See the example that follows.</span></span>  <span data-ttu-id="6e409-137">@odata.id можно получить из [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="6e409-137">The @odata.id can be retrieved from the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>|

## <a name="response"></a><span data-ttu-id="6e409-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e409-138">Response</span></span>

<span data-ttu-id="6e409-139">В случае успешной работы этот метод возвращает код ответа и объект `204 No Content` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6e409-139">If successful, this method returns a `204 No Content` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e409-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e409-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e409-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e409-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/sourceCollections/12aab1671c834213a84ba219c06f4c5a/noncustodialSources/$ref
Content-Type: application/json
Content-length: 206

{
    "@odata.id": "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
}
```

### <a name="response"></a><span data-ttu-id="6e409-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e409-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 204 No Content
```
