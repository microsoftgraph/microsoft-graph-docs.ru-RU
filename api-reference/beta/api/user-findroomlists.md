---
title: 'пользователь: findRoomLists'
description: Получение списков комнат, определенных в клиент.
author: dkershaw10
ms.openlocfilehash: f96f8e5c6349e87d2d71820b7b7cd3b0367908f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310775"
---
# <a name="user-findroomlists"></a><span data-ttu-id="645f1-103">пользователь: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="645f1-103">user: findRoomLists</span></span>

> <span data-ttu-id="645f1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="645f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="645f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="645f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="645f1-106">Получение списков комнат, определенных в клиент.</span><span class="sxs-lookup"><span data-stu-id="645f1-106">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="645f1-107">Клиенты можно упорядочить по комнаты для собраний списков комнат.</span><span class="sxs-lookup"><span data-stu-id="645f1-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="645f1-108">Экземпляр [emailAddress](../resources/emailaddress.md) представлены каждого зала заседаний и список помещений.</span><span class="sxs-lookup"><span data-stu-id="645f1-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="645f1-109">Можно получить все списки комнаты клиента, [Получение всех комнатах](user-findrooms.md) в клиентов или [Получение всех комнатах](user-findrooms.md) в список помещений определенных.</span><span class="sxs-lookup"><span data-stu-id="645f1-109">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="645f1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="645f1-110">Permissions</span></span>
<span data-ttu-id="645f1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="645f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="645f1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="645f1-113">Permission type</span></span>      | <span data-ttu-id="645f1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="645f1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="645f1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="645f1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="645f1-116">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="645f1-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="645f1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="645f1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="645f1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="645f1-118">Not supported.</span></span>    |
|<span data-ttu-id="645f1-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="645f1-119">Application</span></span> | <span data-ttu-id="645f1-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="645f1-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="645f1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="645f1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="645f1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="645f1-122">Request headers</span></span>
| <span data-ttu-id="645f1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="645f1-123">Name</span></span>       | <span data-ttu-id="645f1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="645f1-124">Type</span></span> | <span data-ttu-id="645f1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="645f1-125">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="645f1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="645f1-126">Authorization</span></span>  | <span data-ttu-id="645f1-127">string</span><span class="sxs-lookup"><span data-stu-id="645f1-127">string</span></span>  | <span data-ttu-id="645f1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="645f1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="645f1-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="645f1-130">Content-Type</span></span>  | <span data-ttu-id="645f1-131">строка</span><span class="sxs-lookup"><span data-stu-id="645f1-131">string</span></span>  | <span data-ttu-id="645f1-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="645f1-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="645f1-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="645f1-134">Request body</span></span>
<span data-ttu-id="645f1-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="645f1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="645f1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="645f1-136">Response</span></span>

<span data-ttu-id="645f1-137">Успешно завершена, этот метод возвращает `200 OK` кода и [emailAddress](../resources/emailaddress.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="645f1-137">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="645f1-138">Если нет списков определены в клиентов, возвращается пустой массив.</span><span class="sxs-lookup"><span data-stu-id="645f1-138">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="645f1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="645f1-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="645f1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="645f1-140">Request</span></span>

<span data-ttu-id="645f1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="645f1-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="645f1-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="645f1-142">Response</span></span>
<span data-ttu-id="645f1-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="645f1-143">Here is an example of the response.</span></span> 

<span data-ttu-id="645f1-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="645f1-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->