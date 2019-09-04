---
title: Получение Унифиедролеассигнмент
description: Получение свойств и связей объекта Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8861b1973c270d025786b44ca7a7696aa63fd881
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722113"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="d4c80-103">Получение Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="d4c80-103">Get unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4c80-104">Получение свойств и связей объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c80-104">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4c80-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c80-105">Permissions</span></span>

<span data-ttu-id="d4c80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c80-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c80-108">Permission type</span></span>      | <span data-ttu-id="d4c80-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4c80-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4c80-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4c80-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4c80-111">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d4c80-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4c80-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4c80-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4c80-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c80-113">Not supported.</span></span>    |
|<span data-ttu-id="d4c80-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4c80-114">Application</span></span> | <span data-ttu-id="d4c80-115">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d4c80-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4c80-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4c80-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4c80-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4c80-117">Optional query parameters</span></span>

<span data-ttu-id="d4c80-118">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d4c80-118">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="d4c80-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d4c80-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4c80-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4c80-120">Request headers</span></span>

| <span data-ttu-id="d4c80-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d4c80-121">Name</span></span>      |<span data-ttu-id="d4c80-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d4c80-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4c80-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4c80-123">Authorization</span></span> | <span data-ttu-id="d4c80-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d4c80-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4c80-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4c80-125">Request body</span></span>

<span data-ttu-id="d4c80-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4c80-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4c80-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4c80-127">Response</span></span>

<span data-ttu-id="d4c80-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4c80-128">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c80-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d4c80-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4c80-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4c80-130">Request</span></span>

<span data-ttu-id="d4c80-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4c80-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4c80-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4c80-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4c80-133">C#</span><span class="sxs-lookup"><span data-stu-id="d4c80-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4c80-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4c80-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4c80-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d4c80-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4c80-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4c80-136">Response</span></span>

<span data-ttu-id="d4c80-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4c80-137">The following is an example of the response.</span></span>

> <span data-ttu-id="d4c80-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4c80-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "resourceScope": "/",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
