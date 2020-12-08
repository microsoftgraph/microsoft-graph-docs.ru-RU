---
title: Создание Ситесаурце
description: Создание нового объекта Ситесаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 93cb37a6ff94a52830675f876084fc85a6365a40
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597755"
---
# <a name="create-sitesource"></a><span data-ttu-id="53023-103">Создание Ситесаурце</span><span class="sxs-lookup"><span data-stu-id="53023-103">Create siteSource</span></span>

<span data-ttu-id="53023-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53023-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53023-105">Создание нового объекта [ситесаурце](../resources/sitesource.md) .</span><span class="sxs-lookup"><span data-stu-id="53023-105">Create a new [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53023-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53023-106">Permissions</span></span>

<span data-ttu-id="53023-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53023-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53023-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53023-109">Permission type</span></span>|<span data-ttu-id="53023-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53023-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53023-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53023-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53023-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="53023-112">User.Read</span></span>|
|<span data-ttu-id="53023-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53023-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53023-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53023-114">Not supported.</span></span>|
|<span data-ttu-id="53023-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53023-115">Application</span></span>|<span data-ttu-id="53023-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53023-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53023-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53023-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="53023-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53023-118">Request headers</span></span>

|<span data-ttu-id="53023-119">Имя</span><span class="sxs-lookup"><span data-stu-id="53023-119">Name</span></span>|<span data-ttu-id="53023-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53023-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53023-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53023-121">Authorization</span></span>|<span data-ttu-id="53023-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53023-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="53023-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53023-124">Content-Type</span></span>|<span data-ttu-id="53023-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53023-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53023-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53023-127">Request body</span></span>

<span data-ttu-id="53023-128">В тексте запроса добавьте представление объекта [ситесаурце](../resources/sitesource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53023-128">In the request body, supply a JSON representation of the [siteSource](../resources/sitesource.md) object.</span></span>

<span data-ttu-id="53023-129">В следующей таблице приведены свойства, необходимые при создании [ситесаурце](../resources/sitesource.md).</span><span class="sxs-lookup"><span data-stu-id="53023-129">The following table shows the properties that are required when you create the [siteSource](../resources/sitesource.md).</span></span>

|<span data-ttu-id="53023-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53023-130">Property</span></span>|<span data-ttu-id="53023-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53023-131">Type</span></span>|<span data-ttu-id="53023-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53023-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53023-133">site@odata. Bind</span><span class="sxs-lookup"><span data-stu-id="53023-133">site@odata.bind</span></span>|<span data-ttu-id="53023-134">String</span><span class="sxs-lookup"><span data-stu-id="53023-134">String</span></span>|<span data-ttu-id="53023-135">Идентификатор сайта, который можно получить из ресурса [сайта](../resources/site.md) с помощью метода [получения ресурса сайта по пути](../api/site-getbypath.md) .</span><span class="sxs-lookup"><span data-stu-id="53023-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="53023-136">Использование: {hostname}:/{релативе-Пас}.</span><span class="sxs-lookup"><span data-stu-id="53023-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="53023-137">Для URL-адреса сайта `https://contoso.sharepoint.com/sites/HumanResources` запрос Microsoft Graph будет иметь значение `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="53023-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="53023-138">Идентификатор является первым идентификатором GUID, указанным в поле ID.</span><span class="sxs-lookup"><span data-stu-id="53023-138">The ID is the first GUID listed in the ID field.</span></span>|

## <a name="response"></a><span data-ttu-id="53023-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="53023-139">Response</span></span>

<span data-ttu-id="53023-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ситесаурце](../resources/sitesource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53023-140">If successful, this method returns a `201 Created` response code and a [siteSource](../resources/sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53023-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="53023-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53023-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="53023-142">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="53023-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="53023-143">Response</span></span>

<span data-ttu-id="53023-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53023-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
