---
title: Список memberOf
description: 'Получение групп и ролей каталога, непосредственным участником которых является пользователь. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a7ac90a4d8dcdb74234e80d2e0b70d4011792bf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460268"
---
# <a name="list-memberof"></a><span data-ttu-id="f642b-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="f642b-103">List memberOf</span></span>

<span data-ttu-id="f642b-104">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f642b-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f642b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f642b-105">Permissions</span></span>
<span data-ttu-id="f642b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f642b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f642b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f642b-108">Permission type</span></span>      | <span data-ttu-id="f642b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f642b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f642b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f642b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f642b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f642b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f642b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f642b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f642b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f642b-113">Not supported.</span></span>    |
|<span data-ttu-id="f642b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f642b-114">Application</span></span> | <span data-ttu-id="f642b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f642b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f642b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f642b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f642b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f642b-117">Optional query parameters</span></span>
<span data-ttu-id="f642b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f642b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="f642b-119">$filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f642b-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="f642b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f642b-120">Request headers</span></span>
| <span data-ttu-id="f642b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f642b-121">Header</span></span>       | <span data-ttu-id="f642b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f642b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f642b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f642b-123">Authorization</span></span>  | <span data-ttu-id="f642b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f642b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f642b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f642b-126">Accept</span></span>  | <span data-ttu-id="f642b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f642b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f642b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f642b-128">Request body</span></span>
<span data-ttu-id="f642b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f642b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f642b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f642b-130">Response</span></span>

<span data-ttu-id="f642b-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f642b-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f642b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f642b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f642b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f642b-133">Request</span></span>
<span data-ttu-id="f642b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f642b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f642b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f642b-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f642b-136">C#</span><span class="sxs-lookup"><span data-stu-id="f642b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f642b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f642b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f642b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f642b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f642b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f642b-139">Response</span></span>
<span data-ttu-id="f642b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f642b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
