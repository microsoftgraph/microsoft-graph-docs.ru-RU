---
title: Create Пермиссионгранткондитионсет в исключении коллекции Пермиссионгрантполици
description: Добавьте условия, при которых событие предоставления разрешений исключается в политике предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4fc5f04ebfcb4c07fb8eef894445b2fa9164ed6c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458724"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="6d0fe-103">Create Пермиссионгранткондитионсет в исключении коллекции Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="6d0fe-103">Create permissionGrantConditionSet in excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="6d0fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d0fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d0fe-105">Добавьте условия, при которых событие предоставления разрешений *исключается* в политике предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-105">Add conditions under which a permission grant event is *excluded* in a permission grant policy.</span></span> <span data-ttu-id="6d0fe-106">Для этого необходимо добавить [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в коллекцию **исключений** объекта  [пермиссионгрантполици](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d0fe-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **excludes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d0fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d0fe-107">Permissions</span></span>

<span data-ttu-id="6d0fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d0fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d0fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d0fe-110">Permission type</span></span>      | <span data-ttu-id="6d0fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d0fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d0fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d0fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d0fe-113">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="6d0fe-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="6d0fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d0fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d0fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-115">Not supported.</span></span>    |
|<span data-ttu-id="6d0fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d0fe-116">Application</span></span> | <span data-ttu-id="6d0fe-117">Policy. ReadWrite. Пермиссионгрант</span><span class="sxs-lookup"><span data-stu-id="6d0fe-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d0fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d0fe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a><span data-ttu-id="6d0fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d0fe-119">Request headers</span></span>

| <span data-ttu-id="6d0fe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6d0fe-120">Name</span></span>       | <span data-ttu-id="6d0fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6d0fe-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="6d0fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d0fe-122">Authorization</span></span> | <span data-ttu-id="6d0fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d0fe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d0fe-125">Content-type</span></span> | <span data-ttu-id="6d0fe-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d0fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d0fe-128">Request body</span></span>

<span data-ttu-id="6d0fe-129">В тексте запроса добавьте представление объекта [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6d0fe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d0fe-130">Response</span></span>

<span data-ttu-id="6d0fe-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d0fe-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d0fe-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d0fe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d0fe-133">Request</span></span>

<span data-ttu-id="6d0fe-134">В этом примере *все* делегированные разрешения для Microsoft Graph (**AppID** 00000003-0000-0000-C000-000000000000) исключаются из политики предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-134">In this example, *all* delegated permissions for Microsoft Graph (**appId** 00000003-0000-0000-c000-000000000000) are excluded from the permission grant policy.</span></span>


# <a name="http"></a>[<span data-ttu-id="6d0fe-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d0fe-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6d0fe-136">C#</span><span class="sxs-lookup"><span data-stu-id="6d0fe-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d0fe-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d0fe-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d0fe-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d0fe-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d0fe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d0fe-139">Response</span></span>

<span data-ttu-id="6d0fe-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6d0fe-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d0fe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
