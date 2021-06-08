---
title: Добавление участника
description: Добавьте участника в группу Microsoft 365 или группу безопасности через свойство **навигации** членов.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b9dcef9cfa6a362bc56dfaf16df0b64f930d7ea0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787249"
---
# <a name="add-member"></a><span data-ttu-id="fe281-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="fe281-103">Add member</span></span>

<span data-ttu-id="fe281-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe281-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe281-105">Добавьте участника в группу Microsoft 365 или группу безопасности через свойство **навигации** членов.</span><span class="sxs-lookup"><span data-stu-id="fe281-105">Add a member to a Microsoft 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="fe281-106">Можно добавить пользователей, директоров служб или другие группы.</span><span class="sxs-lookup"><span data-stu-id="fe281-106">You can add users, service principals or other groups.</span></span> 

> [!Important]
> + <span data-ttu-id="fe281-107">Вы можете добавлять пользователей только в группы безопасности и группы Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="fe281-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>
> + <span data-ttu-id="fe281-108">Вы не можете добавлять группы безопасности в группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fe281-108">You cannot add security groups to Microsoft 365 groups.</span></span>
> + <span data-ttu-id="fe281-109">Вы не можете добавлять группы Microsoft 365 в группы безопасности или другие группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fe281-109">You cannot add Microsoft 365 groups to security groups or other Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe281-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe281-110">Permissions</span></span>
<span data-ttu-id="fe281-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe281-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe281-113">Permission type</span></span>      | <span data-ttu-id="fe281-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe281-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe281-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe281-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fe281-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe281-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe281-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe281-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe281-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe281-118">Not supported.</span></span>    |
|<span data-ttu-id="fe281-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe281-119">Application</span></span> | <span data-ttu-id="fe281-120">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe281-120">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe281-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe281-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fe281-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe281-122">Request headers</span></span>
| <span data-ttu-id="fe281-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fe281-123">Name</span></span> | <span data-ttu-id="fe281-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fe281-124">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="fe281-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe281-125">Authorization</span></span> | <span data-ttu-id="fe281-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe281-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe281-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe281-128">Request body</span></span>
<span data-ttu-id="fe281-129">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe281-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="fe281-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe281-130">Response</span></span>
<span data-ttu-id="fe281-131">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fe281-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="fe281-132">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe281-132">It does not return anything in the response body.</span></span> <span data-ttu-id="fe281-133">Если объект уже является членом группы, этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="fe281-133">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="fe281-134">Если добавляемый объект не существует, этот метод возвращает код отклика `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="fe281-134">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span> 

## <a name="example"></a><span data-ttu-id="fe281-135">Пример</span><span class="sxs-lookup"><span data-stu-id="fe281-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe281-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe281-136">Request</span></span>
<span data-ttu-id="fe281-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe281-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe281-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe281-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="fe281-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe281-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe281-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe281-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fe281-141">C#</span><span class="sxs-lookup"><span data-stu-id="fe281-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe281-142">Java</span><span class="sxs-lookup"><span data-stu-id="fe281-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fe281-143">В теле запроса устройте JSON-представление объекта `id` [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или группового объекта, который необходимо добавить. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="fe281-143">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="fe281-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe281-144">Response</span></span>
<span data-ttu-id="fe281-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fe281-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


