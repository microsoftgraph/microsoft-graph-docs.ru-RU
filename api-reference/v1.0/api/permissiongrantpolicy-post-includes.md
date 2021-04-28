---
title: Создание permissionGrantConditionSet включает коллекцию разрешенийGrantPolicy
description: Добавьте условия, при которых событие предоставления разрешений включено в политику предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 79b70637beaff1d90892ab42fc58286d1135b4ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051272"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="298e9-103">Создание permissionGrantConditionSet включает коллекцию разрешенийGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="298e9-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="298e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="298e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="298e9-105">Добавьте условия, при которых событие предоставления разрешений *включено* в политику предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="298e9-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="298e9-106">Это необходимо, добавив [permissionGrantConditionSet](../resources/permissiongrantconditionset.md)  в коллекцию [разрешенийGrantPolicy.](../resources/permissionGrantPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="298e9-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="298e9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="298e9-107">Permissions</span></span>

<span data-ttu-id="298e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="298e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="298e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="298e9-110">Permission type</span></span>      | <span data-ttu-id="298e9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="298e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="298e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="298e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="298e9-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="298e9-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="298e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="298e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="298e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="298e9-115">Not supported.</span></span>    |
|<span data-ttu-id="298e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="298e9-116">Application</span></span> | <span data-ttu-id="298e9-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="298e9-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="298e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="298e9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="298e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="298e9-119">Request headers</span></span>

| <span data-ttu-id="298e9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="298e9-120">Name</span></span>       | <span data-ttu-id="298e9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="298e9-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="298e9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="298e9-122">Authorization</span></span> | <span data-ttu-id="298e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="298e9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="298e9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="298e9-125">Content-type</span></span> | <span data-ttu-id="298e9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="298e9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="298e9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="298e9-128">Request body</span></span>

<span data-ttu-id="298e9-129">В теле запроса необходимо предоставить представление JSON объекта [permissionGrantConditionSet.](../resources/permissiongrantconditionset.md)</span><span class="sxs-lookup"><span data-stu-id="298e9-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="298e9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="298e9-130">Response</span></span>

<span data-ttu-id="298e9-131">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект permissionGrantConditionSet](../resources/permissiongrantconditionset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="298e9-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="298e9-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="298e9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="298e9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="298e9-133">Request</span></span>

<span data-ttu-id="298e9-134">В этом примере *все* делегированные разрешения для клиентских приложений от проверенных издателей включены в политику предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="298e9-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="298e9-135">Так как все остальные условия [из permissionGrantConditionSet](../resources/permissiongrantconditionset.md) были пропущены, они будут принимать значения по умолчанию, которые в каждом случае наиболее все включено.</span><span class="sxs-lookup"><span data-stu-id="298e9-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>


# <a name="http"></a>[<span data-ttu-id="298e9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="298e9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="298e9-137">C#</span><span class="sxs-lookup"><span data-stu-id="298e9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="298e9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="298e9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="298e9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="298e9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="298e9-140">Java</span><span class="sxs-lookup"><span data-stu-id="298e9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-create-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="298e9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="298e9-141">Response</span></span>

<span data-ttu-id="298e9-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="298e9-142">The following is an example of the response.</span></span>

> <span data-ttu-id="298e9-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="298e9-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
