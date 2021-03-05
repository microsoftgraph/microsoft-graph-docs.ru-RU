---
title: Создание permissionGrantConditionSet включает коллекцию разрешенийGrantPolicy
description: Добавьте условия, при которых событие предоставления разрешений включено в политику предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 1300319e2411a7e5e39b7cf9d1fd5ad365a2f363
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448081"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="cdd67-103">Создание permissionGrantConditionSet включает коллекцию разрешенийGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="cdd67-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="cdd67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdd67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdd67-105">Добавьте условия, при которых событие предоставления разрешений *включено* в политику предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="cdd67-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="cdd67-106">Это необходимо, добавив [permissionGrantConditionSet](../resources/permissiongrantconditionset.md)  в коллекцию [разрешенийGrantPolicy.](../resources/permissionGrantPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdd67-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd67-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdd67-107">Permissions</span></span>

<span data-ttu-id="cdd67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd67-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdd67-110">Permission type</span></span>      | <span data-ttu-id="cdd67-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdd67-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd67-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdd67-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd67-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cdd67-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="cdd67-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdd67-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd67-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdd67-115">Not supported.</span></span>    |
|<span data-ttu-id="cdd67-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdd67-116">Application</span></span> | <span data-ttu-id="cdd67-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cdd67-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdd67-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdd67-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="cdd67-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdd67-119">Request headers</span></span>

| <span data-ttu-id="cdd67-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cdd67-120">Name</span></span>       | <span data-ttu-id="cdd67-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cdd67-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cdd67-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdd67-122">Authorization</span></span> | <span data-ttu-id="cdd67-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdd67-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdd67-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdd67-125">Content-type</span></span> | <span data-ttu-id="cdd67-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdd67-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdd67-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdd67-128">Request body</span></span>

<span data-ttu-id="cdd67-129">В теле запроса необходимо предоставить представление JSON объекта [permissionGrantConditionSet.](../resources/permissiongrantconditionset.md)</span><span class="sxs-lookup"><span data-stu-id="cdd67-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cdd67-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdd67-130">Response</span></span>

<span data-ttu-id="cdd67-131">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект permissionGrantConditionSet](../resources/permissiongrantconditionset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cdd67-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdd67-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="cdd67-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdd67-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdd67-133">Request</span></span>

<span data-ttu-id="cdd67-134">В этом примере *все* делегированные разрешения для клиентских приложений от проверенных издателей включены в политику предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="cdd67-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="cdd67-135">Так как все остальные условия [из permissionGrantConditionSet](../resources/permissiongrantconditionset.md) были пропущены, они будут принимать значения по умолчанию, которые в каждом случае наиболее все включено.</span><span class="sxs-lookup"><span data-stu-id="cdd67-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdd67-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd67-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cdd67-137">C#</span><span class="sxs-lookup"><span data-stu-id="cdd67-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdd67-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd67-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdd67-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdd67-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdd67-140">Java</span><span class="sxs-lookup"><span data-stu-id="cdd67-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-create-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cdd67-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdd67-141">Response</span></span>

<span data-ttu-id="cdd67-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdd67-142">The following is an example of the response.</span></span>

> <span data-ttu-id="cdd67-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdd67-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
