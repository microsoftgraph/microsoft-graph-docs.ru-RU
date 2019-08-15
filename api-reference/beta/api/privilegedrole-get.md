---
title: Получение privilegedRole
description: 'Получение свойств и связей объекта Привилежедроле. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a366130529de2c06273f34e8fc336c7ad433a8f8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412819"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="3d83b-103">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3d83b-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d83b-104">Получение свойств и связей объекта [привилежедроле](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="3d83b-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3d83b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d83b-105">Permissions</span></span>
<span data-ttu-id="3d83b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d83b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3d83b-108">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="3d83b-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="3d83b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d83b-109">Permission type</span></span>      | <span data-ttu-id="3d83b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d83b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d83b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d83b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d83b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d83b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d83b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d83b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d83b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d83b-114">Not supported.</span></span>    |
|<span data-ttu-id="3d83b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d83b-115">Application</span></span> | <span data-ttu-id="3d83b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d83b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d83b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d83b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d83b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d83b-118">Optional query parameters</span></span>
<span data-ttu-id="3d83b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3d83b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d83b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d83b-120">Request headers</span></span>
| <span data-ttu-id="3d83b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3d83b-121">Name</span></span>      |<span data-ttu-id="3d83b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d83b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d83b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d83b-123">Authorization</span></span>  | <span data-ttu-id="3d83b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d83b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d83b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d83b-126">Request body</span></span>
<span data-ttu-id="3d83b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d83b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d83b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d83b-128">Response</span></span>

<span data-ttu-id="3d83b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедроле](../resources/privilegedrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d83b-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="3d83b-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="3d83b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3d83b-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="3d83b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="3d83b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3d83b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d83b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d83b-133">Request</span></span>
<span data-ttu-id="3d83b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d83b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3d83b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d83b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d83b-136">C#</span><span class="sxs-lookup"><span data-stu-id="3d83b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d83b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d83b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d83b-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3d83b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3d83b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d83b-139">Response</span></span>
<span data-ttu-id="3d83b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d83b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
