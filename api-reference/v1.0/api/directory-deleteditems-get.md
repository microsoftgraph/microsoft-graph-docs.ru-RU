---
title: Извлечение свойств недавно удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7095dc50e118e39f857373abda9071ba8701f75e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053204"
---
# <a name="get-deleted-item"></a><span data-ttu-id="8e27e-103">Получение удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="8e27e-103">Get deleted item</span></span>

<span data-ttu-id="8e27e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e27e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e27e-105">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8e27e-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="8e27e-106">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](../resources/application.md) [групповых и](../resources/group.md) [пользовательских](../resources/user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8e27e-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e27e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e27e-107">Permissions</span></span>
<span data-ttu-id="8e27e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e27e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="8e27e-110">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="8e27e-110">For applications:</span></span>

|<span data-ttu-id="8e27e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e27e-111">Permission type</span></span>      | <span data-ttu-id="8e27e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e27e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e27e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e27e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e27e-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e27e-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8e27e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e27e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e27e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e27e-116">Not supported.</span></span>    |
|<span data-ttu-id="8e27e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e27e-117">Application</span></span> | <span data-ttu-id="8e27e-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e27e-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="8e27e-119">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="8e27e-119">For users:</span></span>

|<span data-ttu-id="8e27e-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e27e-120">Permission type</span></span>      | <span data-ttu-id="8e27e-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e27e-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e27e-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e27e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="8e27e-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e27e-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="8e27e-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e27e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e27e-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e27e-125">Not supported.</span></span> |
|<span data-ttu-id="8e27e-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e27e-126">Application</span></span> | <span data-ttu-id="8e27e-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e27e-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="8e27e-128">Для групп:</span><span class="sxs-lookup"><span data-stu-id="8e27e-128">For groups:</span></span>

|<span data-ttu-id="8e27e-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e27e-129">Permission type</span></span>      | <span data-ttu-id="8e27e-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e27e-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e27e-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e27e-131">Delegated (work or school account)</span></span> | <span data-ttu-id="8e27e-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e27e-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e27e-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e27e-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e27e-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e27e-134">Not supported.</span></span>    |
|<span data-ttu-id="8e27e-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e27e-135">Application</span></span> | <span data-ttu-id="8e27e-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e27e-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e27e-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e27e-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e27e-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e27e-138">Optional query parameters</span></span>
<span data-ttu-id="8e27e-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e27e-139">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e27e-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e27e-140">Request headers</span></span>
| <span data-ttu-id="8e27e-141">Имя</span><span class="sxs-lookup"><span data-stu-id="8e27e-141">Name</span></span>      |<span data-ttu-id="8e27e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="8e27e-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e27e-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e27e-143">Authorization</span></span>  | <span data-ttu-id="8e27e-144">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="8e27e-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8e27e-145">Accept</span><span class="sxs-lookup"><span data-stu-id="8e27e-145">Accept</span></span>  | <span data-ttu-id="8e27e-146">application/json</span><span class="sxs-lookup"><span data-stu-id="8e27e-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e27e-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e27e-147">Request body</span></span>
<span data-ttu-id="8e27e-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e27e-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e27e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e27e-149">Response</span></span>

<span data-ttu-id="8e27e-150">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e27e-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e27e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="8e27e-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e27e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e27e-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8e27e-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e27e-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="8e27e-154">C#</span><span class="sxs-lookup"><span data-stu-id="8e27e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e27e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e27e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e27e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e27e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e27e-157">Java</span><span class="sxs-lookup"><span data-stu-id="8e27e-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e27e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e27e-158">Response</span></span>
<span data-ttu-id="8e27e-159">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e27e-159">Note: The response object shown here might be shortened for readability.</span></span>
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
