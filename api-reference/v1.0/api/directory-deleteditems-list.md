---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8f573f958cbc1a5acafa8022b3a90168cdcb5e4e
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405076"
---
# <a name="list-deleted-items"></a><span data-ttu-id="ece57-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="ece57-103">List deleted items</span></span>

<span data-ttu-id="ece57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ece57-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ece57-105">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ece57-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ece57-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="ece57-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ece57-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ece57-107">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="ece57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="ece57-110">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="ece57-110">For applications:</span></span>

|<span data-ttu-id="ece57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ece57-111">Permission type</span></span>      | <span data-ttu-id="ece57-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ece57-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ece57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ece57-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ece57-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ece57-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ece57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ece57-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ece57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece57-116">Not supported.</span></span>    |
|<span data-ttu-id="ece57-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ece57-117">Application</span></span> | <span data-ttu-id="ece57-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ece57-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="ece57-119">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="ece57-119">For users:</span></span>

|<span data-ttu-id="ece57-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ece57-120">Permission type</span></span>      | <span data-ttu-id="ece57-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ece57-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ece57-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ece57-122">Delegated (work or school account)</span></span> | <span data-ttu-id="ece57-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ece57-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ece57-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ece57-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ece57-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece57-125">Not supported.</span></span> |
|<span data-ttu-id="ece57-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ece57-126">Application</span></span> | <span data-ttu-id="ece57-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece57-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ece57-128">Для групп:</span><span class="sxs-lookup"><span data-stu-id="ece57-128">For groups:</span></span>

|<span data-ttu-id="ece57-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ece57-129">Permission type</span></span>      | <span data-ttu-id="ece57-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ece57-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ece57-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ece57-131">Delegated (work or school account)</span></span> | <span data-ttu-id="ece57-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ece57-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ece57-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ece57-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ece57-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece57-134">Not supported.</span></span>    |
|<span data-ttu-id="ece57-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ece57-135">Application</span></span> | <span data-ttu-id="ece57-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ece57-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ece57-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ece57-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="ece57-138">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="ece57-138">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="ece57-139">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="ece57-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="ece57-140">Вызов GET/директори/делетедитемс без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece57-140">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ece57-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ece57-141">Optional query parameters</span></span>
<span data-ttu-id="ece57-142">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ece57-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ece57-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ece57-143">Request headers</span></span>
| <span data-ttu-id="ece57-144">Имя</span><span class="sxs-lookup"><span data-stu-id="ece57-144">Name</span></span>      |<span data-ttu-id="ece57-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ece57-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ece57-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ece57-146">Authorization</span></span>  | <span data-ttu-id="ece57-147">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="ece57-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ece57-148">Accept</span><span class="sxs-lookup"><span data-stu-id="ece57-148">Accept</span></span>  | <span data-ttu-id="ece57-149">application/json</span><span class="sxs-lookup"><span data-stu-id="ece57-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ece57-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ece57-150">Request body</span></span>
<span data-ttu-id="ece57-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ece57-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ece57-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ece57-152">Response</span></span>

<span data-ttu-id="ece57-153">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ece57-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ece57-154">Пример</span><span class="sxs-lookup"><span data-stu-id="ece57-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ece57-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ece57-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ece57-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ece57-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="ece57-157">C#</span><span class="sxs-lookup"><span data-stu-id="ece57-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ece57-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ece57-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ece57-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ece57-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ece57-160">Java</span><span class="sxs-lookup"><span data-stu-id="ece57-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ece57-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ece57-161">Response</span></span>
<span data-ttu-id="ece57-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ece57-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->