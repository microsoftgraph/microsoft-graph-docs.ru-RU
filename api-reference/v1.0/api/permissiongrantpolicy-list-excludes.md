---
title: List исключает коллекцию Пермиссионгрантполици
description: Получение списка наборов условий, описывающих условия, при которых событие предоставления разрешений исключается в политике предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 340b371ca1ffbcdb5e39b12c17cc34a0fe8ef96e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523287"
---
# <a name="list-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="34e2b-103">List исключает коллекцию Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="34e2b-103">List excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="34e2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34e2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34e2b-105">Получение наборов условий, *исключаемых* в [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="34e2b-105">Retrieve the condition sets which are *excluded* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34e2b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34e2b-106">Permissions</span></span>

<span data-ttu-id="34e2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34e2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34e2b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34e2b-109">Permission type</span></span>      | <span data-ttu-id="34e2b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34e2b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34e2b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34e2b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34e2b-112">Policy. Read. Пермиссионгрант, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="34e2b-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="34e2b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34e2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34e2b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34e2b-114">Not supported.</span></span>    |
|<span data-ttu-id="34e2b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="34e2b-115">Application</span></span> | <span data-ttu-id="34e2b-116">Policy. Read. Пермиссионгрант, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="34e2b-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34e2b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34e2b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34e2b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34e2b-118">Optional query parameters</span></span>

<span data-ttu-id="34e2b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="34e2b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34e2b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34e2b-120">Request headers</span></span>

| <span data-ttu-id="34e2b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="34e2b-121">Name</span></span>           | <span data-ttu-id="34e2b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="34e2b-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="34e2b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34e2b-123">Authorization</span></span>  | <span data-ttu-id="34e2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34e2b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34e2b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34e2b-126">Request body</span></span>

<span data-ttu-id="34e2b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34e2b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34e2b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="34e2b-128">Response</span></span>

<span data-ttu-id="34e2b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34e2b-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34e2b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="34e2b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="34e2b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="34e2b-131">Request</span></span>

<span data-ttu-id="34e2b-132">Ниже приведен пример запроса на получение наборов условий, **исключаемых** из встроенной политики предоставления разрешений `microsoft-application-admin` .</span><span class="sxs-lookup"><span data-stu-id="34e2b-132">The following is an example of the request to retrieve the **excludes** condition sets of the built-on permission grant policy `microsoft-application-admin`.</span></span> <span data-ttu-id="34e2b-133">Эта политика предоставления разрешений включает все делегированные разрешения, а также все разрешения приложений, кроме разрешений приложений для Microsoft Graph и разрешений приложений для Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="34e2b-133">This permission grant policy includes all delegated permissions, and all application permissions excluding application permissions for Microsoft Graph and application permissions for Azure AD Graph.</span></span>



# <a name="http"></a>[<span data-ttu-id="34e2b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="34e2b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_excludes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/excludes
```
# <a name="c"></a>[<span data-ttu-id="34e2b-135">C#</span><span class="sxs-lookup"><span data-stu-id="34e2b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34e2b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34e2b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34e2b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34e2b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34e2b-138">Java</span><span class="sxs-lookup"><span data-stu-id="34e2b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34e2b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="34e2b-139">Response</span></span>

<span data-ttu-id="34e2b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34e2b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="34e2b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34e2b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c85b029f-4abf-47d8-ae61-d2a38299033a",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000003-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "2a1fbb36-9d9a-42d8-8804-de2aa45aca80",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000002-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
