---
title: Добавление участника
description: Добавляйте участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a3ccacd1ebb1985cd09de31f9568df86660451af
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778432"
---
# <a name="add-member"></a><span data-ttu-id="9d72c-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="9d72c-103">Add member</span></span>
<span data-ttu-id="9d72c-104">Добавляйте участника в группу Office 365 или группу безопасности через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="9d72c-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="9d72c-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="9d72c-105">You can add users or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="9d72c-106">В группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="9d72c-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d72c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d72c-107">Permissions</span></span>
<span data-ttu-id="9d72c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d72c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d72c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d72c-110">Permission type</span></span>      | <span data-ttu-id="9d72c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d72c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d72c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d72c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d72c-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d72c-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d72c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d72c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d72c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d72c-115">Not supported.</span></span>    |
|<span data-ttu-id="9d72c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9d72c-116">Application</span></span> | <span data-ttu-id="9d72c-117">Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d72c-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d72c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d72c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9d72c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d72c-119">Request headers</span></span>
| <span data-ttu-id="9d72c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9d72c-120">Name</span></span>       | <span data-ttu-id="9d72c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9d72c-121">Type</span></span> | <span data-ttu-id="9d72c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9d72c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d72c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d72c-123">Authorization</span></span>  | <span data-ttu-id="9d72c-124">string</span><span class="sxs-lookup"><span data-stu-id="9d72c-124">string</span></span>  | <span data-ttu-id="9d72c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d72c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d72c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d72c-127">Request body</span></span>
<span data-ttu-id="9d72c-128">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d72c-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9d72c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d72c-129">Response</span></span>
<span data-ttu-id="9d72c-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9d72c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d72c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9d72c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9d72c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d72c-133">Request</span></span>
<span data-ttu-id="9d72c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d72c-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d72c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d72c-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d72c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d72c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d72c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d72c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9d72c-138">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d72c-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="9d72c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d72c-139">Response</span></span>
<span data-ttu-id="9d72c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d72c-140">The following is an example of the response.</span></span>
><span data-ttu-id="9d72c-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d72c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d72c-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d72c-142">All the properties will be returned from an actual call.</span></span>
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
