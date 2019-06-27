---
title: 'user: findRoomLists'
description: Получение списка помещений, определенных в клиенте.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a2d2c4aad744e75644fc27a41149905e4f9904a4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270373"
---
# <a name="user-findroomlists"></a><span data-ttu-id="5315c-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="5315c-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5315c-104">Получение списка помещений, определенных в клиенте, в соответствии с представлением в их объектах [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="5315c-104">Get the room lists defined in a tenant, as represented by their [emailAddress](../resources/emailaddress.md) objects.</span></span>

<span data-ttu-id="5315c-105">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="5315c-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="5315c-106">В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="5315c-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="5315c-107">Можно получить все списки помещений в клиенте, [получить все помещения](user-findrooms.md) в клиенте или [получить все помещения](user-findrooms.md) в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="5315c-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="5315c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5315c-108">Permissions</span></span>
<span data-ttu-id="5315c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5315c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5315c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5315c-111">Permission type</span></span>      | <span data-ttu-id="5315c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5315c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5315c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5315c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5315c-114">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5315c-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="5315c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5315c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5315c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5315c-116">Not supported.</span></span>    |
|<span data-ttu-id="5315c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5315c-117">Application</span></span> | <span data-ttu-id="5315c-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5315c-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5315c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5315c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="5315c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5315c-120">Request headers</span></span>
| <span data-ttu-id="5315c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5315c-121">Name</span></span>       | <span data-ttu-id="5315c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5315c-122">Type</span></span> | <span data-ttu-id="5315c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5315c-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="5315c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5315c-124">Authorization</span></span>  | <span data-ttu-id="5315c-125">string</span><span class="sxs-lookup"><span data-stu-id="5315c-125">string</span></span>  | <span data-ttu-id="5315c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5315c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5315c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5315c-128">Content-Type</span></span>  | <span data-ttu-id="5315c-129">string</span><span class="sxs-lookup"><span data-stu-id="5315c-129">string</span></span>  | <span data-ttu-id="5315c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5315c-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5315c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5315c-132">Request body</span></span>
<span data-ttu-id="5315c-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5315c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5315c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5315c-134">Response</span></span>

<span data-ttu-id="5315c-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5315c-135">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>

<span data-ttu-id="5315c-136">Если в клиенте не определены списки, возвращается пустой массив.</span><span class="sxs-lookup"><span data-stu-id="5315c-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="5315c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5315c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5315c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5315c-138">Request</span></span>

<span data-ttu-id="5315c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5315c-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="5315c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5315c-140">Response</span></span>
<span data-ttu-id="5315c-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5315c-141">Here is an example of the response.</span></span> 

<span data-ttu-id="5315c-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5315c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5315c-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5315c-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5315c-145">C#</span><span class="sxs-lookup"><span data-stu-id="5315c-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_room_lists-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5315c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5315c-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_room_lists-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5315c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5315c-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_get_room_lists-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


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
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
