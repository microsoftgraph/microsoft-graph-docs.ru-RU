---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06338f2dfbed00f3150a9278cbc9f4a21a59b5c1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891072"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="b44be-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="b44be-103">Add directory role member</span></span>

<span data-ttu-id="b44be-104">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="b44be-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="b44be-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b44be-105">Permissions</span></span>
<span data-ttu-id="b44be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b44be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44be-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b44be-108">Permission type</span></span>      | <span data-ttu-id="b44be-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b44be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b44be-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b44be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b44be-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b44be-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b44be-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b44be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b44be-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b44be-113">Not supported.</span></span>    |
|<span data-ttu-id="b44be-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b44be-114">Application</span></span> | <span data-ttu-id="b44be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b44be-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b44be-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b44be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="b44be-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b44be-117">Request headers</span></span>
| <span data-ttu-id="b44be-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b44be-118">Name</span></span>       | <span data-ttu-id="b44be-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b44be-119">Type</span></span> | <span data-ttu-id="b44be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b44be-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b44be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b44be-121">Authorization</span></span>  | <span data-ttu-id="b44be-122">string</span><span class="sxs-lookup"><span data-stu-id="b44be-122">string</span></span>  | <span data-ttu-id="b44be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b44be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b44be-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b44be-125">Content-Type</span></span>  | <span data-ttu-id="b44be-126">string</span><span class="sxs-lookup"><span data-stu-id="b44be-126">string</span></span>  | <span data-ttu-id="b44be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b44be-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b44be-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b44be-128">Request body</span></span>
<span data-ttu-id="b44be-129">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b44be-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b44be-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b44be-130">Response</span></span>

<span data-ttu-id="b44be-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b44be-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b44be-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b44be-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b44be-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b44be-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b44be-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b44be-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b44be-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="b44be-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b44be-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b44be-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="b44be-137">C#</span><span class="sxs-lookup"><span data-stu-id="b44be-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b44be-138">Java</span><span class="sxs-lookup"><span data-stu-id="b44be-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b44be-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b44be-139">Response</span></span>
<span data-ttu-id="b44be-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b44be-140">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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
