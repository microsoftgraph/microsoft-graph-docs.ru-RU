---
title: Список Делегатедпермиссионклассификатионс коллекции servicePrincipal
description: Получение списка классификаций, предоставленных делегированным разрешениям, предоставленным субъектом-службой API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 2ff031cbafed3d2239435ed102df6d05d0b63cec
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980579"
---
# <a name="list-delegatedpermissionclassifications-collection-of-serviceprincipal"></a><span data-ttu-id="642e9-103">Список Делегатедпермиссионклассификатионс коллекции servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="642e9-103">List delegatedPermissionClassifications collection of servicePrincipal</span></span>

<span data-ttu-id="642e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642e9-105">Получение списка [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) , настроенных в настоящее время для делегированных разрешений, предоставляемых API.</span><span class="sxs-lookup"><span data-stu-id="642e9-105">Retrieve the list of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) currently configured for the delegated permissions exposed by an API.</span></span>

## <a name="permissions"></a><span data-ttu-id="642e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="642e9-106">Permissions</span></span>

<span data-ttu-id="642e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="642e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="642e9-109">Permission type</span></span>      | <span data-ttu-id="642e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="642e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="642e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="642e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="642e9-112">Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="642e9-112">Application.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="642e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="642e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="642e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="642e9-114">Not supported.</span></span>    |
|<span data-ttu-id="642e9-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="642e9-115">Application</span></span> | <span data-ttu-id="642e9-116">Application. Read. Овнедби, Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="642e9-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="642e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="642e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="642e9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="642e9-118">Optional query parameters</span></span>

<span data-ttu-id="642e9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="642e9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="642e9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="642e9-120">Request headers</span></span>

| <span data-ttu-id="642e9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="642e9-121">Name</span></span>           | <span data-ttu-id="642e9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="642e9-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="642e9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="642e9-123">Authorization</span></span>  | <span data-ttu-id="642e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="642e9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="642e9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="642e9-126">Request body</span></span>

<span data-ttu-id="642e9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="642e9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="642e9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="642e9-128">Response</span></span>

<span data-ttu-id="642e9-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [делегатедпермиссионклассификатион](../resources/delegatedpermissionclassification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="642e9-129">If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642e9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="642e9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="642e9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="642e9-131">Request</span></span>

<span data-ttu-id="642e9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="642e9-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="642e9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="642e9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_delegatedpermissionclassification"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications
```
# <a name="c"></a>[<span data-ttu-id="642e9-134">C#</span><span class="sxs-lookup"><span data-stu-id="642e9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="642e9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="642e9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="642e9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="642e9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="642e9-137">Java</span><span class="sxs-lookup"><span data-stu-id="642e9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="642e9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="642e9-138">Response</span></span>

<span data-ttu-id="642e9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="642e9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="642e9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="642e9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id": "2G3-4TG6YU2J54hjnaRoPQE",
        "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
        "permissionName": "User.Read",
        "classification": "low"
    }
  ]
}
```
