---
title: Обновление permissionGrantPolicy
description: Обновление объекта permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 6e40a6361ec5f72c936f4b8151e001308e48be2b
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787157"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="520c1-103">Обновление permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="520c1-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="520c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="520c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="520c1-105">Обновление свойств  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520c1-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="520c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="520c1-106">Permissions</span></span>

<span data-ttu-id="520c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="520c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="520c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="520c1-109">Permission type</span></span>                        | <span data-ttu-id="520c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="520c1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="520c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="520c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="520c1-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="520c1-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="520c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="520c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="520c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="520c1-114">Not supported.</span></span> |
| <span data-ttu-id="520c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="520c1-115">Application</span></span>                            | <span data-ttu-id="520c1-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="520c1-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="520c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="520c1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="520c1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="520c1-118">Request headers</span></span>

| <span data-ttu-id="520c1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="520c1-119">Name</span></span>           | <span data-ttu-id="520c1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="520c1-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="520c1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="520c1-121">Authorization</span></span>  | <span data-ttu-id="520c1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="520c1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="520c1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="520c1-124">Request body</span></span>

<span data-ttu-id="520c1-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="520c1-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="520c1-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="520c1-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="520c1-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="520c1-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="520c1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="520c1-128">Property</span></span>     | <span data-ttu-id="520c1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="520c1-129">Type</span></span> |<span data-ttu-id="520c1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="520c1-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="520c1-131">displayName</span><span class="sxs-lookup"><span data-stu-id="520c1-131">displayName</span></span> | <span data-ttu-id="520c1-132">String</span><span class="sxs-lookup"><span data-stu-id="520c1-132">String</span></span> |<span data-ttu-id="520c1-133">Отображаемое имя политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="520c1-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="520c1-134">description</span><span class="sxs-lookup"><span data-stu-id="520c1-134">description</span></span> |<span data-ttu-id="520c1-135">String</span><span class="sxs-lookup"><span data-stu-id="520c1-135">String</span></span>| <span data-ttu-id="520c1-136">Описание политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="520c1-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="520c1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="520c1-137">Response</span></span>

<span data-ttu-id="520c1-138">В случае успешной работы этот метод возвращает код ответа и ничего не возвращает `204 No Content` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="520c1-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="520c1-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="520c1-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="520c1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="520c1-140">Request</span></span>

<span data-ttu-id="520c1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="520c1-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="520c1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="520c1-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```
# <a name="c"></a>[<span data-ttu-id="520c1-143">C#</span><span class="sxs-lookup"><span data-stu-id="520c1-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="520c1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="520c1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="520c1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="520c1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="520c1-146">Java</span><span class="sxs-lookup"><span data-stu-id="520c1-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="520c1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="520c1-147">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
