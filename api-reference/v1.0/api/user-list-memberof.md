---
title: Список memberOf
description: 'Получение групп и ролей каталога, непосредственным участником которых является пользователь. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 477bfbd87081ae28aa45cd7498a731b4efaa6939
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509068"
---
# <a name="list-memberof"></a><span data-ttu-id="e828a-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="e828a-103">List memberOf</span></span>

<span data-ttu-id="e828a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e828a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e828a-105">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="e828a-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e828a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e828a-106">Permissions</span></span>
<span data-ttu-id="e828a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e828a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e828a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e828a-109">Permission type</span></span>      | <span data-ttu-id="e828a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e828a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e828a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e828a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e828a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e828a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e828a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e828a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e828a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e828a-114">Not supported.</span></span>    |
|<span data-ttu-id="e828a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e828a-115">Application</span></span> | <span data-ttu-id="e828a-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e828a-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e828a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e828a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e828a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e828a-118">Optional query parameters</span></span>
<span data-ttu-id="e828a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e828a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="e828a-120">$filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e828a-120">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e828a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e828a-121">Request headers</span></span>
| <span data-ttu-id="e828a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e828a-122">Header</span></span>       | <span data-ttu-id="e828a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e828a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e828a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e828a-124">Authorization</span></span>  | <span data-ttu-id="e828a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e828a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e828a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e828a-127">Accept</span></span>  | <span data-ttu-id="e828a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e828a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e828a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e828a-129">Request body</span></span>
<span data-ttu-id="e828a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e828a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e828a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e828a-131">Response</span></span>

<span data-ttu-id="e828a-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e828a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e828a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e828a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e828a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e828a-134">Request</span></span>
<span data-ttu-id="e828a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e828a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e828a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e828a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="c"></a>[<span data-ttu-id="e828a-137">C#</span><span class="sxs-lookup"><span data-stu-id="e828a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e828a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e828a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e828a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e828a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e828a-140">Java</span><span class="sxs-lookup"><span data-stu-id="e828a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e828a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e828a-141">Response</span></span>
<span data-ttu-id="e828a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e828a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
