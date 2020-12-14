---
title: Создание siteSource
description: Создание объекта siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0196fac3cf9b44915aa8f979072b2daadf6213f9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659089"
---
# <a name="create-sitesource"></a><span data-ttu-id="f7f7e-103">Создание siteSource</span><span class="sxs-lookup"><span data-stu-id="f7f7e-103">Create siteSource</span></span>

<span data-ttu-id="f7f7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7f7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7f7e-105">Создание объекта [siteSource.](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="f7f7e-105">Create a new [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7f7e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7f7e-106">Permissions</span></span>

<span data-ttu-id="f7f7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7f7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7f7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7f7e-109">Permission type</span></span>|<span data-ttu-id="f7f7e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7f7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7f7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7f7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7f7e-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="f7f7e-112">User.Read</span></span>|
|<span data-ttu-id="f7f7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7f7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7f7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-114">Not supported.</span></span>|
|<span data-ttu-id="f7f7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7f7e-115">Application</span></span>|<span data-ttu-id="f7f7e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7f7e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7f7e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="f7f7e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7f7e-118">Request headers</span></span>

|<span data-ttu-id="f7f7e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f7f7e-119">Name</span></span>|<span data-ttu-id="f7f7e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f7e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7f7e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7f7e-121">Authorization</span></span>|<span data-ttu-id="f7f7e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f7f7e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7f7e-124">Content-Type</span></span>|<span data-ttu-id="f7f7e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7f7e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7f7e-127">Request body</span></span>

<span data-ttu-id="f7f7e-128">В теле запроса укажу представление объекта [siteSource](../resources/sitesource.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-128">In the request body, supply a JSON representation of the [siteSource](../resources/sitesource.md) object.</span></span>

<span data-ttu-id="f7f7e-129">В следующей таблице показаны свойства, необходимые при создании [siteSource.](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="f7f7e-129">The following table shows the properties that are required when you create the [siteSource](../resources/sitesource.md).</span></span>

|<span data-ttu-id="f7f7e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7f7e-130">Property</span></span>|<span data-ttu-id="f7f7e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7f7e-131">Type</span></span>|<span data-ttu-id="f7f7e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7f7e-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="f7f7e-133">site@odata.bind</span></span>|<span data-ttu-id="f7f7e-134">String</span><span class="sxs-lookup"><span data-stu-id="f7f7e-134">String</span></span>|<span data-ttu-id="f7f7e-135">ИД сайта, который можно получить [](../resources/site.md) из ресурса сайта с помощью метода "Получить ресурс [сайта по пути".](../api/site-getbypath.md)</span><span class="sxs-lookup"><span data-stu-id="f7f7e-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="f7f7e-136">Для использования задается {hostname}:/{relative-path}.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="f7f7e-137">Для URL-адреса сайта запрос Microsoft Graph будет . `https://contoso.sharepoint.com/sites/HumanResources` `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`</span><span class="sxs-lookup"><span data-stu-id="f7f7e-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="f7f7e-138">ИД — это первый GUID, указанный в поле "ИД".</span><span class="sxs-lookup"><span data-stu-id="f7f7e-138">The ID is the first GUID listed in the ID field.</span></span>|

## <a name="response"></a><span data-ttu-id="f7f7e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f7e-139">Response</span></span>

<span data-ttu-id="f7f7e-140">В случае успеха этот метод возвращает код отклика и объект `201 Created` [siteSource](../resources/sitesource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-140">If successful, this method returns a `201 Created` response code and a [siteSource](../resources/sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7f7e-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7f7e-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7f7e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7f7e-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f7f7e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7f7e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
Content-Type: application/json
Content-length: 179

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/{siteId}"
}
```
# <a name="c"></a>[<span data-ttu-id="f7f7e-144">C#</span><span class="sxs-lookup"><span data-stu-id="f7f7e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7f7e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7f7e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7f7e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7f7e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7f7e-147">Java</span><span class="sxs-lookup"><span data-stu-id="f7f7e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7f7e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f7e-148">Response</span></span>

<span data-ttu-id="f7f7e-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Human resources site",
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
