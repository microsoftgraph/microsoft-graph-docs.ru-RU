---
title: Добавление участника
description: Добавление члена в группу безопасности Microsoft 365, группу безопасности или группу безопасности с включенной поддержкой почты с помощью свойства навигации **Members** .
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 74d6ba0443cadf236c6f4af8c0194dfa0cae3d53
ms.sourcegitcommit: 0a979eb1f21ec7834d24c268c24383c3139577ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/05/2020
ms.locfileid: "47400491"
---
# <a name="add-member"></a><span data-ttu-id="cc207-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="cc207-103">Add member</span></span>

<span data-ttu-id="cc207-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc207-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc207-105">Добавление члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="cc207-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="cc207-106">Вы можете добавлять пользователей, организационные контакты, субъекты служб или другие группы.</span><span class="sxs-lookup"><span data-stu-id="cc207-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="cc207-107">Вы можете добавлять пользователей только в группы безопасности и Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="cc207-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc207-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc207-108">Permissions</span></span>

<span data-ttu-id="cc207-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc207-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc207-111">Permission type</span></span>      | <span data-ttu-id="cc207-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc207-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc207-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc207-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cc207-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc207-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc207-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc207-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc207-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc207-116">Not supported.</span></span>    |
|<span data-ttu-id="cc207-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="cc207-117">Application</span></span> | <span data-ttu-id="cc207-118">GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc207-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc207-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc207-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cc207-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc207-120">Request headers</span></span>

| <span data-ttu-id="cc207-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc207-121">Header</span></span>       | <span data-ttu-id="cc207-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc207-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cc207-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc207-123">Authorization</span></span>  | <span data-ttu-id="cc207-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc207-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc207-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc207-126">Content-type</span></span>   | <span data-ttu-id="cc207-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc207-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc207-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc207-129">Request body</span></span>

<span data-ttu-id="cc207-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc207-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cc207-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc207-131">Response</span></span>

<span data-ttu-id="cc207-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cc207-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc207-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc207-134">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="cc207-135">Пример 1: Добавление участника в группу</span><span class="sxs-lookup"><span data-stu-id="cc207-135">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="cc207-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc207-136">Request</span></span>

<span data-ttu-id="cc207-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc207-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

<span data-ttu-id="cc207-138">В тексте запроса добавьте представление идентификатора объекта directoryObject, пользователя или группы, который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc207-138">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="cc207-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc207-139">Response</span></span>

<span data-ttu-id="cc207-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cc207-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="cc207-141">Пример 2: Добавление нескольких участников в группу в едином запросе</span><span class="sxs-lookup"><span data-stu-id="cc207-141">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="cc207-142">В этом примере показано, как добавить несколько членов в группу с поддержкой BIND в операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="cc207-142">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="cc207-143">Обратите внимание, что в один запрос можно добавить до 20 участников.</span><span class="sxs-lookup"><span data-stu-id="cc207-143">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="cc207-144">Операция POST не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc207-144">The POST operation is not supported.</span></span>

#### <a name="request"></a><span data-ttu-id="cc207-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc207-145">Request</span></span>

<span data-ttu-id="cc207-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc207-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{group-id}
Content-type: application/json
Content-length: 30

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```

<span data-ttu-id="cc207-147">В тексте запроса добавьте представление идентификатора объекта directoryObject, пользователя или группы, который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc207-147">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="cc207-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc207-148">Response</span></span>
<span data-ttu-id="cc207-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cc207-149">The following is an example of the response.</span></span>

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
