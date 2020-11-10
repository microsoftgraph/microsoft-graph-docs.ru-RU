---
title: Список Привилежедролес
description: Получение списка объектов Привилежедроле.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 5bf6ba52e0c3c3cc2f729e86cb3a47de18de7f64
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970423"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="dfaf9-103">Список Привилежедролес</span><span class="sxs-lookup"><span data-stu-id="dfaf9-103">List privilegedRoles</span></span>

<span data-ttu-id="dfaf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfaf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfaf9-105">Получение списка объектов [привилежедроле](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="dfaf9-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="dfaf9-106">Чтобы отфильтровать результаты запроса, используйте стандартные выражения OData ``$filter`` в URI.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfaf9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfaf9-107">Permissions</span></span>
<span data-ttu-id="dfaf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfaf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dfaf9-110">Запрашивающая сторона должна иметь одну из следующих ролей: _привилегированный администратор ролей_ , _глобальный администратор_ , _администратор безопасности_ или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_ , _Global Administrator_ , _Security Administrator_ , or _Security Reader_.</span></span>
 

|<span data-ttu-id="dfaf9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfaf9-111">Permission type</span></span>      | <span data-ttu-id="dfaf9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfaf9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfaf9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfaf9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dfaf9-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfaf9-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfaf9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfaf9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfaf9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-116">Not supported.</span></span>    |
|<span data-ttu-id="dfaf9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfaf9-117">Application</span></span> | <span data-ttu-id="dfaf9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfaf9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfaf9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfaf9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfaf9-120">Optional query parameters</span></span>
<span data-ttu-id="dfaf9-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfaf9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfaf9-122">Request headers</span></span>
| <span data-ttu-id="dfaf9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dfaf9-123">Name</span></span>      |<span data-ttu-id="dfaf9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dfaf9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfaf9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfaf9-125">Authorization</span></span>  | <span data-ttu-id="dfaf9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfaf9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfaf9-128">Request body</span></span>
<span data-ttu-id="dfaf9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfaf9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfaf9-130">Response</span></span>

<span data-ttu-id="dfaf9-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедроле](../resources/privilegedrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="dfaf9-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dfaf9-133">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="dfaf9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dfaf9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfaf9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfaf9-135">Request</span></span>
<span data-ttu-id="dfaf9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfaf9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfaf9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="dfaf9-138">C#</span><span class="sxs-lookup"><span data-stu-id="dfaf9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfaf9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfaf9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfaf9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfaf9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfaf9-141">Java</span><span class="sxs-lookup"><span data-stu-id="dfaf9-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dfaf9-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfaf9-142">Response</span></span>
<span data-ttu-id="dfaf9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfaf9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
