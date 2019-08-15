---
title: 'user: findRooms'
description: 'Получение всех помещений для собраний в клиенте пользователя или определенном списке помещений. '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebfa5ad0c308cc2d4936c6e3a2a410a9656c3794
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421136"
---
# <a name="user-findrooms"></a><span data-ttu-id="c8fc3-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="c8fc3-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8fc3-104">Получение объектов [emailAddress](../resources/emailaddress.md), представляющих все помещения для собраний в клиенте пользователя или определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="c8fc3-105">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="c8fc3-106">В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="c8fc3-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="c8fc3-107">Можно [получить все списки помещений](user-findroomlists.md) в клиенте, получить все помещения в клиенте или получить все помещения в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="c8fc3-108">Можно получить до 100 первых помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8fc3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8fc3-109">Permissions</span></span>
<span data-ttu-id="c8fc3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8fc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c8fc3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8fc3-112">Permission type</span></span>      | <span data-ttu-id="c8fc3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8fc3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8fc3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8fc3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c8fc3-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8fc3-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="c8fc3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8fc3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8fc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-117">Not supported.</span></span>    |
|<span data-ttu-id="c8fc3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8fc3-118">Application</span></span> | <span data-ttu-id="c8fc3-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8fc3-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8fc3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8fc3-120">HTTP request</span></span>

<span data-ttu-id="c8fc3-121">Получение всех помещений в клиенте:</span><span class="sxs-lookup"><span data-stu-id="c8fc3-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="c8fc3-122">Получение всех помещений в определенном списке помещений клиента:</span><span class="sxs-lookup"><span data-stu-id="c8fc3-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="c8fc3-123">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c8fc3-123">Query parameters</span></span>

| <span data-ttu-id="c8fc3-124">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c8fc3-124">Query parameter</span></span>       | <span data-ttu-id="c8fc3-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c8fc3-125">Type</span></span> | <span data-ttu-id="c8fc3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c8fc3-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c8fc3-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="c8fc3-127">RoomList</span></span> | <span data-ttu-id="c8fc3-128">string</span><span class="sxs-lookup"><span data-stu-id="c8fc3-128">string</span></span> | <span data-ttu-id="c8fc3-129">SMTP-адрес, связанный со списком помещений.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="c8fc3-130">Каждый список помещений представлен экземпляром [emailAddress](../resources/emailaddress.md), включающим SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c8fc3-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8fc3-131">Request headers</span></span>
| <span data-ttu-id="c8fc3-132">Имя</span><span class="sxs-lookup"><span data-stu-id="c8fc3-132">Name</span></span>       | <span data-ttu-id="c8fc3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c8fc3-133">Type</span></span> | <span data-ttu-id="c8fc3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c8fc3-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c8fc3-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8fc3-135">Authorization</span></span>  | <span data-ttu-id="c8fc3-136">string</span><span class="sxs-lookup"><span data-stu-id="c8fc3-136">string</span></span>  | <span data-ttu-id="c8fc3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8fc3-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8fc3-139">Content-Type</span></span>  | <span data-ttu-id="c8fc3-140">string</span><span class="sxs-lookup"><span data-stu-id="c8fc3-140">string</span></span>  | <span data-ttu-id="c8fc3-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c8fc3-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8fc3-143">Request body</span></span>
<span data-ttu-id="c8fc3-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8fc3-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8fc3-145">Response</span></span>

<span data-ttu-id="c8fc3-146">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c8fc3-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c8fc3-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="c8fc3-148">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c8fc3-148">Request 1</span></span>

<span data-ttu-id="c8fc3-149">В первом примере возвращаются объекты [emailAddress](../resources/emailaddress.md), представляющие все помещения, определенные в клиенте вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c8fc3-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8fc3-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8fc3-151">C#</span><span class="sxs-lookup"><span data-stu-id="c8fc3-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8fc3-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8fc3-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8fc3-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8fc3-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="c8fc3-154">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="c8fc3-154">Response 1</span></span>
<span data-ttu-id="c8fc3-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-155">Here is an example of the response.</span></span> 

<span data-ttu-id="c8fc3-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="c8fc3-158">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c8fc3-158">Request 2</span></span>

<span data-ttu-id="c8fc3-159">Во втором примере возвращаются объекты [emailAddress](../resources/emailaddress.md), представляющие все помещения в указанном списке помещений, определенном по электронному адресу Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-159">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c8fc3-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8fc3-160">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8fc3-161">C#</span><span class="sxs-lookup"><span data-stu-id="c8fc3-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8fc3-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8fc3-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8fc3-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8fc3-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="c8fc3-164">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="c8fc3-164">Response 2</span></span>
<span data-ttu-id="c8fc3-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-165">Here is an example of the response.</span></span> 

<span data-ttu-id="c8fc3-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8fc3-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
