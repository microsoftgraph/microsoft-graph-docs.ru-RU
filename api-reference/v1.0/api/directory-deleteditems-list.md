---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: lleonard-msft
ms.openlocfilehash: 4c972ca554f7a073ddfb5b3472784240c691c973
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314282"
---
# <a name="list-deleted-items"></a><span data-ttu-id="3a253-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="3a253-103">List deleted items</span></span>

<span data-ttu-id="3a253-104">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="3a253-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="3a253-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3a253-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a253-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a253-106">Permissions</span></span>
<span data-ttu-id="3a253-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="3a253-109">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="3a253-109">For users:</span></span>

|<span data-ttu-id="3a253-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a253-110">Permission type</span></span>      | <span data-ttu-id="3a253-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a253-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a253-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a253-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a253-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a253-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3a253-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a253-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a253-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a253-115">Not supported.</span></span> |
|<span data-ttu-id="3a253-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a253-116">Application</span></span> | <span data-ttu-id="3a253-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a253-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="3a253-118">Для групп:</span><span class="sxs-lookup"><span data-stu-id="3a253-118">For groups:</span></span>

|<span data-ttu-id="3a253-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a253-119">Permission type</span></span>      | <span data-ttu-id="3a253-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a253-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a253-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a253-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3a253-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a253-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3a253-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a253-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a253-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a253-124">Not supported.</span></span>    |
|<span data-ttu-id="3a253-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a253-125">Application</span></span> | <span data-ttu-id="3a253-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a253-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a253-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a253-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="3a253-128">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="3a253-128">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="3a253-129">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="3a253-129">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="3a253-130">Вызов GET/каталог/deletedItems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a253-130">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3a253-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a253-131">Optional query parameters</span></span>
<span data-ttu-id="3a253-132">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a253-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a253-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a253-133">Request headers</span></span>
| <span data-ttu-id="3a253-134">Имя</span><span class="sxs-lookup"><span data-stu-id="3a253-134">Name</span></span>      |<span data-ttu-id="3a253-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3a253-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a253-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a253-136">Authorization</span></span>  | <span data-ttu-id="3a253-137">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="3a253-137">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="3a253-138">Accept</span><span class="sxs-lookup"><span data-stu-id="3a253-138">Accept</span></span>  | <span data-ttu-id="3a253-139">application/json</span><span class="sxs-lookup"><span data-stu-id="3a253-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a253-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a253-140">Request body</span></span>
<span data-ttu-id="3a253-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a253-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a253-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a253-142">Response</span></span>

<span data-ttu-id="3a253-143">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a253-143">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a253-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3a253-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a253-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a253-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="3a253-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a253-146">Response</span></span>
<span data-ttu-id="3a253-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a253-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->