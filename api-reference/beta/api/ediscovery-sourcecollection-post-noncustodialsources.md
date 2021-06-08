---
title: Добавление noncustodialDataSource
description: Добавьте noncustodialSources, разместив их в коллекции noncustodialSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b6d3dde3e779aad317e3d2827e602d5097300d22
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786792"
---
# <a name="add-noncustodialdatasource"></a><span data-ttu-id="6c2d0-103">Добавление noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="6c2d0-103">Add noncustodialDataSource</span></span>

<span data-ttu-id="6c2d0-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6c2d0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c2d0-105">Добавьте noncustodialSources в [sourceCollection.](../api/ediscovery-sourcecollection-get.md)</span><span class="sxs-lookup"><span data-stu-id="6c2d0-105">Add noncustodialSources to a [sourceCollection](../api/ediscovery-sourcecollection-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c2d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c2d0-106">Permissions</span></span>

<span data-ttu-id="6c2d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c2d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c2d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c2d0-109">Permission type</span></span>|<span data-ttu-id="6c2d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c2d0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c2d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c2d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c2d0-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2d0-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6c2d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c2d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c2d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-114">Not supported.</span></span>|
|<span data-ttu-id="6c2d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c2d0-115">Application</span></span>|<span data-ttu-id="6c2d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c2d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c2d0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6c2d0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c2d0-118">Request headers</span></span>

|<span data-ttu-id="6c2d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6c2d0-119">Name</span></span>|<span data-ttu-id="6c2d0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c2d0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c2d0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c2d0-121">Authorization</span></span>|<span data-ttu-id="6c2d0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6c2d0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c2d0-124">Content-Type</span></span>|<span data-ttu-id="6c2d0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c2d0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c2d0-127">Request body</span></span>

<span data-ttu-id="6c2d0-128">В теле запроса подарят представление JSON объекта [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="6c2d0-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="6c2d0-129">В следующей таблице показаны свойства, необходимые при создании [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="6c2d0-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="6c2d0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c2d0-130">Property</span></span>|<span data-ttu-id="6c2d0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6c2d0-131">Type</span></span>|<span data-ttu-id="6c2d0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6c2d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c2d0-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="6c2d0-133">@odata.id</span></span>|<span data-ttu-id="6c2d0-134">String</span><span class="sxs-lookup"><span data-stu-id="6c2d0-134">String</span></span>|<span data-ttu-id="6c2d0-135">Строка, определяемая объектом custodial.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-135">String that defines the custodial object.</span></span> <span data-ttu-id="6c2d0-136">См. пример, который следует.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-136">See the example that follows.</span></span>  <span data-ttu-id="6c2d0-137">@odata.id можно получить из [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="6c2d0-137">The @odata.id can be retrieved from the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>|

## <a name="response"></a><span data-ttu-id="6c2d0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c2d0-138">Response</span></span>

<span data-ttu-id="6c2d0-139">В случае успешной работы этот метод возвращает код ответа и объект `204 No Content` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6c2d0-139">If successful, this method returns a `204 No Content` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c2d0-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c2d0-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c2d0-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c2d0-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c2d0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c2d0-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6c2d0-143">C#</span><span class="sxs-lookup"><span data-stu-id="6c2d0-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-noncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c2d0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c2d0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-noncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c2d0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c2d0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-noncustodialdatasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c2d0-146">Java</span><span class="sxs-lookup"><span data-stu-id="6c2d0-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-noncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c2d0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c2d0-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
