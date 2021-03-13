---
title: Тег обновления
description: Обновление свойств объекта тегов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ee8d46d92b7f5e29a4612d3399028dacc36ad6fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776398"
---
# <a name="update-tag"></a><span data-ttu-id="0739e-103">Тег обновления</span><span class="sxs-lookup"><span data-stu-id="0739e-103">Update tag</span></span>

<span data-ttu-id="0739e-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0739e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0739e-105">Обновление свойств объекта [тегов.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="0739e-105">Update the properties of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0739e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0739e-106">Permissions</span></span>

<span data-ttu-id="0739e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0739e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0739e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0739e-109">Permission type</span></span>|<span data-ttu-id="0739e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0739e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0739e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0739e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0739e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0739e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0739e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0739e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0739e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0739e-114">Not supported.</span></span>|
|<span data-ttu-id="0739e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0739e-115">Application</span></span>|<span data-ttu-id="0739e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0739e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0739e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0739e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="request-headers"></a><span data-ttu-id="0739e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0739e-118">Request headers</span></span>

|<span data-ttu-id="0739e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0739e-119">Name</span></span>|<span data-ttu-id="0739e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0739e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0739e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0739e-121">Authorization</span></span>|<span data-ttu-id="0739e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0739e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0739e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0739e-124">Content-Type</span></span>|<span data-ttu-id="0739e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0739e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0739e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0739e-127">Request body</span></span>

<span data-ttu-id="0739e-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0739e-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0739e-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0739e-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0739e-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0739e-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="0739e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0739e-131">Property</span></span>|<span data-ttu-id="0739e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0739e-132">Type</span></span>|<span data-ttu-id="0739e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0739e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0739e-134">description</span><span class="sxs-lookup"><span data-stu-id="0739e-134">description</span></span>|<span data-ttu-id="0739e-135">String</span><span class="sxs-lookup"><span data-stu-id="0739e-135">String</span></span>|<span data-ttu-id="0739e-136">Описание тега.</span><span class="sxs-lookup"><span data-stu-id="0739e-136">The description for the tag.</span></span>|
|<span data-ttu-id="0739e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0739e-137">displayName</span></span>|<span data-ttu-id="0739e-138">String</span><span class="sxs-lookup"><span data-stu-id="0739e-138">String</span></span>|<span data-ttu-id="0739e-139">Отображение имени тега.</span><span class="sxs-lookup"><span data-stu-id="0739e-139">Display name of the tag.</span></span>|

## <a name="response"></a><span data-ttu-id="0739e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0739e-140">Response</span></span>

<span data-ttu-id="0739e-141">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0739e-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0739e-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="0739e-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0739e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0739e-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0739e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0739e-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tag"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
Content-Type: application/json
Content-length: 210

{
  "description":"This is an updated description."
}
```
# <a name="c"></a>[<span data-ttu-id="0739e-145">C#</span><span class="sxs-lookup"><span data-stu-id="0739e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0739e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0739e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0739e-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0739e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0739e-148">Java</span><span class="sxs-lookup"><span data-stu-id="0739e-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0739e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0739e-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
