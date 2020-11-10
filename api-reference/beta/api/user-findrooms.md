---
title: 'user: findRooms'
description: 'Получение всех помещений для собраний в клиенте пользователя или определенном списке помещений. '
localization_priority: Priority
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 292634327717d720a80d55065041de7571660858
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970135"
---
# <a name="user-findrooms"></a><span data-ttu-id="d82d2-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="d82d2-103">user: findRooms</span></span>

<span data-ttu-id="d82d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d82d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d82d2-105">Получение объектов [emailAddress](../resources/emailaddress.md), представляющих все помещения для собраний в клиенте пользователя или определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="d82d2-105">Get the [emailAddress](../resources/emailaddress.md) objects that represent all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="d82d2-106">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="d82d2-106">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="d82d2-107">В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="d82d2-107">In this API, each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="d82d2-108">Можно [получить все списки помещений](user-findroomlists.md) в клиенте, получить все помещения в клиенте или получить все помещения в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="d82d2-108">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="d82d2-109">Можно получить до 100 первых помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d82d2-109">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d82d2-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d82d2-110">Permissions</span></span>
<span data-ttu-id="d82d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d82d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d82d2-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d82d2-113">Permission type</span></span>      | <span data-ttu-id="d82d2-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d82d2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d82d2-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d82d2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d82d2-116">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d82d2-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="d82d2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d82d2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d82d2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d82d2-118">Not supported.</span></span>    |
|<span data-ttu-id="d82d2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d82d2-119">Application</span></span> | <span data-ttu-id="d82d2-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d82d2-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d82d2-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d82d2-121">HTTP request</span></span>

<span data-ttu-id="d82d2-122">Получение всех помещений в клиенте:</span><span class="sxs-lookup"><span data-stu-id="d82d2-122">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="d82d2-123">Получение всех помещений в определенном списке помещений клиента:</span><span class="sxs-lookup"><span data-stu-id="d82d2-123">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="d82d2-124">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d82d2-124">Query parameters</span></span>

| <span data-ttu-id="d82d2-125">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="d82d2-125">Query parameter</span></span>       | <span data-ttu-id="d82d2-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d82d2-126">Type</span></span> | <span data-ttu-id="d82d2-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d82d2-127">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="d82d2-128">RoomList</span><span class="sxs-lookup"><span data-stu-id="d82d2-128">RoomList</span></span> | <span data-ttu-id="d82d2-129">string</span><span class="sxs-lookup"><span data-stu-id="d82d2-129">string</span></span> | <span data-ttu-id="d82d2-130">SMTP-адрес, связанный со списком помещений.</span><span class="sxs-lookup"><span data-stu-id="d82d2-130">The SMTP address associated with the room list.</span></span> <span data-ttu-id="d82d2-131">Каждый список помещений представлен экземпляром [emailAddress](../resources/emailaddress.md), включающим SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="d82d2-131">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d82d2-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d82d2-132">Request headers</span></span>
| <span data-ttu-id="d82d2-133">Имя</span><span class="sxs-lookup"><span data-stu-id="d82d2-133">Name</span></span>       | <span data-ttu-id="d82d2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="d82d2-134">Type</span></span> | <span data-ttu-id="d82d2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d82d2-135">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="d82d2-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="d82d2-136">Authorization</span></span>  | <span data-ttu-id="d82d2-137">string</span><span class="sxs-lookup"><span data-stu-id="d82d2-137">string</span></span>  | <span data-ttu-id="d82d2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d82d2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d82d2-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d82d2-140">Content-Type</span></span>  | <span data-ttu-id="d82d2-141">string</span><span class="sxs-lookup"><span data-stu-id="d82d2-141">string</span></span>  | <span data-ttu-id="d82d2-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d82d2-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d82d2-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d82d2-144">Request body</span></span>
<span data-ttu-id="d82d2-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d82d2-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d82d2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d82d2-146">Response</span></span>

<span data-ttu-id="d82d2-147">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d82d2-147">If successful, this method returns a `200 OK` response code and a collection of [emailAddress](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="d82d2-148">Пример</span><span class="sxs-lookup"><span data-stu-id="d82d2-148">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="d82d2-149">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="d82d2-149">Request 1</span></span>

<span data-ttu-id="d82d2-150">В первом примере возвращаются объекты [emailAddress](../resources/emailaddress.md), представляющие все помещения, определенные в клиенте вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="d82d2-150">The first example gets the [emailAddress](../resources/emailaddress.md) objects that represent all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="d82d2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d82d2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="c"></a>[<span data-ttu-id="d82d2-152">C#</span><span class="sxs-lookup"><span data-stu-id="d82d2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d82d2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d82d2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d82d2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d82d2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d82d2-155">Java</span><span class="sxs-lookup"><span data-stu-id="d82d2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-rooms-in-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="d82d2-156">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="d82d2-156">Response 1</span></span>
<span data-ttu-id="d82d2-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d82d2-157">Here is an example of the response.</span></span> 

<span data-ttu-id="d82d2-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d82d2-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="d82d2-160">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="d82d2-160">Request 2</span></span>

<span data-ttu-id="d82d2-161">Во втором примере возвращаются объекты [emailAddress](../resources/emailaddress.md), представляющие все помещения в указанном списке помещений, определенном по электронному адресу Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="d82d2-161">The second example gets the [emailAddress](../resources/emailaddress.md) objects that represent the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="http"></a>[<span data-ttu-id="d82d2-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d82d2-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="c"></a>[<span data-ttu-id="d82d2-163">C#</span><span class="sxs-lookup"><span data-stu-id="d82d2-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d82d2-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d82d2-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d82d2-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d82d2-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d82d2-166">Java</span><span class="sxs-lookup"><span data-stu-id="d82d2-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-rooms-from-specific-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="d82d2-167">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="d82d2-167">Response 2</span></span>
<span data-ttu-id="d82d2-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d82d2-168">Here is an example of the response.</span></span> 

<span data-ttu-id="d82d2-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d82d2-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


