---
title: 'пользователь: findRooms'
description: 'Получение всех комнатах для собраний в клиент пользователя или в списке конкретных комнаты. '
ms.openlocfilehash: 3169202f83af0696cbd2aaadd83d3beb9a3c01d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080161"
---
# <a name="user-findrooms"></a><span data-ttu-id="baae1-103">пользователь: findRooms</span><span class="sxs-lookup"><span data-stu-id="baae1-103">user: findRooms</span></span>

> <span data-ttu-id="baae1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="baae1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="baae1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baae1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="baae1-106">Получение всех комнатах для собраний в клиент пользователя или в списке конкретных комнаты.</span><span class="sxs-lookup"><span data-stu-id="baae1-106">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="baae1-107">Клиенты можно упорядочить по комнаты для собраний списков комнат.</span><span class="sxs-lookup"><span data-stu-id="baae1-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="baae1-108">Экземпляр [emailAddress](../resources/emailaddress.md) представлены каждого зала заседаний и список помещений.</span><span class="sxs-lookup"><span data-stu-id="baae1-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="baae1-109">Можно [получить все списки помещения](user-findroomlists.md) в клиентов, получение всех комнатах в клиентов или получение всех комнатах в списке конкретных комнаты.</span><span class="sxs-lookup"><span data-stu-id="baae1-109">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="baae1-110">Вы можете получить регистрация первые 100 комнат в клиентов.</span><span class="sxs-lookup"><span data-stu-id="baae1-110">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="baae1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="baae1-111">Permissions</span></span>
<span data-ttu-id="baae1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baae1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="baae1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baae1-114">Permission type</span></span>      | <span data-ttu-id="baae1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="baae1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baae1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baae1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="baae1-117">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="baae1-117">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="baae1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baae1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baae1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baae1-119">Not supported.</span></span>    |
|<span data-ttu-id="baae1-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baae1-120">Application</span></span> | <span data-ttu-id="baae1-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="baae1-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="baae1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baae1-122">HTTP request</span></span>

<span data-ttu-id="baae1-123">Для получения всех комнатах клиента:</span><span class="sxs-lookup"><span data-stu-id="baae1-123">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="baae1-124">Чтобы получить все помещения в список помещений конкретного клиента:</span><span class="sxs-lookup"><span data-stu-id="baae1-124">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="baae1-125">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="baae1-125">Query parameters</span></span>

| <span data-ttu-id="baae1-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="baae1-126">Query parameter</span></span>       | <span data-ttu-id="baae1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="baae1-127">Type</span></span> | <span data-ttu-id="baae1-128">Description</span><span class="sxs-lookup"><span data-stu-id="baae1-128">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="baae1-129">RoomList</span><span class="sxs-lookup"><span data-stu-id="baae1-129">RoomList</span></span> | <span data-ttu-id="baae1-130">string</span><span class="sxs-lookup"><span data-stu-id="baae1-130">string</span></span> | <span data-ttu-id="baae1-131">SMTP-адрес, связанный с список помещений.</span><span class="sxs-lookup"><span data-stu-id="baae1-131">The SMTP address associated with the room list.</span></span> <span data-ttu-id="baae1-132">Каждый список помещений представляется экземпляром [emailAddress](../resources/emailaddress.md) , которое включает в себя SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="baae1-132">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="baae1-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="baae1-133">Request headers</span></span>
| <span data-ttu-id="baae1-134">Имя</span><span class="sxs-lookup"><span data-stu-id="baae1-134">Name</span></span>       | <span data-ttu-id="baae1-135">Тип</span><span class="sxs-lookup"><span data-stu-id="baae1-135">Type</span></span> | <span data-ttu-id="baae1-136">Описание</span><span class="sxs-lookup"><span data-stu-id="baae1-136">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="baae1-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="baae1-137">Authorization</span></span>  | <span data-ttu-id="baae1-138">string</span><span class="sxs-lookup"><span data-stu-id="baae1-138">string</span></span>  | <span data-ttu-id="baae1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baae1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="baae1-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="baae1-141">Content-Type</span></span>  | <span data-ttu-id="baae1-142">строка</span><span class="sxs-lookup"><span data-stu-id="baae1-142">string</span></span>  | <span data-ttu-id="baae1-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baae1-p106">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="baae1-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="baae1-145">Request body</span></span>
<span data-ttu-id="baae1-146">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="baae1-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baae1-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="baae1-147">Response</span></span>

<span data-ttu-id="baae1-148">Успешно завершена, этот метод возвращает `200 OK` кода и [emailAddress](../resources/emailaddress.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="baae1-148">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="baae1-149">Пример</span><span class="sxs-lookup"><span data-stu-id="baae1-149">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="baae1-150">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="baae1-150">Request 1</span></span>

<span data-ttu-id="baae1-151">В первом примере выполняется получение всех комнатах, определенные в пользователь выполнил вход для клиентов.</span><span class="sxs-lookup"><span data-stu-id="baae1-151">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="baae1-152">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="baae1-152">Response 1</span></span>
<span data-ttu-id="baae1-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="baae1-153">Here is an example of the response.</span></span> 

<span data-ttu-id="baae1-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baae1-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="baae1-156">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="baae1-156">Request 2</span></span>

<span data-ttu-id="baae1-157">Во втором примере возвращает комнат в списке указанного комнаты, с адресом электронной почты Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="baae1-157">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="baae1-158">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="baae1-158">Response 2</span></span>
<span data-ttu-id="baae1-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="baae1-159">Here is an example of the response.</span></span> 

<span data-ttu-id="baae1-p108">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baae1-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->