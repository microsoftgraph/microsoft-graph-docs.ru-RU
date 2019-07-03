---
title: Добавление участника
description: С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9ed8ef9f054a9d0c7a69ab21067664b7fd2f6853
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440262"
---
# <a name="add-member"></a><span data-ttu-id="5d1f7-103">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="5d1f7-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d1f7-104">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="5d1f7-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-105">You can add users or other groups.</span></span> <span data-ttu-id="5d1f7-106">Важно! В Группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d1f7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d1f7-107">Permissions</span></span>
<span data-ttu-id="5d1f7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d1f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d1f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d1f7-110">Permission type</span></span>      | <span data-ttu-id="5d1f7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d1f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d1f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d1f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5d1f7-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d1f7-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d1f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d1f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d1f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-115">Not supported.</span></span>    |
|<span data-ttu-id="5d1f7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5d1f7-116">Application</span></span> | <span data-ttu-id="5d1f7-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1f7-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d1f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d1f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5d1f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d1f7-119">Request headers</span></span>
| <span data-ttu-id="5d1f7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5d1f7-120">Name</span></span>       | <span data-ttu-id="5d1f7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5d1f7-121">Type</span></span> | <span data-ttu-id="5d1f7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5d1f7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d1f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d1f7-123">Authorization</span></span>  | <span data-ttu-id="5d1f7-124">string</span><span class="sxs-lookup"><span data-stu-id="5d1f7-124">string</span></span>  | <span data-ttu-id="5d1f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d1f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d1f7-127">Request body</span></span>
<span data-ttu-id="5d1f7-128">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5d1f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d1f7-129">Response</span></span>
<span data-ttu-id="5d1f7-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d1f7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5d1f7-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5d1f7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d1f7-133">Request</span></span>
<span data-ttu-id="5d1f7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5d1f7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d1f7-135">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d1f7-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d1f7-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5d1f7-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5d1f7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5d1f7-138">В тексте запроса добавьте `id` представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [группы](../resources/group.md) , который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="5d1f7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d1f7-139">Response</span></span>
<span data-ttu-id="5d1f7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-140">The following is an example of the response.</span></span>
><span data-ttu-id="5d1f7-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d1f7-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-142">All the properties will be returned from an actual call.</span></span>
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
