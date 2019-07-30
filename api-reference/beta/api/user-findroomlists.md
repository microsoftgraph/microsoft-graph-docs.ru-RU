---
title: 'user: findRoomLists'
description: Получение списка помещений, определенных в клиенте.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1946b7080bf37d0852964f3fac677e04052f55d3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867768"
---
# <a name="user-findroomlists"></a><span data-ttu-id="708be-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="708be-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="708be-104">Получение списка помещений, определенных в клиенте, в соответствии с представлением в их объектах [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="708be-104">Get the room lists defined in a tenant, as represented by their [emailAddress](../resources/emailaddress.md) objects.</span></span>

<span data-ttu-id="708be-105">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="708be-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="708be-106">В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="708be-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="708be-107">Можно получить все списки помещений в клиенте, [получить все помещения](user-findrooms.md) в клиенте или [получить все помещения](user-findrooms.md) в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="708be-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="708be-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="708be-108">Permissions</span></span>
<span data-ttu-id="708be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="708be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="708be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="708be-111">Permission type</span></span>      | <span data-ttu-id="708be-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="708be-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="708be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="708be-113">Delegated (work or school account)</span></span> | <span data-ttu-id="708be-114">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="708be-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="708be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="708be-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="708be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="708be-116">Not supported.</span></span>    |
|<span data-ttu-id="708be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="708be-117">Application</span></span> | <span data-ttu-id="708be-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="708be-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="708be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="708be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="708be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="708be-120">Request headers</span></span>
| <span data-ttu-id="708be-121">Имя</span><span class="sxs-lookup"><span data-stu-id="708be-121">Name</span></span>       | <span data-ttu-id="708be-122">Тип</span><span class="sxs-lookup"><span data-stu-id="708be-122">Type</span></span> | <span data-ttu-id="708be-123">Описание</span><span class="sxs-lookup"><span data-stu-id="708be-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="708be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="708be-124">Authorization</span></span>  | <span data-ttu-id="708be-125">string</span><span class="sxs-lookup"><span data-stu-id="708be-125">string</span></span>  | <span data-ttu-id="708be-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="708be-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="708be-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="708be-128">Content-Type</span></span>  | <span data-ttu-id="708be-129">string</span><span class="sxs-lookup"><span data-stu-id="708be-129">string</span></span>  | <span data-ttu-id="708be-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="708be-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="708be-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="708be-132">Request body</span></span>
<span data-ttu-id="708be-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="708be-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="708be-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="708be-134">Response</span></span>

<span data-ttu-id="708be-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="708be-135">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>

<span data-ttu-id="708be-136">Если в клиенте не определены списки, возвращается пустой массив.</span><span class="sxs-lookup"><span data-stu-id="708be-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="708be-137">Пример</span><span class="sxs-lookup"><span data-stu-id="708be-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="708be-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="708be-138">Request</span></span>

<span data-ttu-id="708be-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="708be-139">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="708be-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="708be-140">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="708be-141">C#</span><span class="sxs-lookup"><span data-stu-id="708be-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-room-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="708be-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="708be-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-room-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="708be-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="708be-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-room-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="708be-144">Java</span><span class="sxs-lookup"><span data-stu-id="708be-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-room-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="708be-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="708be-145">Response</span></span>
<span data-ttu-id="708be-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="708be-146">Here is an example of the response.</span></span> 

<span data-ttu-id="708be-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="708be-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
