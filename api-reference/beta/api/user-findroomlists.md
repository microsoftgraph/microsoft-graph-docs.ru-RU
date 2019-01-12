---
title: 'пользователь: findRoomLists'
description: Получение списков комнат, определенных в клиент.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f170b40689b09f54ea53632ca113018de1671b4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979294"
---
# <a name="user-findroomlists"></a><span data-ttu-id="4d4e0-103">пользователь: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="4d4e0-103">user: findRoomLists</span></span>

> <span data-ttu-id="4d4e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d4e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d4e0-106">Получение списков комнат, определенных в клиент.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-106">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="4d4e0-107">Клиенты можно упорядочить по комнаты для собраний списков комнат.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="4d4e0-108">Экземпляр [emailAddress](../resources/emailaddress.md) представлены каждого зала заседаний и список помещений.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="4d4e0-109">Можно получить все списки комнаты клиента, [Получение всех комнатах](user-findrooms.md) в клиентов или [Получение всех комнатах](user-findrooms.md) в список помещений определенных.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-109">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="4d4e0-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d4e0-110">Permissions</span></span>
<span data-ttu-id="4d4e0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d4e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d4e0-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d4e0-113">Permission type</span></span>      | <span data-ttu-id="4d4e0-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d4e0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d4e0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d4e0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4d4e0-116">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d4e0-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="4d4e0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d4e0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d4e0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-118">Not supported.</span></span>    |
|<span data-ttu-id="4d4e0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d4e0-119">Application</span></span> | <span data-ttu-id="4d4e0-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d4e0-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d4e0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d4e0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="4d4e0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d4e0-122">Request headers</span></span>
| <span data-ttu-id="4d4e0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4d4e0-123">Name</span></span>       | <span data-ttu-id="4d4e0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4d4e0-124">Type</span></span> | <span data-ttu-id="4d4e0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4d4e0-125">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="4d4e0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d4e0-126">Authorization</span></span>  | <span data-ttu-id="4d4e0-127">строка</span><span class="sxs-lookup"><span data-stu-id="4d4e0-127">string</span></span>  | <span data-ttu-id="4d4e0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d4e0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d4e0-130">Content-Type</span></span>  | <span data-ttu-id="4d4e0-131">строка</span><span class="sxs-lookup"><span data-stu-id="4d4e0-131">string</span></span>  | <span data-ttu-id="4d4e0-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4d4e0-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d4e0-134">Request body</span></span>
<span data-ttu-id="4d4e0-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d4e0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d4e0-136">Response</span></span>

<span data-ttu-id="4d4e0-137">Успешно завершена, этот метод возвращает `200 OK` кода и [emailAddress](../resources/emailaddress.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-137">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="4d4e0-138">Если нет списков определены в клиентов, возвращается пустой массив.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-138">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="4d4e0-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4d4e0-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d4e0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d4e0-140">Request</span></span>

<span data-ttu-id="4d4e0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="4d4e0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d4e0-142">Response</span></span>
<span data-ttu-id="4d4e0-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-143">Here is an example of the response.</span></span> 

<span data-ttu-id="4d4e0-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d4e0-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
