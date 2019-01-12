---
title: 'пользователь: findRooms'
description: 'Получение всех комнатах для собраний в клиент пользователя или в списке конкретных комнаты. '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0be6034056b20473b65e9a04c70419b3e4e1ba95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934011"
---
# <a name="user-findrooms"></a><span data-ttu-id="4de47-103">пользователь: findRooms</span><span class="sxs-lookup"><span data-stu-id="4de47-103">user: findRooms</span></span>

> <span data-ttu-id="4de47-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4de47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4de47-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4de47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4de47-106">Получение всех комнатах для собраний в клиент пользователя или в списке конкретных комнаты.</span><span class="sxs-lookup"><span data-stu-id="4de47-106">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="4de47-107">Клиенты можно упорядочить по комнаты для собраний списков комнат.</span><span class="sxs-lookup"><span data-stu-id="4de47-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="4de47-108">Экземпляр [emailAddress](../resources/emailaddress.md) представлены каждого зала заседаний и список помещений.</span><span class="sxs-lookup"><span data-stu-id="4de47-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="4de47-109">Можно [получить все списки помещения](user-findroomlists.md) в клиентов, получение всех комнатах в клиентов или получение всех комнатах в списке конкретных комнаты.</span><span class="sxs-lookup"><span data-stu-id="4de47-109">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="4de47-110">Вы можете получить регистрация первые 100 комнат в клиентов.</span><span class="sxs-lookup"><span data-stu-id="4de47-110">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4de47-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4de47-111">Permissions</span></span>
<span data-ttu-id="4de47-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4de47-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4de47-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4de47-114">Permission type</span></span>      | <span data-ttu-id="4de47-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4de47-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4de47-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4de47-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4de47-117">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4de47-117">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="4de47-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4de47-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4de47-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4de47-119">Not supported.</span></span>    |
|<span data-ttu-id="4de47-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4de47-120">Application</span></span> | <span data-ttu-id="4de47-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4de47-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4de47-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4de47-122">HTTP request</span></span>

<span data-ttu-id="4de47-123">Для получения всех комнатах клиента:</span><span class="sxs-lookup"><span data-stu-id="4de47-123">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="4de47-124">Чтобы получить все помещения в список помещений конкретного клиента:</span><span class="sxs-lookup"><span data-stu-id="4de47-124">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="4de47-125">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4de47-125">Query parameters</span></span>

| <span data-ttu-id="4de47-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="4de47-126">Query parameter</span></span>       | <span data-ttu-id="4de47-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4de47-127">Type</span></span> | <span data-ttu-id="4de47-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4de47-128">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="4de47-129">RoomList</span><span class="sxs-lookup"><span data-stu-id="4de47-129">RoomList</span></span> | <span data-ttu-id="4de47-130">строка</span><span class="sxs-lookup"><span data-stu-id="4de47-130">string</span></span> | <span data-ttu-id="4de47-131">SMTP-адрес, связанный с список помещений.</span><span class="sxs-lookup"><span data-stu-id="4de47-131">The SMTP address associated with the room list.</span></span> <span data-ttu-id="4de47-132">Каждый список помещений представляется экземпляром [emailAddress](../resources/emailaddress.md) , которое включает в себя SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="4de47-132">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4de47-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4de47-133">Request headers</span></span>
| <span data-ttu-id="4de47-134">Имя</span><span class="sxs-lookup"><span data-stu-id="4de47-134">Name</span></span>       | <span data-ttu-id="4de47-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4de47-135">Type</span></span> | <span data-ttu-id="4de47-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4de47-136">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="4de47-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="4de47-137">Authorization</span></span>  | <span data-ttu-id="4de47-138">строка</span><span class="sxs-lookup"><span data-stu-id="4de47-138">string</span></span>  | <span data-ttu-id="4de47-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4de47-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4de47-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4de47-141">Content-Type</span></span>  | <span data-ttu-id="4de47-142">строка</span><span class="sxs-lookup"><span data-stu-id="4de47-142">string</span></span>  | <span data-ttu-id="4de47-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4de47-p106">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4de47-145">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4de47-145">Request body</span></span>
<span data-ttu-id="4de47-146">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4de47-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4de47-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4de47-147">Response</span></span>

<span data-ttu-id="4de47-148">Успешно завершена, этот метод возвращает `200 OK` кода и [emailAddress](../resources/emailaddress.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4de47-148">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="4de47-149">Пример</span><span class="sxs-lookup"><span data-stu-id="4de47-149">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="4de47-150">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="4de47-150">Request 1</span></span>

<span data-ttu-id="4de47-151">В первом примере выполняется получение всех комнатах, определенные в пользователь выполнил вход для клиентов.</span><span class="sxs-lookup"><span data-stu-id="4de47-151">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="4de47-152">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="4de47-152">Response 1</span></span>
<span data-ttu-id="4de47-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4de47-153">Here is an example of the response.</span></span> 

<span data-ttu-id="4de47-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4de47-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="4de47-156">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="4de47-156">Request 2</span></span>

<span data-ttu-id="4de47-157">Во втором примере возвращает комнат в списке указанного комнаты, с адресом электронной почты Building2Rooms@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="4de47-157">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="4de47-158">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="4de47-158">Response 2</span></span>
<span data-ttu-id="4de47-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4de47-159">Here is an example of the response.</span></span> 

<span data-ttu-id="4de47-p108">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4de47-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
