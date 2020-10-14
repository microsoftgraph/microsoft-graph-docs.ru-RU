---
title: Обновление Пермиссионгрантполици
description: Обновление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 1bc18442c7c6e1713ca1ed863a631519aeadef00
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459620"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="4c881-103">Обновление Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="4c881-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="4c881-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c881-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c881-105">Обновление свойств объекта  [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4c881-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c881-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c881-106">Permissions</span></span>

<span data-ttu-id="4c881-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c881-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c881-109">Permission type</span></span>                        | <span data-ttu-id="4c881-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c881-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c881-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c881-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c881-112">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="4c881-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="4c881-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c881-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c881-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c881-114">Not supported.</span></span> |
| <span data-ttu-id="4c881-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c881-115">Application</span></span>                            | <span data-ttu-id="4c881-116">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="4c881-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c881-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c881-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c881-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c881-118">Request headers</span></span>

| <span data-ttu-id="4c881-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4c881-119">Name</span></span>           | <span data-ttu-id="4c881-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4c881-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="4c881-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c881-121">Authorization</span></span>  | <span data-ttu-id="4c881-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c881-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c881-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c881-124">Request body</span></span>

<span data-ttu-id="4c881-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4c881-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4c881-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4c881-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c881-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4c881-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c881-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c881-128">Property</span></span>     | <span data-ttu-id="4c881-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4c881-129">Type</span></span> |<span data-ttu-id="4c881-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4c881-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c881-131">displayName</span><span class="sxs-lookup"><span data-stu-id="4c881-131">displayName</span></span> | <span data-ttu-id="4c881-132">String</span><span class="sxs-lookup"><span data-stu-id="4c881-132">String</span></span> |<span data-ttu-id="4c881-133">Отображаемое имя политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="4c881-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="4c881-134">description</span><span class="sxs-lookup"><span data-stu-id="4c881-134">description</span></span> |<span data-ttu-id="4c881-135">String</span><span class="sxs-lookup"><span data-stu-id="4c881-135">String</span></span>| <span data-ttu-id="4c881-136">Описание политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="4c881-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="4c881-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c881-137">Response</span></span>

<span data-ttu-id="4c881-138">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c881-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c881-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c881-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c881-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c881-140">Request</span></span>

<span data-ttu-id="4c881-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c881-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c881-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c881-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```
# <a name="c"></a>[<span data-ttu-id="4c881-143">C#</span><span class="sxs-lookup"><span data-stu-id="4c881-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c881-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c881-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c881-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c881-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c881-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c881-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
