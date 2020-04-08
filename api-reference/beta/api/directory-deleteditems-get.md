---
title: Получение удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36d93cb91efe7bbd696fbd90c0a1de4640e67f62
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181030"
---
# <a name="get-deleted-item"></a><span data-ttu-id="3506a-103">Получение удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="3506a-103">Get deleted item</span></span>

<span data-ttu-id="3506a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3506a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3506a-105">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="3506a-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="3506a-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="3506a-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="3506a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3506a-107">Permissions</span></span>
<span data-ttu-id="3506a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3506a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="3506a-110">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="3506a-110">For applications:</span></span>

|<span data-ttu-id="3506a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3506a-111">Permission type</span></span>      | <span data-ttu-id="3506a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3506a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3506a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3506a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3506a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3506a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3506a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3506a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3506a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3506a-116">Not supported.</span></span>    |
|<span data-ttu-id="3506a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3506a-117">Application</span></span> | <span data-ttu-id="3506a-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3506a-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="3506a-119">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="3506a-119">For users:</span></span>

|<span data-ttu-id="3506a-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3506a-120">Permission type</span></span>      | <span data-ttu-id="3506a-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3506a-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3506a-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3506a-122">Delegated (work or school account)</span></span> | <span data-ttu-id="3506a-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3506a-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="3506a-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3506a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3506a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3506a-125">Not supported.</span></span> |
|<span data-ttu-id="3506a-126">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3506a-126">Application</span></span> | <span data-ttu-id="3506a-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3506a-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="3506a-128">Для групп:</span><span class="sxs-lookup"><span data-stu-id="3506a-128">For groups:</span></span>

|<span data-ttu-id="3506a-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3506a-129">Permission type</span></span>      | <span data-ttu-id="3506a-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3506a-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3506a-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3506a-131">Delegated (work or school account)</span></span> | <span data-ttu-id="3506a-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3506a-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3506a-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3506a-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3506a-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3506a-134">Not supported.</span></span>    |
|<span data-ttu-id="3506a-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3506a-135">Application</span></span> | <span data-ttu-id="3506a-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3506a-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3506a-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3506a-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3506a-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3506a-138">Optional query parameters</span></span>
<span data-ttu-id="3506a-139">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3506a-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3506a-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3506a-140">Request headers</span></span>
| <span data-ttu-id="3506a-141">Имя</span><span class="sxs-lookup"><span data-stu-id="3506a-141">Name</span></span>      |<span data-ttu-id="3506a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="3506a-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3506a-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="3506a-143">Authorization</span></span>  | <span data-ttu-id="3506a-144">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="3506a-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="3506a-145">Accept</span><span class="sxs-lookup"><span data-stu-id="3506a-145">Accept</span></span>  | <span data-ttu-id="3506a-146">application/json</span><span class="sxs-lookup"><span data-stu-id="3506a-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3506a-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3506a-147">Request body</span></span>
<span data-ttu-id="3506a-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3506a-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3506a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3506a-149">Response</span></span>

<span data-ttu-id="3506a-150">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3506a-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3506a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="3506a-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3506a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="3506a-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3506a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="3506a-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="3506a-154">C#</span><span class="sxs-lookup"><span data-stu-id="3506a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3506a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3506a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3506a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3506a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3506a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3506a-157">Response</span></span>
<span data-ttu-id="3506a-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3506a-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
