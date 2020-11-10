---
title: Create Пермиссионгранткондитионсет в исключении коллекции Пермиссионгрантполици
description: Добавьте условия, при которых событие предоставления разрешений исключается в политике предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 39fcd797f61be5bf8468edc2a5153d08b29f32c5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969302"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="ec217-103">Create Пермиссионгранткондитионсет в исключении коллекции Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="ec217-103">Create permissionGrantConditionSet in excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="ec217-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec217-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec217-105">Добавьте условия, при которых событие предоставления разрешений *исключается* в политике предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="ec217-105">Add conditions under which a permission grant event is *excluded* in a permission grant policy.</span></span> <span data-ttu-id="ec217-106">Для этого необходимо добавить [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в коллекцию **исключений** объекта  [пермиссионгрантполици](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ec217-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **excludes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec217-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec217-107">Permissions</span></span>

<span data-ttu-id="ec217-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec217-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec217-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec217-110">Permission type</span></span>      | <span data-ttu-id="ec217-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec217-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec217-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec217-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec217-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ec217-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="ec217-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec217-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec217-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec217-115">Not supported.</span></span>    |
|<span data-ttu-id="ec217-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ec217-116">Application</span></span> | <span data-ttu-id="ec217-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ec217-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec217-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec217-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a><span data-ttu-id="ec217-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec217-119">Request headers</span></span>

| <span data-ttu-id="ec217-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec217-120">Name</span></span>       | <span data-ttu-id="ec217-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec217-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ec217-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec217-122">Authorization</span></span> | <span data-ttu-id="ec217-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec217-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec217-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec217-125">Content-type</span></span> | <span data-ttu-id="ec217-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec217-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec217-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec217-128">Request body</span></span>

<span data-ttu-id="ec217-129">В тексте запроса добавьте представление объекта [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec217-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec217-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec217-130">Response</span></span>

<span data-ttu-id="ec217-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec217-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec217-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec217-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec217-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec217-133">Request</span></span>

<span data-ttu-id="ec217-134">В этом примере *все* делегированные разрешения для Microsoft Graph ( **AppID** 00000003-0000-0000-C000-000000000000) исключаются из политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="ec217-134">In this example, *all* delegated permissions for Microsoft Graph ( **appId** 00000003-0000-0000-c000-000000000000) are excluded from the permission grant policy.</span></span>


# <a name="http"></a>[<span data-ttu-id="ec217-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec217-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_excludes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes
Content-Type: application/json

{
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="ec217-136">C#</span><span class="sxs-lookup"><span data-stu-id="ec217-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec217-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec217-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec217-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec217-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec217-139">Java</span><span class="sxs-lookup"><span data-stu-id="ec217-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-create-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec217-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec217-140">Response</span></span>

<span data-ttu-id="ec217-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec217-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ec217-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec217-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "9a532f49-e646-405d-8c7c-d4c8e8a4d294",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
