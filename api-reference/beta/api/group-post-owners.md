---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c1870b3e772c82e4e62abc83dee16530988e35cb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420079"
---
# <a name="add-group-owner"></a><span data-ttu-id="a47d2-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="a47d2-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a47d2-p102">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="a47d2-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="a47d2-107">**Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a47d2-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="a47d2-108">Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.</span><span class="sxs-lookup"><span data-stu-id="a47d2-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a47d2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a47d2-109">Permissions</span></span>
<span data-ttu-id="a47d2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a47d2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a47d2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a47d2-112">Permission type</span></span>      | <span data-ttu-id="a47d2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a47d2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a47d2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a47d2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a47d2-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a47d2-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a47d2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a47d2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a47d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a47d2-117">Not supported.</span></span>    |
|<span data-ttu-id="a47d2-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="a47d2-118">Application</span></span> | <span data-ttu-id="a47d2-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a47d2-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a47d2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a47d2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a47d2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a47d2-121">Request headers</span></span>
| <span data-ttu-id="a47d2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a47d2-122">Name</span></span>       | <span data-ttu-id="a47d2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a47d2-123">Type</span></span> | <span data-ttu-id="a47d2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a47d2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a47d2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a47d2-125">Authorization</span></span>  | <span data-ttu-id="a47d2-126">string</span><span class="sxs-lookup"><span data-stu-id="a47d2-126">string</span></span>  | <span data-ttu-id="a47d2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a47d2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a47d2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a47d2-129">Request body</span></span>
<span data-ttu-id="a47d2-130">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a47d2-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a47d2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a47d2-131">Response</span></span>
<span data-ttu-id="a47d2-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a47d2-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a47d2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a47d2-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a47d2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a47d2-135">Request</span></span>
<span data-ttu-id="a47d2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a47d2-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a47d2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a47d2-137">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a47d2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a47d2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a47d2-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a47d2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="a47d2-140">C#</span><span class="sxs-lookup"><span data-stu-id="a47d2-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a47d2-141">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a47d2-141">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="a47d2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a47d2-142">Response</span></span>
<span data-ttu-id="a47d2-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a47d2-143">The following is an example of the response.</span></span>
><span data-ttu-id="a47d2-144">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a47d2-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a47d2-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a47d2-145">All the properties will be returned from an actual call.</span></span>
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
