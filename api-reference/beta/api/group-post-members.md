---
title: Добавление участника
description: Добавьте члена в группу Office 365 или группу безопасности с помощью свойства навигации **Members** .
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 64ddd8881cb210a06fff35f0d30d1e3a78c85d81
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323250"
---
# <a name="add-member"></a><span data-ttu-id="702fe-103">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="702fe-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="702fe-104">Добавьте члена в группу Office 365 или группу безопасности с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="702fe-104">Add a member to an Office 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="702fe-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="702fe-105">You can add users or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="702fe-106">Вы можете добавлять только пользователей в группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="702fe-106">You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="702fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="702fe-107">Permissions</span></span>
<span data-ttu-id="702fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="702fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="702fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="702fe-110">Permission type</span></span>      | <span data-ttu-id="702fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="702fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="702fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="702fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="702fe-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="702fe-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="702fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="702fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="702fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="702fe-115">Not supported.</span></span>    |
|<span data-ttu-id="702fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="702fe-116">Application</span></span> | <span data-ttu-id="702fe-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="702fe-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="702fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="702fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="702fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="702fe-119">Request headers</span></span>
| <span data-ttu-id="702fe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="702fe-120">Name</span></span> | <span data-ttu-id="702fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="702fe-121">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="702fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="702fe-122">Authorization</span></span> | <span data-ttu-id="702fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="702fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="702fe-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="702fe-125">Request body</span></span>
<span data-ttu-id="702fe-126">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="702fe-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="702fe-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="702fe-127">Response</span></span>
<span data-ttu-id="702fe-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="702fe-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="702fe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="702fe-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="702fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="702fe-131">Request</span></span>
<span data-ttu-id="702fe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="702fe-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="702fe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="702fe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="702fe-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="702fe-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="702fe-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="702fe-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="702fe-136">C#</span><span class="sxs-lookup"><span data-stu-id="702fe-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="702fe-137">Java</span><span class="sxs-lookup"><span data-stu-id="702fe-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="702fe-138">В тексте запроса добавьте `id` представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [группы](../resources/group.md) , который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="702fe-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="702fe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="702fe-139">Response</span></span>
<span data-ttu-id="702fe-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="702fe-140">The following is an example of the response.</span></span>
><span data-ttu-id="702fe-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="702fe-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="702fe-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="702fe-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
