---
title: Список Привилежедролес
description: Получение списка объектов Привилежедроле.
localization_priority: Normal
ms.openlocfilehash: e1a4f94176fb0cbed9ac585605c5e15b02f16942
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875825"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="4b0aa-103">Список Привилежедролес</span><span class="sxs-lookup"><span data-stu-id="4b0aa-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b0aa-104">Получение списка объектов [привилежедроле](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="4b0aa-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="4b0aa-105">Чтобы отфильтровать результаты запроса, используйте стандартные выражения OData ``$filter`` в URI.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b0aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b0aa-106">Permissions</span></span>
<span data-ttu-id="4b0aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b0aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4b0aa-109">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="4b0aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b0aa-110">Permission type</span></span>      | <span data-ttu-id="4b0aa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b0aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b0aa-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b0aa-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b0aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b0aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-115">Not supported.</span></span>    |
|<span data-ttu-id="4b0aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b0aa-116">Application</span></span> | <span data-ttu-id="4b0aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b0aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b0aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b0aa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b0aa-119">Optional query parameters</span></span>
<span data-ttu-id="4b0aa-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b0aa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b0aa-121">Request headers</span></span>
| <span data-ttu-id="4b0aa-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4b0aa-122">Name</span></span>      |<span data-ttu-id="4b0aa-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4b0aa-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b0aa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b0aa-124">Authorization</span></span>  | <span data-ttu-id="4b0aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b0aa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b0aa-127">Request body</span></span>
<span data-ttu-id="4b0aa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b0aa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0aa-129">Response</span></span>

<span data-ttu-id="4b0aa-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедроле](../resources/privilegedrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="4b0aa-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4b0aa-132">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4b0aa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4b0aa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b0aa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b0aa-134">Request</span></span>
<span data-ttu-id="4b0aa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4b0aa-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0aa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b0aa-137">C#</span><span class="sxs-lookup"><span data-stu-id="4b0aa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b0aa-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="4b0aa-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b0aa-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4b0aa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4b0aa-140">Java</span><span class="sxs-lookup"><span data-stu-id="4b0aa-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4b0aa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0aa-141">Response</span></span>
<span data-ttu-id="4b0aa-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b0aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
