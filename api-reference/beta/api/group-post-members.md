---
title: Добавление участника
description: Добавьте члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a6c2cd31cb087d2bea6dcb730a1fd2581ed99552
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002095"
---
# <a name="add-member"></a><span data-ttu-id="b4ccd-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="b4ccd-103">Add member</span></span>

<span data-ttu-id="b4ccd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4ccd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4ccd-105">Добавьте члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="b4ccd-105">Add a member to a Microsoft 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="b4ccd-106">Вы можете добавлять пользователей, участников служб или другие группы.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-106">You can add users, service principals or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="b4ccd-107">Вы можете добавлять пользователей только в группы безопасности и Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ccd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ccd-108">Permissions</span></span>
<span data-ttu-id="b4ccd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ccd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ccd-111">Permission type</span></span>      | <span data-ttu-id="b4ccd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ccd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ccd-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4ccd-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4ccd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ccd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-116">Not supported.</span></span>    |
|<span data-ttu-id="b4ccd-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b4ccd-117">Application</span></span> | <span data-ttu-id="b4ccd-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ccd-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ccd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4ccd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b4ccd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4ccd-120">Request headers</span></span>
| <span data-ttu-id="b4ccd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b4ccd-121">Name</span></span> | <span data-ttu-id="b4ccd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b4ccd-122">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="b4ccd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4ccd-123">Authorization</span></span> | <span data-ttu-id="b4ccd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ccd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4ccd-126">Request body</span></span>
<span data-ttu-id="b4ccd-127">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-127">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b4ccd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ccd-128">Response</span></span>
<span data-ttu-id="b4ccd-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4ccd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b4ccd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4ccd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4ccd-132">Request</span></span>
<span data-ttu-id="b4ccd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4ccd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ccd-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b4ccd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ccd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4ccd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4ccd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b4ccd-137">C#</span><span class="sxs-lookup"><span data-stu-id="b4ccd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b4ccd-138">В тексте запроса `id` добавьте представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [группы](../resources/group.md) , который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="b4ccd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ccd-139">Response</span></span>
<span data-ttu-id="b4ccd-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-140">The following is an example of the response.</span></span>
><span data-ttu-id="b4ccd-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4ccd-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-142">All the properties will be returned from an actual call.</span></span>
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


