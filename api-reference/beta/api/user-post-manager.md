---
title: Назначение руководителя
description: С помощью этого API можно назначить руководителя пользователю.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8d545b1aa606ae1c87391138347d6d4018a5d6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987530"
---
# <a name="assign-a-manager"></a><span data-ttu-id="bd2db-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="bd2db-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd2db-104">С помощью этого API можно назначить руководителя пользователю.</span><span class="sxs-lookup"><span data-stu-id="bd2db-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="bd2db-105">Примечание. Назначать подчиненных невозможно. Вместо этого используйте данный API.</span><span class="sxs-lookup"><span data-stu-id="bd2db-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd2db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd2db-106">Permissions</span></span>
<span data-ttu-id="bd2db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd2db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd2db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd2db-109">Permission type</span></span>      | <span data-ttu-id="bd2db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd2db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd2db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd2db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bd2db-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd2db-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd2db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd2db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd2db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd2db-114">Not supported.</span></span>    |
|<span data-ttu-id="bd2db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd2db-115">Application</span></span> | <span data-ttu-id="bd2db-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd2db-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd2db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd2db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bd2db-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd2db-118">Request headers</span></span>
| <span data-ttu-id="bd2db-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bd2db-119">Name</span></span>       | <span data-ttu-id="bd2db-120">Тип</span><span class="sxs-lookup"><span data-stu-id="bd2db-120">Type</span></span> | <span data-ttu-id="bd2db-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bd2db-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bd2db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd2db-122">Authorization</span></span>  | <span data-ttu-id="bd2db-123">string</span><span class="sxs-lookup"><span data-stu-id="bd2db-123">string</span></span>  | <span data-ttu-id="bd2db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd2db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd2db-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd2db-126">Request body</span></span>
<span data-ttu-id="bd2db-127">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd2db-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="bd2db-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd2db-128">Response</span></span>

<span data-ttu-id="bd2db-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bd2db-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd2db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bd2db-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd2db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd2db-132">Request</span></span>
<span data-ttu-id="bd2db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd2db-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd2db-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd2db-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_for_user"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd2db-135">C#</span><span class="sxs-lookup"><span data-stu-id="bd2db-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-for-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd2db-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd2db-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-for-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd2db-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bd2db-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-for-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bd2db-138">Java</span><span class="sxs-lookup"><span data-stu-id="bd2db-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-for-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bd2db-139">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd2db-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="bd2db-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd2db-140">Response</span></span>
<span data-ttu-id="bd2db-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd2db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
