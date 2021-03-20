---
title: Создание legalHold siteSource
description: Создание нового объекта legalHold siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bca1f4c54593cc92f9b085bc86669981974e4432
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952463"
---
# <a name="create-legalhold-sitesource"></a><span data-ttu-id="ca912-103">Создание legalHold siteSource</span><span class="sxs-lookup"><span data-stu-id="ca912-103">Create legalHold siteSource</span></span>

<span data-ttu-id="ca912-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ca912-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca912-105">Добавляет siteSource в объект legalHold.</span><span class="sxs-lookup"><span data-stu-id="ca912-105">Adds a siteSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca912-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca912-106">Permissions</span></span>

<span data-ttu-id="ca912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca912-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca912-109">Permission type</span></span>|<span data-ttu-id="ca912-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca912-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca912-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca912-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca912-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca912-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ca912-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca912-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca912-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca912-114">Not supported.</span></span>|
|<span data-ttu-id="ca912-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca912-115">Application</span></span>|<span data-ttu-id="ca912-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca912-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca912-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca912-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="ca912-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca912-118">Request headers</span></span>

|<span data-ttu-id="ca912-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ca912-119">Name</span></span>|<span data-ttu-id="ca912-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ca912-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ca912-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca912-121">Authorization</span></span>|<span data-ttu-id="ca912-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca912-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ca912-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca912-124">Content-Type</span></span>|<span data-ttu-id="ca912-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca912-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca912-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca912-127">Request body</span></span>

<span data-ttu-id="ca912-128">В теле запроса укажи представление JSON объекта [siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="ca912-128">In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

<span data-ttu-id="ca912-129">В следующей таблице показаны свойства, необходимые при создании [сайтаSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="ca912-129">The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).</span></span>

|<span data-ttu-id="ca912-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca912-130">Property</span></span>|<span data-ttu-id="ca912-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca912-131">Type</span></span>|<span data-ttu-id="ca912-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca912-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca912-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="ca912-133">site@odata.bind</span></span>|<span data-ttu-id="ca912-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ca912-134">String</span></span>|<span data-ttu-id="ca912-135">ID сайта, который можно получить с ресурса [сайта](../resources/site.md) с помощью метода Get a site resource [by path.](../api/site-getbypath.md)</span><span class="sxs-lookup"><span data-stu-id="ca912-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="ca912-136">Использование {hostname}:/{relative-path}.</span><span class="sxs-lookup"><span data-stu-id="ca912-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="ca912-137">Для URL-адреса сайта `https://contoso.sharepoint.com/sites/HumanResources` запрос Microsoft Graph будет `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="ca912-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="ca912-138">ID — это первый GUID, указанный в поле ID.</span><span class="sxs-lookup"><span data-stu-id="ca912-138">The ID is the first GUID listed in the ID field.</span></span>  <span data-ttu-id="ca912-139">Для URL-адреса сайта OneDrive запрос `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` Microsoft Graph будет `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`</span><span class="sxs-lookup"><span data-stu-id="ca912-139">For the OneDrive for business site URL `https://contoso-my.sharepoint.com/personal/adelev_contoso_com`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`</span></span> |

## <a name="response"></a><span data-ttu-id="ca912-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca912-140">Response</span></span>

<span data-ttu-id="ca912-141">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ca912-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca912-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca912-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca912-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca912-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ca912-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca912-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/siteSources
Content-Type: application/json
Content-length: 154

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```
# <a name="c"></a>[<span data-ttu-id="ca912-145">C#</span><span class="sxs-lookup"><span data-stu-id="ca912-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca912-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca912-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca912-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca912-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca912-148">Java</span><span class="sxs-lookup"><span data-stu-id="ca912-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca912-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca912-149">Response</span></span>

<span data-ttu-id="ca912-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca912-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('387566cc-38ae-4e85-ab4b-cd2dd34faa07')/siteSources/$entity",
    "displayName": "Adele Vance",
    "createdDateTime": "2020-12-28T20:08:57.857Z",
    "id": "50073f3e-cb22-48e5-95a9-51a3da455181",
    "createdBy": {
        "user": {
            "id": null,
            "displayName": "EDiscovery admin"
        }
    }
}
```
