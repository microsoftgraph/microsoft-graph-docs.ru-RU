---
title: Добавление участника
description: Добавляйте участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 86a50debcddc05eeee41279bd20d3dfd5b12081b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337148"
---
# <a name="add-member"></a><span data-ttu-id="31e5a-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="31e5a-103">Add member</span></span>
<span data-ttu-id="31e5a-104">Добавляйте участника в группу Office 365 или группу безопасности через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="31e5a-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="31e5a-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="31e5a-105">You can add users or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="31e5a-106">В группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="31e5a-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="31e5a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31e5a-107">Permissions</span></span>
<span data-ttu-id="31e5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31e5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31e5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31e5a-110">Permission type</span></span>      | <span data-ttu-id="31e5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31e5a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31e5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31e5a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="31e5a-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31e5a-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31e5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31e5a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31e5a-115">Not supported.</span></span>    |
|<span data-ttu-id="31e5a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="31e5a-116">Application</span></span> | <span data-ttu-id="31e5a-117">Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e5a-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31e5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31e5a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="31e5a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31e5a-119">Request headers</span></span>
| <span data-ttu-id="31e5a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="31e5a-120">Name</span></span>       | <span data-ttu-id="31e5a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="31e5a-121">Type</span></span> | <span data-ttu-id="31e5a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31e5a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="31e5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e5a-123">Authorization</span></span>  | <span data-ttu-id="31e5a-124">string</span><span class="sxs-lookup"><span data-stu-id="31e5a-124">string</span></span>  | <span data-ttu-id="31e5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31e5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31e5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31e5a-127">Request body</span></span>
<span data-ttu-id="31e5a-128">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31e5a-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="31e5a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="31e5a-129">Response</span></span>
<span data-ttu-id="31e5a-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31e5a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e5a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="31e5a-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="31e5a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="31e5a-133">Request</span></span>
<span data-ttu-id="31e5a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31e5a-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="31e5a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="31e5a-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31e5a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31e5a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31e5a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31e5a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="31e5a-138">C#</span><span class="sxs-lookup"><span data-stu-id="31e5a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="31e5a-139">Java</span><span class="sxs-lookup"><span data-stu-id="31e5a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="31e5a-140">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31e5a-140">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="31e5a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="31e5a-141">Response</span></span>
<span data-ttu-id="31e5a-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31e5a-142">The following is an example of the response.</span></span>
><span data-ttu-id="31e5a-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31e5a-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31e5a-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31e5a-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
