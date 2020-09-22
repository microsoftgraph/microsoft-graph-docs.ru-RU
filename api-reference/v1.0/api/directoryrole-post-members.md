---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 04cf9a62fb4929a5f8df53a796374366cf6fd267
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052385"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="644a2-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="644a2-103">Add directory role member</span></span>

<span data-ttu-id="644a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="644a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="644a2-105">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="644a2-105">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="644a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="644a2-106">Permissions</span></span>
<span data-ttu-id="644a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="644a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="644a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="644a2-109">Permission type</span></span>      | <span data-ttu-id="644a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="644a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="644a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="644a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="644a2-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="644a2-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="644a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="644a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="644a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="644a2-114">Not supported.</span></span>    |
|<span data-ttu-id="644a2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="644a2-115">Application</span></span> | <span data-ttu-id="644a2-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="644a2-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="644a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="644a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="644a2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="644a2-118">Request headers</span></span>
| <span data-ttu-id="644a2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="644a2-119">Name</span></span>       | <span data-ttu-id="644a2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="644a2-120">Type</span></span> | <span data-ttu-id="644a2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="644a2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="644a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="644a2-122">Authorization</span></span>  | <span data-ttu-id="644a2-123">string</span><span class="sxs-lookup"><span data-stu-id="644a2-123">string</span></span>  | <span data-ttu-id="644a2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="644a2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="644a2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="644a2-126">Content-Type</span></span>  | <span data-ttu-id="644a2-127">string</span><span class="sxs-lookup"><span data-stu-id="644a2-127">string</span></span>  | <span data-ttu-id="644a2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="644a2-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="644a2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="644a2-129">Request body</span></span>
<span data-ttu-id="644a2-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="644a2-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="644a2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="644a2-131">Response</span></span>

<span data-ttu-id="644a2-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="644a2-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="644a2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="644a2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="644a2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="644a2-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="644a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="644a2-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="644a2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="644a2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="644a2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="644a2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="644a2-138">C#</span><span class="sxs-lookup"><span data-stu-id="644a2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="644a2-139">Java</span><span class="sxs-lookup"><span data-stu-id="644a2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="644a2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="644a2-140">Response</span></span>
<span data-ttu-id="644a2-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="644a2-141">Note: The response object shown here may be truncated for brevity.</span></span> 
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

