---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6c0e92b0286f1efdddc962f478cfc277d08c493
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936855"
---
# <a name="list-deleted-items"></a><span data-ttu-id="202f1-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="202f1-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="202f1-104">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="202f1-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="202f1-105">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="202f1-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="202f1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="202f1-106">Permissions</span></span>
<span data-ttu-id="202f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="202f1-109">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="202f1-109">For applications:</span></span>

|<span data-ttu-id="202f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202f1-110">Permission type</span></span>      | <span data-ttu-id="202f1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="202f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="202f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="202f1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="202f1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="202f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202f1-115">Not supported.</span></span>    |
|<span data-ttu-id="202f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202f1-116">Application</span></span> | <span data-ttu-id="202f1-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="202f1-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="202f1-118">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="202f1-118">For users:</span></span>

|<span data-ttu-id="202f1-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202f1-119">Permission type</span></span>      | <span data-ttu-id="202f1-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="202f1-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="202f1-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202f1-121">Delegated (work or school account)</span></span> | <span data-ttu-id="202f1-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="202f1-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="202f1-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202f1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202f1-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202f1-124">Not supported.</span></span> |
|<span data-ttu-id="202f1-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202f1-125">Application</span></span> | <span data-ttu-id="202f1-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="202f1-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="202f1-127">Для групп:</span><span class="sxs-lookup"><span data-stu-id="202f1-127">For groups:</span></span>

|<span data-ttu-id="202f1-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202f1-128">Permission type</span></span>      | <span data-ttu-id="202f1-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="202f1-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="202f1-130">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202f1-130">Delegated (work or school account)</span></span> | <span data-ttu-id="202f1-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="202f1-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="202f1-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202f1-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202f1-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202f1-133">Not supported.</span></span>    |
|<span data-ttu-id="202f1-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202f1-134">Application</span></span> | <span data-ttu-id="202f1-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="202f1-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="202f1-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="202f1-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="202f1-137">Этот API в настоящее время поддерживает получение типов объектов приложений (Microsoft. Graph. Application), групп (Microsoft. Graph. Group) или пользователей (Microsoft. Graph. User) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="202f1-137">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="202f1-138">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="202f1-138">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="202f1-139">Вызов GET /directory/deleteditems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202f1-139">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="202f1-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="202f1-140">Optional query parameters</span></span>
<span data-ttu-id="202f1-141">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="202f1-141">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="202f1-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="202f1-142">Request headers</span></span>
| <span data-ttu-id="202f1-143">Имя</span><span class="sxs-lookup"><span data-stu-id="202f1-143">Name</span></span>      |<span data-ttu-id="202f1-144">Описание</span><span class="sxs-lookup"><span data-stu-id="202f1-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="202f1-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="202f1-145">Authorization</span></span>  | <span data-ttu-id="202f1-146">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="202f1-146">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="202f1-147">Accept</span><span class="sxs-lookup"><span data-stu-id="202f1-147">Accept</span></span>  | <span data-ttu-id="202f1-148">application/json</span><span class="sxs-lookup"><span data-stu-id="202f1-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="202f1-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="202f1-149">Request body</span></span>
<span data-ttu-id="202f1-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="202f1-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="202f1-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="202f1-151">Response</span></span>

<span data-ttu-id="202f1-152">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="202f1-152">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="202f1-153">Пример</span><span class="sxs-lookup"><span data-stu-id="202f1-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="202f1-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="202f1-154">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="202f1-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="202f1-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="202f1-156">C#</span><span class="sxs-lookup"><span data-stu-id="202f1-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="202f1-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="202f1-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="202f1-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="202f1-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="202f1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="202f1-159">Response</span></span>
<span data-ttu-id="202f1-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="202f1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
