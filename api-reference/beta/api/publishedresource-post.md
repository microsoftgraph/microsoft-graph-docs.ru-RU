---
title: Создание publishedResource
description: Создание объекта **publishedResource.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2b87c40556cb7612e6c354ddb8e5815fb4d08760
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130391"
---
# <a name="create-publishedresource"></a><span data-ttu-id="40a8b-103">Создание publishedResource</span><span class="sxs-lookup"><span data-stu-id="40a8b-103">Create publishedResource</span></span>

<span data-ttu-id="40a8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40a8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40a8b-105">Создание объекта [publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="40a8b-105">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40a8b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40a8b-106">Permissions</span></span>

<span data-ttu-id="40a8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40a8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40a8b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40a8b-109">Permission type</span></span>                        | <span data-ttu-id="40a8b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40a8b-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="40a8b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40a8b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40a8b-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40a8b-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="40a8b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40a8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40a8b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40a8b-114">Not supported.</span></span> |
| <span data-ttu-id="40a8b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40a8b-115">Application</span></span>                            | <span data-ttu-id="40a8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40a8b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40a8b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40a8b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="40a8b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40a8b-118">Request headers</span></span>

| <span data-ttu-id="40a8b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="40a8b-119">Name</span></span>      |<span data-ttu-id="40a8b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40a8b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40a8b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40a8b-121">Authorization</span></span> | <span data-ttu-id="40a8b-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="40a8b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="40a8b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40a8b-123">Request body</span></span>

<span data-ttu-id="40a8b-124">В теле запроса укажу представление объекта [publishedResource](../resources/publishedresource.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="40a8b-124">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="40a8b-125">Укавите значения для следующих свойств.</span><span class="sxs-lookup"><span data-stu-id="40a8b-125">Supply the values for the following properties.</span></span>

| <span data-ttu-id="40a8b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="40a8b-126">Property</span></span>     | <span data-ttu-id="40a8b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="40a8b-127">Type</span></span>        | <span data-ttu-id="40a8b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="40a8b-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40a8b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="40a8b-129">displayName</span></span>|<span data-ttu-id="40a8b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="40a8b-130">String</span></span>|<span data-ttu-id="40a8b-131">Отображаемого имени publishedResource.</span><span class="sxs-lookup"><span data-stu-id="40a8b-131">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="40a8b-132">resourceName</span><span class="sxs-lookup"><span data-stu-id="40a8b-132">resourceName</span></span>|<span data-ttu-id="40a8b-133">String</span><span class="sxs-lookup"><span data-stu-id="40a8b-133">String</span></span>|<span data-ttu-id="40a8b-134">Имя publishedResource.</span><span class="sxs-lookup"><span data-stu-id="40a8b-134">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="40a8b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40a8b-135">Response</span></span>

<span data-ttu-id="40a8b-136">В случае успеха этот метод возвращает код отклика и `201 Created` [объект publishedResource](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40a8b-136">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40a8b-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="40a8b-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40a8b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="40a8b-138">Request</span></span>

<span data-ttu-id="40a8b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40a8b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40a8b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="40a8b-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="40a8b-141">C#</span><span class="sxs-lookup"><span data-stu-id="40a8b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40a8b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40a8b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40a8b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40a8b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40a8b-144">Java</span><span class="sxs-lookup"><span data-stu-id="40a8b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40a8b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="40a8b-145">Response</span></span>

<span data-ttu-id="40a8b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40a8b-146">The following is an example of the response.</span></span>

> <span data-ttu-id="40a8b-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40a8b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



