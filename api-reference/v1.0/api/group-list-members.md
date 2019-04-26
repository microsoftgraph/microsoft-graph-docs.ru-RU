---
title: Список участников
description: Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты и другие группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 70bf3040402c03dc1918d271a2abb8e4adb5d40b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584651"
---
# <a name="list-members"></a><span data-ttu-id="24bb4-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="24bb4-104">List members</span></span>
<span data-ttu-id="24bb4-p102">Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты и другие группы. Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="24bb4-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="24bb4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24bb4-108">Permissions</span></span>
<span data-ttu-id="24bb4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24bb4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24bb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24bb4-111">Permission type</span></span>      | <span data-ttu-id="24bb4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24bb4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24bb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24bb4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="24bb4-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24bb4-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="24bb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24bb4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24bb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24bb4-116">Not supported.</span></span>    |
|<span data-ttu-id="24bb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24bb4-117">Application</span></span> | <span data-ttu-id="24bb4-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="24bb4-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24bb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24bb4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24bb4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24bb4-120">Optional query parameters</span></span>
<span data-ttu-id="24bb4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="24bb4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24bb4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24bb4-122">Request headers</span></span>
| <span data-ttu-id="24bb4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="24bb4-123">Name</span></span>       | <span data-ttu-id="24bb4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="24bb4-124">Type</span></span> | <span data-ttu-id="24bb4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="24bb4-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="24bb4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="24bb4-126">Authorization</span></span>  | <span data-ttu-id="24bb4-127">string</span><span class="sxs-lookup"><span data-stu-id="24bb4-127">string</span></span>  | <span data-ttu-id="24bb4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24bb4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24bb4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24bb4-130">Request body</span></span>
<span data-ttu-id="24bb4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24bb4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24bb4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="24bb4-132">Response</span></span>
<span data-ttu-id="24bb4-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24bb4-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24bb4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="24bb4-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="24bb4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="24bb4-135">Request</span></span>
<span data-ttu-id="24bb4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24bb4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="24bb4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="24bb4-137">Response</span></span>
<span data-ttu-id="24bb4-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24bb4-138">The following is an example of the response.</span></span>
><span data-ttu-id="24bb4-139">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="24bb4-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24bb4-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24bb4-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
