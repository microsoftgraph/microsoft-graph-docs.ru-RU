---
title: Добавление участника
description: Добавляйте участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 06afa7ef7426e65b3b9a83eeb45a9af4353f1342
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123645"
---
# <a name="add-member"></a><span data-ttu-id="0cba3-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="0cba3-103">Add member</span></span>

<span data-ttu-id="0cba3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cba3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cba3-105">Добавляйте участника в группу Office 365 или группу безопасности через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="0cba3-105">Add a member to an Office 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="0cba3-106">Вы можете добавлять пользователей, контакты организации или другие группы.</span><span class="sxs-lookup"><span data-stu-id="0cba3-106">You can add users, organizational contacts, or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="0cba3-107">Вы можете добавлять пользователей только в группы безопасности и группы Office 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="0cba3-107">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cba3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cba3-108">Permissions</span></span>
<span data-ttu-id="0cba3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cba3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cba3-111">Permission type</span></span>      | <span data-ttu-id="0cba3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cba3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cba3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cba3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0cba3-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0cba3-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0cba3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cba3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cba3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cba3-116">Not supported.</span></span>    |
|<span data-ttu-id="0cba3-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0cba3-117">Application</span></span> | <span data-ttu-id="0cba3-118">GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cba3-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cba3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cba3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0cba3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cba3-120">Request headers</span></span>
| <span data-ttu-id="0cba3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cba3-121">Header</span></span>       | <span data-ttu-id="0cba3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0cba3-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="0cba3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cba3-123">Authorization</span></span>  | <span data-ttu-id="0cba3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cba3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0cba3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cba3-126">Content-type</span></span>   | <span data-ttu-id="0cba3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cba3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cba3-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cba3-129">Request body</span></span>
<span data-ttu-id="0cba3-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cba3-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="0cba3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cba3-131">Response</span></span>
<span data-ttu-id="0cba3-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0cba3-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cba3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0cba3-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0cba3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cba3-135">Request</span></span>
<span data-ttu-id="0cba3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cba3-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cba3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cba3-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="0cba3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cba3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cba3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cba3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0cba3-140">C#</span><span class="sxs-lookup"><span data-stu-id="0cba3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cba3-141">Java</span><span class="sxs-lookup"><span data-stu-id="0cba3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0cba3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cba3-142">Response</span></span>
<span data-ttu-id="0cba3-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0cba3-143">The following is an example of the response.</span></span>

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
