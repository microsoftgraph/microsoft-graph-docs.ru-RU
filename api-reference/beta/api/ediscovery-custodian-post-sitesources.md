---
title: Создание сайта-хранителяSource
description: Создайте новый объект custodian siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01b4699e8f3625df4c046f23546709115b93551b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447053"
---
# <a name="create-custodian-sitesource"></a><span data-ttu-id="c4de6-103">Создание сайта-хранителяSource</span><span class="sxs-lookup"><span data-stu-id="c4de6-103">Create custodian siteSource</span></span>

<span data-ttu-id="c4de6-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c4de6-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4de6-105">Создайте новый объект [custodian siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="c4de6-105">Create a new custodian [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4de6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4de6-106">Permissions</span></span>

<span data-ttu-id="c4de6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4de6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4de6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4de6-109">Permission type</span></span>|<span data-ttu-id="c4de6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4de6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4de6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4de6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4de6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4de6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c4de6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4de6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4de6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4de6-114">Not supported.</span></span>|
|<span data-ttu-id="c4de6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4de6-115">Application</span></span>|<span data-ttu-id="c4de6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4de6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4de6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4de6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="c4de6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4de6-118">Request headers</span></span>

|<span data-ttu-id="c4de6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4de6-119">Name</span></span>|<span data-ttu-id="c4de6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4de6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4de6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4de6-121">Authorization</span></span>|<span data-ttu-id="c4de6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4de6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4de6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4de6-124">Content-Type</span></span>|<span data-ttu-id="c4de6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4de6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4de6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4de6-127">Request body</span></span>

<span data-ttu-id="c4de6-128">В теле запроса укажи представление JSON объекта [siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="c4de6-128">In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

<span data-ttu-id="c4de6-129">В следующей таблице показаны свойства, необходимые при создании [сайтаSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="c4de6-129">The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).</span></span>

|<span data-ttu-id="c4de6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4de6-130">Property</span></span>|<span data-ttu-id="c4de6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4de6-131">Type</span></span>|<span data-ttu-id="c4de6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4de6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4de6-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="c4de6-133">site@odata.bind</span></span>|<span data-ttu-id="c4de6-134">String</span><span class="sxs-lookup"><span data-stu-id="c4de6-134">String</span></span>|<span data-ttu-id="c4de6-135">ID сайта, который можно получить с ресурса [сайта](../resources/site.md) с помощью метода Get a site resource [by path.](../api/site-getbypath.md)</span><span class="sxs-lookup"><span data-stu-id="c4de6-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="c4de6-136">Использование {hostname}:/{relative-path}.</span><span class="sxs-lookup"><span data-stu-id="c4de6-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="c4de6-137">Для URL-адреса сайта `https://contoso.sharepoint.com/sites/HumanResources` запрос Microsoft Graph будет `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="c4de6-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="c4de6-138">ID — это первый GUID, указанный в поле ID.</span><span class="sxs-lookup"><span data-stu-id="c4de6-138">The ID is the first GUID listed in the ID field.</span></span>  <span data-ttu-id="c4de6-139">Для URL-адреса сайта OneDrive для бизнеса `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` запрос Microsoft Graph будет `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com` .</span><span class="sxs-lookup"><span data-stu-id="c4de6-139">For the OneDrive for Business site URL `https://contoso-my.sharepoint.com/personal/adelev_contoso_com`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`.</span></span> |

## <a name="response"></a><span data-ttu-id="c4de6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4de6-140">Response</span></span>

<span data-ttu-id="c4de6-141">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4de6-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4de6-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4de6-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4de6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4de6-143">Request</span></span>

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
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```

### <a name="response"></a><span data-ttu-id="c4de6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4de6-144">Response</span></span>

<span data-ttu-id="c4de6-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4de6-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
