---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 45995e2fae9a694d5880ccff6addcfadb8aab28a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613962"
---
# <a name="add-group-owner"></a><span data-ttu-id="5a4ea-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="5a4ea-104">Add group owner</span></span>
<span data-ttu-id="5a4ea-p102">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="5a4ea-107">**Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="5a4ea-108">Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5a4ea-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a4ea-109">Permissions</span></span>
<span data-ttu-id="5a4ea-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a4ea-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a4ea-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a4ea-112">Permission type</span></span>      | <span data-ttu-id="5a4ea-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a4ea-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a4ea-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a4ea-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5a4ea-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a4ea-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a4ea-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a4ea-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a4ea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-117">Not supported.</span></span>    |
|<span data-ttu-id="5a4ea-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="5a4ea-118">Application</span></span> | <span data-ttu-id="5a4ea-119">Group.ReadWrite.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a4ea-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a4ea-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a4ea-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5a4ea-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a4ea-121">Request headers</span></span>
| <span data-ttu-id="5a4ea-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5a4ea-122">Name</span></span>       | <span data-ttu-id="5a4ea-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5a4ea-123">Type</span></span> | <span data-ttu-id="5a4ea-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5a4ea-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a4ea-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a4ea-125">Authorization</span></span>  | <span data-ttu-id="5a4ea-126">string</span><span class="sxs-lookup"><span data-stu-id="5a4ea-126">string</span></span>  | <span data-ttu-id="5a4ea-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a4ea-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a4ea-129">Request body</span></span>
<span data-ttu-id="5a4ea-130">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5a4ea-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4ea-131">Response</span></span>
<span data-ttu-id="5a4ea-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a4ea-134">Пример</span><span class="sxs-lookup"><span data-stu-id="5a4ea-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5a4ea-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a4ea-135">Request</span></span>
<span data-ttu-id="5a4ea-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="5a4ea-137">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="5a4ea-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4ea-138">Response</span></span>
<span data-ttu-id="5a4ea-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-139">The following is an example of the response.</span></span>
><span data-ttu-id="5a4ea-140">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5a4ea-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a4ea-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a4ea-142">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="5a4ea-142">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a4ea-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a4ea-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

