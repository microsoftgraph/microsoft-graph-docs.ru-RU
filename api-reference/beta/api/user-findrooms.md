---
title: 'user: findRooms'
description: 'Получение всех помещений для собраний в клиенте пользователя или определенном списке помещений. '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9c7d6fb47a52e67ae5dd884d9413726e9b2e3bae
ms.sourcegitcommit: 126b15ac37fb199c7b1001f91e70d8463a18c280
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2019
ms.locfileid: "34083328"
---
# <a name="user-findrooms"></a><span data-ttu-id="9e081-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="9e081-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e081-104">Получение объектов [emailAddress](../resources/emailaddress.md), представляющих все помещения для собраний в клиенте пользователя или определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="9e081-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="9e081-105">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="9e081-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="9e081-106">В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="9e081-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="9e081-107">Можно [получить все списки помещений](user-findroomlists.md) в клиенте, получить все помещения в клиенте или получить все помещения в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="9e081-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="9e081-108">Можно получить до 100 первых помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9e081-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e081-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e081-109">Permissions</span></span>
<span data-ttu-id="9e081-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e081-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e081-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e081-112">Permission type</span></span>      | <span data-ttu-id="9e081-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e081-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e081-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e081-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9e081-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e081-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="9e081-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e081-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e081-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e081-117">Not supported.</span></span>    |
|<span data-ttu-id="9e081-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e081-118">Application</span></span> | <span data-ttu-id="9e081-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e081-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e081-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e081-120">HTTP request</span></span>

<span data-ttu-id="9e081-121">Получение всех помещений в клиенте:</span><span class="sxs-lookup"><span data-stu-id="9e081-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="9e081-122">Получение всех помещений в определенном списке помещений клиента:</span><span class="sxs-lookup"><span data-stu-id="9e081-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/<id>/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="9e081-123">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="9e081-123">Query parameters</span></span>

| <span data-ttu-id="9e081-124">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="9e081-124">Query parameter</span></span>       | <span data-ttu-id="9e081-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9e081-125">Type</span></span> | <span data-ttu-id="9e081-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9e081-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="9e081-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="9e081-127">RoomList</span></span> | <span data-ttu-id="9e081-128">string</span><span class="sxs-lookup"><span data-stu-id="9e081-128">string</span></span> | <span data-ttu-id="9e081-129">SMTP-адрес, связанный со списком помещений.</span><span class="sxs-lookup"><span data-stu-id="9e081-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="9e081-130">Каждый список помещений представлен экземпляром [emailAddress](../resources/emailaddress.md), включающим SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="9e081-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9e081-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e081-131">Request headers</span></span>
| <span data-ttu-id="9e081-132">Имя</span><span class="sxs-lookup"><span data-stu-id="9e081-132">Name</span></span>       | <span data-ttu-id="9e081-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9e081-133">Type</span></span> | <span data-ttu-id="9e081-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9e081-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="9e081-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e081-135">Authorization</span></span>  | <span data-ttu-id="9e081-136">string</span><span class="sxs-lookup"><span data-stu-id="9e081-136">string</span></span>  | <span data-ttu-id="9e081-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e081-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e081-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e081-139">Content-Type</span></span>  | <span data-ttu-id="9e081-140">string</span><span class="sxs-lookup"><span data-stu-id="9e081-140">string</span></span>  | <span data-ttu-id="9e081-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e081-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9e081-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e081-143">Request body</span></span>
<span data-ttu-id="9e081-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e081-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e081-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e081-145">Response</span></span>

<span data-ttu-id="9e081-146">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e081-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="9e081-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9e081-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="9e081-148">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="9e081-148">Request 1</span></span>

<span data-ttu-id="9e081-149">В первом примере возвращаются объекты [emailAddress](../resources/emailaddress.md), представляющие все помещения, определенные в клиенте вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e081-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="9e081-150">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="9e081-150">Response 1</span></span>
<span data-ttu-id="9e081-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e081-151">Here is an example of the response.</span></span> 

<span data-ttu-id="9e081-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e081-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
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
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9e081-154">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9e081-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9e081-155">C#</span><span class="sxs-lookup"><span data-stu-id="9e081-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e081-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e081-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="9e081-157">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="9e081-157">Request 2</span></span>

<span data-ttu-id="9e081-158">Во втором примере возвращаются объекты [emailAddress](../resources/emailaddress.md), представляющие все помещения в указанном списке помещений, определенном по электронному адресу Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="9e081-158">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="9e081-159">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="9e081-159">Response 2</span></span>
<span data-ttu-id="9e081-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e081-160">Here is an example of the response.</span></span> 

<span data-ttu-id="9e081-p107">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e081-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
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
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9e081-163">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9e081-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9e081-164">C#</span><span class="sxs-lookup"><span data-stu-id="9e081-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e081-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e081-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
