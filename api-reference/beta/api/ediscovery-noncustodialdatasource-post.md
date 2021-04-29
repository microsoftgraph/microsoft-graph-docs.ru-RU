---
title: Создание noncustodialDataSource
description: Создайте новый объект noncustodialDataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 87817dfed8b4ba12c98661e847aa7e44302a7771
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080860"
---
# <a name="create-noncustodialdatasource"></a><span data-ttu-id="9f945-103">Создание noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="9f945-103">Create noncustodialDataSource</span></span>

<span data-ttu-id="9f945-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9f945-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f945-105">Создайте новый [объект noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="9f945-105">Create a new [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f945-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f945-106">Permissions</span></span>

<span data-ttu-id="9f945-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f945-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f945-109">Permission type</span></span>|<span data-ttu-id="9f945-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f945-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f945-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f945-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f945-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f945-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="9f945-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f945-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f945-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f945-114">Not supported.</span></span>|
|<span data-ttu-id="9f945-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f945-115">Application</span></span>|<span data-ttu-id="9f945-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f945-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f945-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f945-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
```

## <a name="request-headers"></a><span data-ttu-id="9f945-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f945-118">Request headers</span></span>

|<span data-ttu-id="9f945-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f945-119">Name</span></span>|<span data-ttu-id="9f945-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f945-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f945-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f945-121">Authorization</span></span>|<span data-ttu-id="9f945-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f945-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9f945-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f945-124">Content-Type</span></span>|<span data-ttu-id="9f945-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f945-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f945-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f945-127">Request body</span></span>

<span data-ttu-id="9f945-128">В теле запроса подарят представление JSON объекта [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="9f945-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="9f945-129">В следующей таблице показаны свойства, необходимые при создании [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="9f945-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="9f945-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f945-130">Property</span></span>|<span data-ttu-id="9f945-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f945-131">Type</span></span>|<span data-ttu-id="9f945-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f945-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f945-133">applyHoldToSource</span><span class="sxs-lookup"><span data-stu-id="9f945-133">applyHoldToSource</span></span>|<span data-ttu-id="9f945-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f945-134">Boolean</span></span>|<span data-ttu-id="9f945-135">Указывает, применяется ли удержание к источнику данных без хранения (например, к почтовому ящику или сайту).</span><span class="sxs-lookup"><span data-stu-id="9f945-135">Indicates if hold is applied to non-custodial data source (such as mailbox or site).</span></span>|
|<span data-ttu-id="9f945-136">datasource</span><span class="sxs-lookup"><span data-stu-id="9f945-136">datasource</span></span>|[<span data-ttu-id="9f945-137">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="9f945-137">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="9f945-138">Либо userSource, либо siteSource.</span><span class="sxs-lookup"><span data-stu-id="9f945-138">Either a userSource or siteSource.</span></span>  <span data-ttu-id="9f945-139">Для userSource используйте "dataSource": { "@odata.type": "microsoft.graph.ediscovery.userSource", "email" : "SMTP address"}.</span><span class="sxs-lookup"><span data-stu-id="9f945-139">For userSource, use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.userSource", "email" : "SMTP address"}.</span></span>  <span data-ttu-id="9f945-140">Для источника сайта используйте "dataSource": { "@odata.type": "microsoft.graph.ediscovery.siteSource", "site@odata.bind": "siteId" }, где siteId можно извлечь из URL-адреса сайта, например, запрос Microsoft Graph будет `https://contoso.sharepoint.com/sites/HumanResources` `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="9f945-140">For site source use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.siteSource", "site@odata.bind" : "siteId" }, where siteId can be derived from the site URL, e.g. `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="9f945-141">ID — это первый GUID, указанный в поле ID.</span><span class="sxs-lookup"><span data-stu-id="9f945-141">The ID is the first GUID listed in the ID field.</span></span>

## <a name="response"></a><span data-ttu-id="9f945-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f945-142">Response</span></span>

<span data-ttu-id="9f945-143">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f945-143">If successful, this method returns a `201 Created` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f945-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f945-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f945-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f945-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
Content-Type: application/json
Content-length: 206

{
    "applyHoldToSource" : true,
    "dataSource" : {
        "@odata.type" : "microsoft.graph.ediscovery.userSource",
        "email" : "adelev@contoso.com"
    }
}
```

### <a name="response"></a><span data-ttu-id="9f945-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f945-146">Response</span></span>

<span data-ttu-id="9f945-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f945-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "0",
    "lastModifiedDateTime": "2021-02-19T07:02:45.7732516Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "39374346363831303741353341373443",
    "displayName": null,
    "createdDateTime": "2021-02-19T07:02:45.4863718Z",
    "applyHoldToSource": true
}
```
