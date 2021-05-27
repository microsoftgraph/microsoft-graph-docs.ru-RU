---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7736c3ae73cc18436387b4d9e90813daadb19957
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681370"
---
# <a name="add-group-owner"></a><span data-ttu-id="37785-103">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="37785-103">Add group owner</span></span>

<span data-ttu-id="37785-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37785-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37785-p101">Добавление пользователя или субъекта-службы к владельцам группы. Владельцы — это группа пользователей или субъектов-служб, которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="37785-p101">Add a user or service principal to the group's owners. The owners are a set of users or service principals who are allowed to modify the group object.</span></span>

><span data-ttu-id="37785-107">**Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="37785-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="37785-108">Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.</span><span class="sxs-lookup"><span data-stu-id="37785-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="37785-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37785-109">Permissions</span></span>
<span data-ttu-id="37785-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37785-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37785-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37785-112">Permission type</span></span>      | <span data-ttu-id="37785-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37785-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37785-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37785-114">Delegated (work or school account)</span></span> | <span data-ttu-id="37785-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37785-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37785-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37785-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37785-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37785-117">Not supported.</span></span>    |
|<span data-ttu-id="37785-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37785-118">Application</span></span> | <span data-ttu-id="37785-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37785-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37785-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37785-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="37785-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37785-121">Request headers</span></span>
| <span data-ttu-id="37785-122">Имя</span><span class="sxs-lookup"><span data-stu-id="37785-122">Name</span></span>       | <span data-ttu-id="37785-123">Описание</span><span class="sxs-lookup"><span data-stu-id="37785-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37785-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37785-124">Authorization</span></span>  | <span data-ttu-id="37785-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37785-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37785-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37785-127">Content-type</span></span> | <span data-ttu-id="37785-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37785-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37785-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37785-130">Request body</span></span>
<span data-ttu-id="37785-131">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37785-131">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="37785-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="37785-132">Response</span></span>
<span data-ttu-id="37785-133">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37785-133">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="37785-134">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37785-134">It does not return anything in the response body.</span></span> <span data-ttu-id="37785-135">Если объект уже является членом группы, этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="37785-135">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="37785-136">Если добавляемый объект не существует, этот метод возвращает код отклика `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="37785-136">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="example"></a><span data-ttu-id="37785-137">Пример</span><span class="sxs-lookup"><span data-stu-id="37785-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="37785-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="37785-138">Request</span></span>
<span data-ttu-id="37785-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37785-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37785-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="37785-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="37785-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37785-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37785-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37785-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="37785-143">C#</span><span class="sxs-lookup"><span data-stu-id="37785-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37785-144">Java</span><span class="sxs-lookup"><span data-stu-id="37785-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="37785-145">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37785-145">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="37785-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="37785-146">Response</span></span>
<span data-ttu-id="37785-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="37785-147">The following is an example of the response.</span></span>
><span data-ttu-id="37785-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37785-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


