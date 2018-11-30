---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
ms.openlocfilehash: 8c879430c78cb1d06150bade842addcb4ba0af38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026304"
---
# <a name="add-group-owner"></a><span data-ttu-id="f1e5b-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="f1e5b-104">Add group owner</span></span>
<span data-ttu-id="f1e5b-p102">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1e5b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1e5b-107">Permissions</span></span>
<span data-ttu-id="f1e5b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1e5b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e5b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1e5b-110">Permission type</span></span>      | <span data-ttu-id="f1e5b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1e5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1e5b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1e5b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1e5b-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1e5b-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1e5b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1e5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1e5b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-115">Not supported.</span></span>    |
|<span data-ttu-id="f1e5b-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f1e5b-116">Application</span></span> | <span data-ttu-id="f1e5b-117">Group.ReadWrite.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e5b-117">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1e5b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1e5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f1e5b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1e5b-119">Request headers</span></span>
| <span data-ttu-id="f1e5b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f1e5b-120">Name</span></span>       | <span data-ttu-id="f1e5b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f1e5b-121">Type</span></span> | <span data-ttu-id="f1e5b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f1e5b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1e5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e5b-123">Authorization</span></span>  | <span data-ttu-id="f1e5b-124">string</span><span class="sxs-lookup"><span data-stu-id="f1e5b-124">string</span></span>  | <span data-ttu-id="f1e5b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1e5b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1e5b-127">Request body</span></span>
<span data-ttu-id="f1e5b-128">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-128">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f1e5b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1e5b-129">Response</span></span>
<span data-ttu-id="f1e5b-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e5b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f1e5b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f1e5b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1e5b-133">Request</span></span>
<span data-ttu-id="f1e5b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="f1e5b-135">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-135">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="f1e5b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1e5b-136">Response</span></span>
<span data-ttu-id="f1e5b-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-137">The following is an example of the response.</span></span>
><span data-ttu-id="f1e5b-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1e5b-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1e5b-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
