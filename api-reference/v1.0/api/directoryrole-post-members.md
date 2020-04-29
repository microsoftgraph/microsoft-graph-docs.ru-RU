---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c5f958f4543c985b6ecf8684080d261ed874028
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181380"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="581f3-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="581f3-103">Add directory role member</span></span>

<span data-ttu-id="581f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="581f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="581f3-105">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="581f3-105">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="581f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="581f3-106">Permissions</span></span>
<span data-ttu-id="581f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="581f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="581f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="581f3-109">Permission type</span></span>      | <span data-ttu-id="581f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="581f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="581f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="581f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="581f3-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="581f3-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="581f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="581f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="581f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="581f3-114">Not supported.</span></span>    |
|<span data-ttu-id="581f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="581f3-115">Application</span></span> | <span data-ttu-id="581f3-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="581f3-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="581f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="581f3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="581f3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="581f3-118">Request headers</span></span>
| <span data-ttu-id="581f3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="581f3-119">Name</span></span>       | <span data-ttu-id="581f3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="581f3-120">Type</span></span> | <span data-ttu-id="581f3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="581f3-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="581f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="581f3-122">Authorization</span></span>  | <span data-ttu-id="581f3-123">string</span><span class="sxs-lookup"><span data-stu-id="581f3-123">string</span></span>  | <span data-ttu-id="581f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="581f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="581f3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="581f3-126">Content-Type</span></span>  | <span data-ttu-id="581f3-127">string</span><span class="sxs-lookup"><span data-stu-id="581f3-127">string</span></span>  | <span data-ttu-id="581f3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="581f3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="581f3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="581f3-129">Request body</span></span>
<span data-ttu-id="581f3-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="581f3-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="581f3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="581f3-131">Response</span></span>

<span data-ttu-id="581f3-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="581f3-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="581f3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="581f3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="581f3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="581f3-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="581f3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="581f3-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="581f3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="581f3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="581f3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="581f3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="581f3-138">C#</span><span class="sxs-lookup"><span data-stu-id="581f3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="581f3-139">Java</span><span class="sxs-lookup"><span data-stu-id="581f3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="581f3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="581f3-140">Response</span></span>
<span data-ttu-id="581f3-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="581f3-141">Note: The response object shown here may be truncated for brevity.</span></span> 
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
