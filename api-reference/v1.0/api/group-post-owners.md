---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d141d6f6543f452c681d6d371a2548b12eabc58c
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639914"
---
# <a name="add-group-owner"></a><span data-ttu-id="a1682-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="a1682-104">Add group owner</span></span>

<span data-ttu-id="a1682-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1682-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1682-106">Добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="a1682-106">Add a user to the group's owners.</span></span> <span data-ttu-id="a1682-107">Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="a1682-107">The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="a1682-108">**Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a1682-108">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="a1682-109">Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.</span><span class="sxs-lookup"><span data-stu-id="a1682-109">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a1682-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1682-110">Permissions</span></span>
<span data-ttu-id="a1682-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1682-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1682-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1682-113">Permission type</span></span>      | <span data-ttu-id="a1682-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1682-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1682-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1682-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a1682-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1682-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1682-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1682-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1682-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1682-118">Not supported.</span></span>    |
|<span data-ttu-id="a1682-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="a1682-119">Application</span></span> | <span data-ttu-id="a1682-120">Group.ReadWrite.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1682-120">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1682-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1682-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a1682-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1682-122">Request headers</span></span>
| <span data-ttu-id="a1682-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a1682-123">Name</span></span>       | <span data-ttu-id="a1682-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a1682-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1682-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1682-125">Authorization</span></span>  | <span data-ttu-id="a1682-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1682-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1682-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1682-128">Content-Type</span></span> | <span data-ttu-id="a1682-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1682-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1682-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1682-131">Request body</span></span>
<span data-ttu-id="a1682-132">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1682-132">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a1682-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1682-133">Response</span></span>
<span data-ttu-id="a1682-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1682-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1682-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a1682-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a1682-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1682-137">Request</span></span>
<span data-ttu-id="a1682-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1682-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1682-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1682-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a1682-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1682-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1682-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1682-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a1682-142">C#</span><span class="sxs-lookup"><span data-stu-id="a1682-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1682-143">Java</span><span class="sxs-lookup"><span data-stu-id="a1682-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a1682-144">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1682-144">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="a1682-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1682-145">Response</span></span>
<span data-ttu-id="a1682-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1682-146">The following is an example of the response.</span></span>
><span data-ttu-id="a1682-147">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1682-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a1682-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1682-148">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

