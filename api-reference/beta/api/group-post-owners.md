---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f71d683baf1340143ae82801461e2efb7334811e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002060"
---
# <a name="add-group-owner"></a><span data-ttu-id="dd8cc-103">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="dd8cc-103">Add group owner</span></span>

<span data-ttu-id="dd8cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd8cc-105">Добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-105">Add a user to the group's owners.</span></span> <span data-ttu-id="dd8cc-106">Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-106">The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="dd8cc-107">**Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="dd8cc-108">Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dd8cc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd8cc-109">Permissions</span></span>
<span data-ttu-id="dd8cc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd8cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd8cc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd8cc-112">Permission type</span></span>      | <span data-ttu-id="dd8cc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd8cc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd8cc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd8cc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dd8cc-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd8cc-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd8cc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd8cc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd8cc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-117">Not supported.</span></span>    |
|<span data-ttu-id="dd8cc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd8cc-118">Application</span></span> | <span data-ttu-id="dd8cc-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd8cc-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd8cc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd8cc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dd8cc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd8cc-121">Request headers</span></span>
| <span data-ttu-id="dd8cc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dd8cc-122">Name</span></span>       | <span data-ttu-id="dd8cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dd8cc-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd8cc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd8cc-124">Authorization</span></span>  | <span data-ttu-id="dd8cc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd8cc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd8cc-127">Content-type</span></span> | <span data-ttu-id="dd8cc-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd8cc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd8cc-130">Request body</span></span>
<span data-ttu-id="dd8cc-131">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-131">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="dd8cc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd8cc-132">Response</span></span>
<span data-ttu-id="dd8cc-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd8cc-135">Пример</span><span class="sxs-lookup"><span data-stu-id="dd8cc-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dd8cc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd8cc-136">Request</span></span>
<span data-ttu-id="dd8cc-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd8cc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd8cc-138">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="dd8cc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd8cc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd8cc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd8cc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dd8cc-141">C#</span><span class="sxs-lookup"><span data-stu-id="dd8cc-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dd8cc-142">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-142">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="dd8cc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd8cc-143">Response</span></span>
<span data-ttu-id="dd8cc-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-144">The following is an example of the response.</span></span>
><span data-ttu-id="dd8cc-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd8cc-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd8cc-146">All the properties will be returned from an actual call.</span></span>
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


