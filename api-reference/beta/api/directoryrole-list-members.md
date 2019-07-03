---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6884513d2b95bcd322a1d920865cbd44c5ce3b25
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436930"
---
# <a name="list-members"></a><span data-ttu-id="2309c-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="2309c-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2309c-105">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="2309c-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="2309c-106">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="2309c-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="2309c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2309c-107">Permissions</span></span>
<span data-ttu-id="2309c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2309c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2309c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2309c-110">Permission type</span></span>      | <span data-ttu-id="2309c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2309c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2309c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2309c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2309c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2309c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2309c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2309c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2309c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2309c-115">Not supported.</span></span>    |
|<span data-ttu-id="2309c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2309c-116">Application</span></span> | <span data-ttu-id="2309c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2309c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2309c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2309c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2309c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2309c-119">Optional query parameters</span></span>
<span data-ttu-id="2309c-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2309c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2309c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2309c-121">Request headers</span></span>
| <span data-ttu-id="2309c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2309c-122">Name</span></span>       | <span data-ttu-id="2309c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2309c-123">Type</span></span> | <span data-ttu-id="2309c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2309c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2309c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2309c-125">Authorization</span></span>  | <span data-ttu-id="2309c-126">string</span><span class="sxs-lookup"><span data-stu-id="2309c-126">string</span></span>  | <span data-ttu-id="2309c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2309c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2309c-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2309c-129">Request body</span></span>
<span data-ttu-id="2309c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2309c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2309c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2309c-131">Response</span></span>

<span data-ttu-id="2309c-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2309c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2309c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2309c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2309c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2309c-134">Request</span></span>
<span data-ttu-id="2309c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2309c-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2309c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2309c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2309c-137">C#</span><span class="sxs-lookup"><span data-stu-id="2309c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2309c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="2309c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2309c-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2309c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2309c-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="2309c-140">Response</span></span>
<span data-ttu-id="2309c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2309c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
