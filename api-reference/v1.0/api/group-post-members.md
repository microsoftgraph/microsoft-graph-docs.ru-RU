---
title: Добавление участника
description: Добавляйте участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c43bded94b1c5fd683c2ca5ca72515a12ce2ec9b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999411"
---
# <a name="add-member"></a><span data-ttu-id="d7593-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="d7593-103">Add member</span></span>
<span data-ttu-id="d7593-104">Добавляйте участника в группу Office 365 или группу безопасности через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="d7593-104">Add a member to an Office 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="d7593-105">Вы можете добавлять пользователей, контакты организации или другие группы.</span><span class="sxs-lookup"><span data-stu-id="d7593-105">You can add users, organizational contacts, or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="d7593-106">Вы можете добавлять пользователей только в группы безопасности и группы Office 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="d7593-106">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7593-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7593-107">Permissions</span></span>
<span data-ttu-id="d7593-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7593-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7593-110">Permission type</span></span>      | <span data-ttu-id="d7593-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7593-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7593-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7593-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7593-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7593-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7593-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7593-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7593-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7593-115">Not supported.</span></span>    |
|<span data-ttu-id="d7593-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7593-116">Application</span></span> | <span data-ttu-id="d7593-117">Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7593-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7593-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7593-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d7593-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7593-119">Request headers</span></span>
| <span data-ttu-id="d7593-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7593-120">Header</span></span>       | <span data-ttu-id="d7593-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7593-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d7593-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7593-122">Authorization</span></span>  | <span data-ttu-id="d7593-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7593-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7593-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7593-125">Content-type</span></span>   | <span data-ttu-id="d7593-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7593-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7593-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7593-128">Request body</span></span>
<span data-ttu-id="d7593-129">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7593-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d7593-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7593-130">Response</span></span>
<span data-ttu-id="d7593-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7593-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7593-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d7593-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d7593-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7593-134">Request</span></span>
<span data-ttu-id="d7593-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7593-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7593-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7593-136">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7593-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7593-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7593-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7593-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="d7593-139">C#</span><span class="sxs-lookup"><span data-stu-id="d7593-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d7593-140">Java</span><span class="sxs-lookup"><span data-stu-id="d7593-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d7593-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7593-141">Response</span></span>
<span data-ttu-id="d7593-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d7593-142">The following is an example of the response.</span></span>

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
