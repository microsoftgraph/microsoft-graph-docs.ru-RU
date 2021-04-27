---
title: Создание publishedResource
description: Создание нового **объекта publishedResource.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0cf0b586010b6d68a36f4d710bc24f0035ecafa7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055164"
---
# <a name="create-publishedresource"></a><span data-ttu-id="0a735-103">Создание publishedResource</span><span class="sxs-lookup"><span data-stu-id="0a735-103">Create publishedResource</span></span>

<span data-ttu-id="0a735-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a735-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a735-105">Создание нового [объекта publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="0a735-105">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a735-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a735-106">Permissions</span></span>

<span data-ttu-id="0a735-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a735-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a735-109">Permission type</span></span>                        | <span data-ttu-id="0a735-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a735-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a735-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a735-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a735-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a735-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="0a735-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a735-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a735-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a735-114">Not supported.</span></span> |
| <span data-ttu-id="0a735-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a735-115">Application</span></span>                            | <span data-ttu-id="0a735-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a735-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a735-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a735-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="0a735-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a735-118">Request headers</span></span>

| <span data-ttu-id="0a735-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0a735-119">Name</span></span>      |<span data-ttu-id="0a735-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0a735-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a735-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a735-121">Authorization</span></span> | <span data-ttu-id="0a735-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0a735-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a735-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a735-123">Request body</span></span>

<span data-ttu-id="0a735-124">В теле запроса поставляем представление JSON объекта [publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="0a735-124">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="0a735-125">Поставляем значения для следующих свойств.</span><span class="sxs-lookup"><span data-stu-id="0a735-125">Supply the values for the following properties.</span></span>

| <span data-ttu-id="0a735-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a735-126">Property</span></span>     | <span data-ttu-id="0a735-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0a735-127">Type</span></span>        | <span data-ttu-id="0a735-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0a735-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a735-129">displayName</span><span class="sxs-lookup"><span data-stu-id="0a735-129">displayName</span></span>|<span data-ttu-id="0a735-130">String</span><span class="sxs-lookup"><span data-stu-id="0a735-130">String</span></span>|<span data-ttu-id="0a735-131">Отображение имени опубликованногоРесурса.</span><span class="sxs-lookup"><span data-stu-id="0a735-131">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="0a735-132">resourceName</span><span class="sxs-lookup"><span data-stu-id="0a735-132">resourceName</span></span>|<span data-ttu-id="0a735-133">String</span><span class="sxs-lookup"><span data-stu-id="0a735-133">String</span></span>|<span data-ttu-id="0a735-134">Имя опубликованногоResource.</span><span class="sxs-lookup"><span data-stu-id="0a735-134">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="0a735-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a735-135">Response</span></span>

<span data-ttu-id="0a735-136">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект publishedResource](../resources/publishedresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a735-136">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a735-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a735-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a735-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a735-138">Request</span></span>

<span data-ttu-id="0a735-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a735-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a735-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a735-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0a735-141">C#</span><span class="sxs-lookup"><span data-stu-id="0a735-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a735-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a735-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a735-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a735-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a735-144">Java</span><span class="sxs-lookup"><span data-stu-id="0a735-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a735-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a735-145">Response</span></span>

<span data-ttu-id="0a735-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0a735-146">The following is an example of the response.</span></span>

> <span data-ttu-id="0a735-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a735-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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



