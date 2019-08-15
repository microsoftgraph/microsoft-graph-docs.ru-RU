---
title: Создание Публишедресаурце
description: Создание нового объекта **публишедресаурце** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbb9bd814d8bb7947628145c62eb7717a4f2f83c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412343"
---
# <a name="create-publishedresource"></a><span data-ttu-id="fa3f0-103">Создание Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="fa3f0-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa3f0-104">Создание нового объекта [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="fa3f0-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa3f0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa3f0-105">Permissions</span></span>

<span data-ttu-id="fa3f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa3f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa3f0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa3f0-108">Permission type</span></span>                        | <span data-ttu-id="fa3f0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa3f0-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa3f0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa3f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa3f0-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa3f0-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="fa3f0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa3f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa3f0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-113">Not supported.</span></span> |
| <span data-ttu-id="fa3f0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa3f0-114">Application</span></span>                            | <span data-ttu-id="fa3f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa3f0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa3f0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="fa3f0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa3f0-117">Request headers</span></span>

| <span data-ttu-id="fa3f0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fa3f0-118">Name</span></span>      |<span data-ttu-id="fa3f0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fa3f0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa3f0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa3f0-120">Authorization</span></span> | <span data-ttu-id="fa3f0-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="fa3f0-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa3f0-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa3f0-122">Request body</span></span>

<span data-ttu-id="fa3f0-123">В тексте запроса добавьте представление объекта [публишедресаурце](../resources/publishedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="fa3f0-124">Укажите значения для следующих свойств.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="fa3f0-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa3f0-125">Property</span></span>     | <span data-ttu-id="fa3f0-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fa3f0-126">Type</span></span>        | <span data-ttu-id="fa3f0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fa3f0-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fa3f0-128">displayName</span><span class="sxs-lookup"><span data-stu-id="fa3f0-128">displayName</span></span>|<span data-ttu-id="fa3f0-129">String</span><span class="sxs-lookup"><span data-stu-id="fa3f0-129">String</span></span>|<span data-ttu-id="fa3f0-130">Отображаемое имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="fa3f0-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="fa3f0-131">resourceName</span></span>|<span data-ttu-id="fa3f0-132">String</span><span class="sxs-lookup"><span data-stu-id="fa3f0-132">String</span></span>|<span data-ttu-id="fa3f0-133">Имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="fa3f0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa3f0-134">Response</span></span>

<span data-ttu-id="fa3f0-135">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa3f0-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa3f0-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa3f0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa3f0-137">Request</span></span>

<span data-ttu-id="fa3f0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa3f0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa3f0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_publishedresource_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources
Content-Type: application/json

{
    "displayName": "New provisioning",
    "resourceName": "domain1.contoso.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa3f0-140">C#</span><span class="sxs-lookup"><span data-stu-id="fa3f0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa3f0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa3f0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa3f0-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fa3f0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa3f0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa3f0-143">Response</span></span>

<span data-ttu-id="fa3f0-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-144">The following is an example of the response.</span></span>

> <span data-ttu-id="fa3f0-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa3f0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 201 Created

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "publishingType": "provisioning",
    "displayName": "New provisionin",
    "resourceName": "domain1.contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
