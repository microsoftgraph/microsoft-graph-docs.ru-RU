---
title: Список привилегированныхролей
description: Извлечение списка объектов privilegedRole.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 1567b4fbf3d1be3be85b309e2b6edab05e90828d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441325"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="2e956-103">Список привилегированныхролей</span><span class="sxs-lookup"><span data-stu-id="2e956-103">List privilegedRoles</span></span>

<span data-ttu-id="2e956-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e956-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e956-105">Извлечение списка [объектов privilegedRole.](../resources/privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="2e956-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="2e956-106">Чтобы отфильтровать результаты запроса, используйте стандартные выражения OData ``$filter`` в URI.</span><span class="sxs-lookup"><span data-stu-id="2e956-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e956-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e956-107">Permissions</span></span>
<span data-ttu-id="2e956-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2e956-110">У запросителя должна быть одна из следующих ролей: _администратор_ привилегированных _ролей,_ глобальный _администратор,_ администратор безопасности или _читатель безопасности._</span><span class="sxs-lookup"><span data-stu-id="2e956-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="2e956-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e956-111">Permission type</span></span>      | <span data-ttu-id="2e956-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e956-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e956-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e956-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2e956-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e956-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e956-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e956-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e956-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e956-116">Not supported.</span></span>    |
|<span data-ttu-id="2e956-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e956-117">Application</span></span> | <span data-ttu-id="2e956-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e956-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e956-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e956-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e956-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e956-120">Optional query parameters</span></span>
<span data-ttu-id="2e956-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e956-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e956-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e956-122">Request headers</span></span>
| <span data-ttu-id="2e956-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2e956-123">Name</span></span>      |<span data-ttu-id="2e956-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2e956-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e956-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e956-125">Authorization</span></span>  | <span data-ttu-id="2e956-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e956-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e956-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e956-128">Request body</span></span>
<span data-ttu-id="2e956-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e956-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e956-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e956-130">Response</span></span>

<span data-ttu-id="2e956-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [privilegedRole](../resources/privilegedrole.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2e956-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="2e956-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="2e956-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2e956-133">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="2e956-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="2e956-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2e956-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e956-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e956-135">Request</span></span>
<span data-ttu-id="2e956-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e956-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e956-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e956-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="2e956-138">C#</span><span class="sxs-lookup"><span data-stu-id="2e956-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e956-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e956-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e956-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e956-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e956-141">Java</span><span class="sxs-lookup"><span data-stu-id="2e956-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e956-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e956-142">Response</span></span>
<span data-ttu-id="2e956-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e956-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
