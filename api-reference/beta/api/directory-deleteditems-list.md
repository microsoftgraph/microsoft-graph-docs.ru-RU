---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6c33dc40d556f36b2155542a63f8b82f54e672b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009004"
---
# <a name="list-deleted-items"></a><span data-ttu-id="8e408-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="8e408-103">List deleted items</span></span>

<span data-ttu-id="8e408-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e408-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e408-105">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8e408-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="8e408-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="8e408-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e408-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e408-107">Permissions</span></span>

<span data-ttu-id="8e408-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="8e408-110">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="8e408-110">For applications:</span></span>

|<span data-ttu-id="8e408-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e408-111">Permission type</span></span>      | <span data-ttu-id="8e408-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e408-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e408-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e408-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e408-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e408-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8e408-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e408-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e408-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e408-116">Not supported.</span></span>    |
|<span data-ttu-id="8e408-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e408-117">Application</span></span> | <span data-ttu-id="8e408-118">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8e408-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="8e408-119">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="8e408-119">For users:</span></span>

|<span data-ttu-id="8e408-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e408-120">Permission type</span></span>      | <span data-ttu-id="8e408-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e408-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e408-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e408-122">Delegated (work or school account)</span></span> | <span data-ttu-id="8e408-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e408-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e408-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e408-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e408-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e408-125">Not supported.</span></span> |
|<span data-ttu-id="8e408-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e408-126">Application</span></span> | <span data-ttu-id="8e408-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e408-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="8e408-128">Для групп:</span><span class="sxs-lookup"><span data-stu-id="8e408-128">For groups:</span></span>

|<span data-ttu-id="8e408-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e408-129">Permission type</span></span>      | <span data-ttu-id="8e408-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e408-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e408-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e408-131">Delegated (work or school account)</span></span> | <span data-ttu-id="8e408-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e408-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e408-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e408-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e408-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e408-134">Not supported.</span></span>    |
|<span data-ttu-id="8e408-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e408-135">Application</span></span> | <span data-ttu-id="8e408-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e408-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e408-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e408-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="8e408-138">Этот API в настоящее время поддерживает получение типов объектов приложений (Microsoft. Graph. Application), групп (Microsoft. Graph. Group) или пользователей (Microsoft. Graph. User) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="8e408-138">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="8e408-139">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="8e408-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="8e408-140">Вызов GET /directory/deleteditems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e408-140">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8e408-141">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8e408-141">Optional query parameters</span></span>
<span data-ttu-id="8e408-142">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e408-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e408-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e408-143">Request headers</span></span>
| <span data-ttu-id="8e408-144">Имя</span><span class="sxs-lookup"><span data-stu-id="8e408-144">Name</span></span>      |<span data-ttu-id="8e408-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8e408-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e408-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e408-146">Authorization</span></span>  | <span data-ttu-id="8e408-147">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="8e408-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8e408-148">Accept</span><span class="sxs-lookup"><span data-stu-id="8e408-148">Accept</span></span>  | <span data-ttu-id="8e408-149">application/json</span><span class="sxs-lookup"><span data-stu-id="8e408-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e408-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e408-150">Request body</span></span>
<span data-ttu-id="8e408-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e408-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e408-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e408-152">Response</span></span>

<span data-ttu-id="8e408-153">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e408-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e408-154">Пример</span><span class="sxs-lookup"><span data-stu-id="8e408-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e408-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e408-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8e408-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e408-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="8e408-157">C#</span><span class="sxs-lookup"><span data-stu-id="8e408-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e408-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e408-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e408-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e408-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e408-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e408-160">Response</span></span>
<span data-ttu-id="8e408-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e408-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


