---
title: Получение privilegedRoleAssignment
description: Получение свойств и связей объекта Привилежедролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: b21ec9ca5fe189f99193419ab1751893d293906d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875756"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="b90fa-103">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b90fa-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b90fa-104">Получение свойств и связей объекта Привилежедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="b90fa-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b90fa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b90fa-105">Permissions</span></span>
<span data-ttu-id="b90fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b90fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b90fa-108">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="b90fa-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="b90fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b90fa-109">Permission type</span></span>      | <span data-ttu-id="b90fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b90fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b90fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b90fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b90fa-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b90fa-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b90fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b90fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b90fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90fa-114">Not supported.</span></span>    |
|<span data-ttu-id="b90fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b90fa-115">Application</span></span> | <span data-ttu-id="b90fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b90fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b90fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b90fa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b90fa-118">Optional query parameters</span></span>
<span data-ttu-id="b90fa-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b90fa-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b90fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b90fa-120">Request headers</span></span>
| <span data-ttu-id="b90fa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b90fa-121">Name</span></span>      |<span data-ttu-id="b90fa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b90fa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b90fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b90fa-123">Authorization</span></span>  | <span data-ttu-id="b90fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b90fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b90fa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b90fa-126">Request body</span></span>
<span data-ttu-id="b90fa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b90fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b90fa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b90fa-128">Response</span></span>

<span data-ttu-id="b90fa-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b90fa-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="b90fa-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="b90fa-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b90fa-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="b90fa-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b90fa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b90fa-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b90fa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b90fa-133">Request</span></span>
<span data-ttu-id="b90fa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b90fa-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b90fa-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b90fa-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b90fa-136">C#</span><span class="sxs-lookup"><span data-stu-id="b90fa-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b90fa-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b90fa-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b90fa-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b90fa-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b90fa-139">Java</span><span class="sxs-lookup"><span data-stu-id="b90fa-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b90fa-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b90fa-140">Response</span></span>
<span data-ttu-id="b90fa-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b90fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
