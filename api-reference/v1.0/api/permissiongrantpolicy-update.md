---
title: Обновление Пермиссионгрантполици
description: Обновление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 403968aa3ee4cde189c5b58331cd4dc90dd3cabd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524089"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="515a6-103">Обновление Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="515a6-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="515a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="515a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="515a6-105">Обновление свойств объекта  [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="515a6-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="515a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="515a6-106">Permissions</span></span>

<span data-ttu-id="515a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="515a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="515a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="515a6-109">Permission type</span></span>                        | <span data-ttu-id="515a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="515a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="515a6-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="515a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="515a6-112">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="515a6-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="515a6-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="515a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="515a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="515a6-114">Not supported.</span></span> |
| <span data-ttu-id="515a6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="515a6-115">Application</span></span>                            | <span data-ttu-id="515a6-116">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="515a6-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="515a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="515a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="515a6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="515a6-118">Request headers</span></span>

| <span data-ttu-id="515a6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="515a6-119">Name</span></span>           | <span data-ttu-id="515a6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="515a6-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="515a6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="515a6-121">Authorization</span></span>  | <span data-ttu-id="515a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="515a6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="515a6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="515a6-124">Request body</span></span>

<span data-ttu-id="515a6-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="515a6-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="515a6-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="515a6-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="515a6-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="515a6-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="515a6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="515a6-128">Property</span></span>     | <span data-ttu-id="515a6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="515a6-129">Type</span></span> |<span data-ttu-id="515a6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="515a6-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="515a6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="515a6-131">displayName</span></span> | <span data-ttu-id="515a6-132">String</span><span class="sxs-lookup"><span data-stu-id="515a6-132">String</span></span> |<span data-ttu-id="515a6-133">Отображаемое имя политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="515a6-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="515a6-134">description</span><span class="sxs-lookup"><span data-stu-id="515a6-134">description</span></span> |<span data-ttu-id="515a6-135">String</span><span class="sxs-lookup"><span data-stu-id="515a6-135">String</span></span>| <span data-ttu-id="515a6-136">Описание политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="515a6-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="515a6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="515a6-137">Response</span></span>

<span data-ttu-id="515a6-138">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="515a6-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="515a6-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="515a6-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="515a6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="515a6-140">Request</span></span>

<span data-ttu-id="515a6-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="515a6-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="515a6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="515a6-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="515a6-143">C#</span><span class="sxs-lookup"><span data-stu-id="515a6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="515a6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="515a6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="515a6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="515a6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="515a6-146">Java</span><span class="sxs-lookup"><span data-stu-id="515a6-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="515a6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="515a6-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
