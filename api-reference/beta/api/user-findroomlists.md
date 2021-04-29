---
title: 'user: findRoomLists'
description: Получение списка помещений, определенных в клиенте.
author: vrod9429
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c091ac7071ce76dbb59cb69c10da2b6fa519f3cc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052651"
---
# <a name="user-findroomlists"></a><span data-ttu-id="8333c-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="8333c-103">user: findRoomLists</span></span>

<span data-ttu-id="8333c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8333c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8333c-105">Получение списка помещений, определенных в клиенте, в соответствии с представлением в их объектах [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="8333c-105">Get the room lists defined in a tenant, as represented by their [emailAddress](../resources/emailaddress.md) objects.</span></span>

<span data-ttu-id="8333c-106">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="8333c-106">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="8333c-107">В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="8333c-107">In this API, each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="8333c-108">Можно получить все списки помещений в клиенте, [получить все помещения](user-findrooms.md) в клиенте или [получить все помещения](user-findrooms.md) в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="8333c-108">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="8333c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8333c-109">Permissions</span></span>
<span data-ttu-id="8333c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8333c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8333c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8333c-112">Permission type</span></span>      | <span data-ttu-id="8333c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8333c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8333c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8333c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8333c-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8333c-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="8333c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8333c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8333c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8333c-117">Not supported.</span></span>    |
|<span data-ttu-id="8333c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8333c-118">Application</span></span> | <span data-ttu-id="8333c-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8333c-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8333c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8333c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/{id}/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="8333c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8333c-121">Request headers</span></span>
| <span data-ttu-id="8333c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8333c-122">Name</span></span>       | <span data-ttu-id="8333c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8333c-123">Type</span></span> | <span data-ttu-id="8333c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8333c-124">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="8333c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8333c-125">Authorization</span></span>  | <span data-ttu-id="8333c-126">string</span><span class="sxs-lookup"><span data-stu-id="8333c-126">string</span></span>  | <span data-ttu-id="8333c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8333c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8333c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8333c-129">Content-Type</span></span>  | <span data-ttu-id="8333c-130">string</span><span class="sxs-lookup"><span data-stu-id="8333c-130">string</span></span>  | <span data-ttu-id="8333c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8333c-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8333c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8333c-133">Request body</span></span>
<span data-ttu-id="8333c-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8333c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8333c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8333c-135">Response</span></span>

<span data-ttu-id="8333c-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8333c-136">If successful, this method returns a `200 OK` response code and a collection of [emailAddress](../resources/emailaddress.md) objects in the response body.</span></span>

<span data-ttu-id="8333c-137">Если в клиенте не определены списки, возвращается пустой массив.</span><span class="sxs-lookup"><span data-stu-id="8333c-137">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="8333c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8333c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8333c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8333c-139">Request</span></span>

<span data-ttu-id="8333c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8333c-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8333c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8333c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRoomLists
```
# <a name="c"></a>[<span data-ttu-id="8333c-142">C#</span><span class="sxs-lookup"><span data-stu-id="8333c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-room-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8333c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8333c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-room-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8333c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8333c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-room-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8333c-145">Java</span><span class="sxs-lookup"><span data-stu-id="8333c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-room-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8333c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8333c-146">Response</span></span>
<span data-ttu-id="8333c-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8333c-147">Here is an example of the response.</span></span> 

<span data-ttu-id="8333c-148">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8333c-148">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


