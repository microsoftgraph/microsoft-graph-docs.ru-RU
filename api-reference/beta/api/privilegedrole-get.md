---
title: Получение privilegedRole
description: 'Получение свойств и связей объекта Привилежедроле. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36d9fa5a4e5d85f6617f223523770fe1e25698b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455381"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="91895-103">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="91895-103">Get privilegedRole</span></span>

<span data-ttu-id="91895-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91895-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91895-105">Получение свойств и связей объекта [привилежедроле](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="91895-105">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="91895-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91895-106">Permissions</span></span>
<span data-ttu-id="91895-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="91895-109">Запрашивающая сторона должна иметь одну из следующих ролей: _привилегированный администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="91895-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="91895-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91895-110">Permission type</span></span>      | <span data-ttu-id="91895-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91895-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91895-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91895-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91895-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91895-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91895-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91895-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91895-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91895-115">Not supported.</span></span>    |
|<span data-ttu-id="91895-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91895-116">Application</span></span> | <span data-ttu-id="91895-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91895-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91895-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91895-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91895-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91895-119">Optional query parameters</span></span>
<span data-ttu-id="91895-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91895-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91895-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91895-121">Request headers</span></span>
| <span data-ttu-id="91895-122">Имя</span><span class="sxs-lookup"><span data-stu-id="91895-122">Name</span></span>      |<span data-ttu-id="91895-123">Описание</span><span class="sxs-lookup"><span data-stu-id="91895-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91895-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91895-124">Authorization</span></span>  | <span data-ttu-id="91895-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91895-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91895-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91895-127">Request body</span></span>
<span data-ttu-id="91895-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91895-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91895-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="91895-129">Response</span></span>

<span data-ttu-id="91895-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедроле](../resources/privilegedrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91895-130">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="91895-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="91895-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="91895-132">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="91895-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="91895-133">Пример</span><span class="sxs-lookup"><span data-stu-id="91895-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91895-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="91895-134">Request</span></span>
<span data-ttu-id="91895-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91895-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91895-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="91895-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="91895-137">C#</span><span class="sxs-lookup"><span data-stu-id="91895-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91895-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91895-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91895-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91895-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91895-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="91895-140">Response</span></span>
<span data-ttu-id="91895-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91895-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
