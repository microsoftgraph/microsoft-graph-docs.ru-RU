---
title: 'user: findRoomLists'
description: Получение списка помещений, определенных в клиенте.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cc26367c9cecd16604f7cfefb3be5ce265e3c2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520580"
---
# <a name="user-findroomlists"></a><span data-ttu-id="e919f-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="e919f-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e919f-104">Получение списка помещений, определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e919f-104">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="e919f-105">Клиенты могут упорядочивать помещения для собраний в списках помещений.</span><span class="sxs-lookup"><span data-stu-id="e919f-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="e919f-106">Каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).</span><span class="sxs-lookup"><span data-stu-id="e919f-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="e919f-107">Можно получить все списки помещений в клиенте, [получить все помещения](user-findrooms.md) в клиенте или [получить все помещения](user-findrooms.md) в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="e919f-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="e919f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e919f-108">Permissions</span></span>
<span data-ttu-id="e919f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e919f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e919f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e919f-111">Permission type</span></span>      | <span data-ttu-id="e919f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e919f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e919f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e919f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e919f-114">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e919f-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e919f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e919f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e919f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e919f-116">Not supported.</span></span>    |
|<span data-ttu-id="e919f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e919f-117">Application</span></span> | <span data-ttu-id="e919f-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e919f-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e919f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e919f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="e919f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e919f-120">Request headers</span></span>
| <span data-ttu-id="e919f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e919f-121">Name</span></span>       | <span data-ttu-id="e919f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e919f-122">Type</span></span> | <span data-ttu-id="e919f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e919f-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="e919f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e919f-124">Authorization</span></span>  | <span data-ttu-id="e919f-125">string</span><span class="sxs-lookup"><span data-stu-id="e919f-125">string</span></span>  | <span data-ttu-id="e919f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e919f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e919f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e919f-128">Content-Type</span></span>  | <span data-ttu-id="e919f-129">string</span><span class="sxs-lookup"><span data-stu-id="e919f-129">string</span></span>  | <span data-ttu-id="e919f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e919f-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e919f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e919f-132">Request body</span></span>
<span data-ttu-id="e919f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e919f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e919f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e919f-134">Response</span></span>

<span data-ttu-id="e919f-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [emailAddress](../resources/emailaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e919f-135">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="e919f-136">Если в клиенте не определены списки, возвращается пустой массив.</span><span class="sxs-lookup"><span data-stu-id="e919f-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="e919f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e919f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e919f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e919f-138">Request</span></span>

<span data-ttu-id="e919f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e919f-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="e919f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e919f-140">Response</span></span>
<span data-ttu-id="e919f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e919f-141">Here is an example of the response.</span></span> 

<span data-ttu-id="e919f-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e919f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
