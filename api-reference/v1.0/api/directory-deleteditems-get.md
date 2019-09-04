---
title: Получение удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f148a16db752c6e996364af7d9e0e3fb8c94945
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721329"
---
# <a name="get-deleted-item"></a><span data-ttu-id="a6373-103">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="a6373-103">Get deleted item</span></span>

<span data-ttu-id="a6373-104">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a6373-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="a6373-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a6373-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6373-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6373-106">Permissions</span></span>
<span data-ttu-id="a6373-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="a6373-109">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="a6373-109">For users:</span></span>

|<span data-ttu-id="a6373-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6373-110">Permission type</span></span>      | <span data-ttu-id="a6373-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6373-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6373-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6373-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6373-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6373-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="a6373-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6373-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6373-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6373-115">Not supported.</span></span> |
|<span data-ttu-id="a6373-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6373-116">Application</span></span> | <span data-ttu-id="a6373-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6373-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="a6373-118">Для групп:</span><span class="sxs-lookup"><span data-stu-id="a6373-118">For groups:</span></span>

|<span data-ttu-id="a6373-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6373-119">Permission type</span></span>      | <span data-ttu-id="a6373-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6373-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6373-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6373-121">Delegated (work or school account)</span></span> | <span data-ttu-id="a6373-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6373-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a6373-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6373-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6373-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6373-124">Not supported.</span></span>    |
|<span data-ttu-id="a6373-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6373-125">Application</span></span> | <span data-ttu-id="a6373-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6373-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6373-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6373-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6373-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6373-128">Optional query parameters</span></span>
<span data-ttu-id="a6373-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6373-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6373-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6373-130">Request headers</span></span>
| <span data-ttu-id="a6373-131">Имя</span><span class="sxs-lookup"><span data-stu-id="a6373-131">Name</span></span>      |<span data-ttu-id="a6373-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6373-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6373-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6373-133">Authorization</span></span>  | <span data-ttu-id="a6373-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="a6373-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="a6373-135">Accept</span><span class="sxs-lookup"><span data-stu-id="a6373-135">Accept</span></span>  | <span data-ttu-id="a6373-136">application/json</span><span class="sxs-lookup"><span data-stu-id="a6373-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6373-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6373-137">Request body</span></span>
<span data-ttu-id="a6373-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6373-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6373-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6373-139">Response</span></span>

<span data-ttu-id="a6373-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6373-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6373-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a6373-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6373-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6373-142">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a6373-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6373-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6373-144">C#</span><span class="sxs-lookup"><span data-stu-id="a6373-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6373-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6373-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6373-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a6373-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a6373-147">Java</span><span class="sxs-lookup"><span data-stu-id="a6373-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a6373-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6373-148">Response</span></span>
<span data-ttu-id="a6373-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6373-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
