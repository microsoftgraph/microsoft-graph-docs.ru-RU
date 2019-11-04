---
title: Получение свойств недавно удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99725624da9d0d5106c44d391c66afff105bc047
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938816"
---
# <a name="get-deleted-item"></a><span data-ttu-id="dc742-103">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="dc742-103">Get deleted item</span></span>

<span data-ttu-id="dc742-104">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="dc742-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="dc742-105">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="dc742-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc742-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc742-106">Permissions</span></span>
<span data-ttu-id="dc742-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="dc742-109">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="dc742-109">For applications:</span></span>

|<span data-ttu-id="dc742-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc742-110">Permission type</span></span>      | <span data-ttu-id="dc742-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc742-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc742-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc742-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc742-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc742-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc742-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc742-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc742-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc742-115">Not supported.</span></span>    |
|<span data-ttu-id="dc742-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc742-116">Application</span></span> | <span data-ttu-id="dc742-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc742-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="dc742-118">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="dc742-118">For users:</span></span>

|<span data-ttu-id="dc742-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc742-119">Permission type</span></span>      | <span data-ttu-id="dc742-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc742-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc742-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc742-121">Delegated (work or school account)</span></span> | <span data-ttu-id="dc742-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc742-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="dc742-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc742-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc742-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc742-124">Not supported.</span></span> |
|<span data-ttu-id="dc742-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="dc742-125">Application</span></span> | <span data-ttu-id="dc742-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc742-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="dc742-127">Для групп:</span><span class="sxs-lookup"><span data-stu-id="dc742-127">For groups:</span></span>

|<span data-ttu-id="dc742-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc742-128">Permission type</span></span>      | <span data-ttu-id="dc742-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc742-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc742-130">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc742-130">Delegated (work or school account)</span></span> | <span data-ttu-id="dc742-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc742-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="dc742-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc742-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc742-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc742-133">Not supported.</span></span>    |
|<span data-ttu-id="dc742-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc742-134">Application</span></span> | <span data-ttu-id="dc742-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc742-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc742-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc742-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc742-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc742-137">Optional query parameters</span></span>
<span data-ttu-id="dc742-138">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc742-138">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc742-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc742-139">Request headers</span></span>
| <span data-ttu-id="dc742-140">Имя</span><span class="sxs-lookup"><span data-stu-id="dc742-140">Name</span></span>      |<span data-ttu-id="dc742-141">Описание</span><span class="sxs-lookup"><span data-stu-id="dc742-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc742-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc742-142">Authorization</span></span>  | <span data-ttu-id="dc742-143">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="dc742-143">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="dc742-144">Accept</span><span class="sxs-lookup"><span data-stu-id="dc742-144">Accept</span></span>  | <span data-ttu-id="dc742-145">application/json</span><span class="sxs-lookup"><span data-stu-id="dc742-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc742-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc742-146">Request body</span></span>
<span data-ttu-id="dc742-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc742-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc742-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc742-148">Response</span></span>

<span data-ttu-id="dc742-149">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc742-149">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc742-150">Пример</span><span class="sxs-lookup"><span data-stu-id="dc742-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc742-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc742-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc742-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc742-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc742-153">C#</span><span class="sxs-lookup"><span data-stu-id="dc742-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc742-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc742-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc742-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc742-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc742-156">Java</span><span class="sxs-lookup"><span data-stu-id="dc742-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc742-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc742-157">Response</span></span>
<span data-ttu-id="dc742-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc742-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
