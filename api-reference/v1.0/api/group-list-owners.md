---
title: Список владельцев
description: 'Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы. '
ms.openlocfilehash: 9bb7592827f5dfe9eef2aff0fa8917fe68f683dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026349"
---
# <a name="list-owners"></a><span data-ttu-id="f7e19-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="f7e19-104">List owners</span></span>
<span data-ttu-id="f7e19-p102">Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="f7e19-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f7e19-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e19-107">Permissions</span></span>
<span data-ttu-id="f7e19-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e19-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e19-110">Permission type</span></span>      | <span data-ttu-id="f7e19-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e19-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7e19-113">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e19-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="f7e19-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e19-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e19-115">Not supported.</span></span>    |
|<span data-ttu-id="f7e19-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7e19-116">Application</span></span> | <span data-ttu-id="f7e19-117">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e19-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7e19-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7e19-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7e19-119">Optional query parameters</span></span>
<span data-ttu-id="f7e19-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7e19-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7e19-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e19-121">Request headers</span></span>
| <span data-ttu-id="f7e19-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f7e19-122">Name</span></span>       | <span data-ttu-id="f7e19-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f7e19-123">Type</span></span> | <span data-ttu-id="f7e19-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e19-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7e19-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e19-125">Authorization</span></span>  | <span data-ttu-id="f7e19-126">string</span><span class="sxs-lookup"><span data-stu-id="f7e19-126">string</span></span>  | <span data-ttu-id="f7e19-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e19-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7e19-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7e19-129">Request body</span></span>
<span data-ttu-id="f7e19-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7e19-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e19-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e19-131">Response</span></span>
<span data-ttu-id="f7e19-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e19-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e19-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f7e19-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7e19-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e19-134">Request</span></span>
<span data-ttu-id="f7e19-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7e19-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="f7e19-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7e19-136">Response</span></span>
<span data-ttu-id="f7e19-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f7e19-137">The following is an example of the response.</span></span>
><span data-ttu-id="f7e19-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="f7e19-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f7e19-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7e19-139">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
