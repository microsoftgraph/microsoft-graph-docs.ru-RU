---
title: Добавление владельца
description: Используйте этот API, чтобы добавить владельца в приложение.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6299f481c3cfcad1eb62cd1460f7f0d2b071e62
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107075"
---
# <a name="add-owner"></a><span data-ttu-id="07e00-103">Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="07e00-103">Add owner</span></span>

<span data-ttu-id="07e00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e00-105">Используйте этот API, чтобы добавить владельца в приложение путем публикации в коллекции Owners.</span><span class="sxs-lookup"><span data-stu-id="07e00-105">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="07e00-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07e00-106">Permissions</span></span>
<span data-ttu-id="07e00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07e00-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07e00-109">Permission type</span></span>      | <span data-ttu-id="07e00-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07e00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07e00-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07e00-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="07e00-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07e00-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07e00-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07e00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07e00-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07e00-114">Not supported.</span></span>    |
|<span data-ttu-id="07e00-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07e00-115">Application</span></span> | <span data-ttu-id="07e00-116">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="07e00-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07e00-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07e00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="07e00-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07e00-118">Request headers</span></span>
| <span data-ttu-id="07e00-119">Имя</span><span class="sxs-lookup"><span data-stu-id="07e00-119">Name</span></span> | <span data-ttu-id="07e00-120">Описание</span><span class="sxs-lookup"><span data-stu-id="07e00-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="07e00-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07e00-121">Authorization</span></span> | <span data-ttu-id="07e00-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07e00-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07e00-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07e00-124">Request body</span></span>
<span data-ttu-id="07e00-125">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="07e00-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="07e00-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="07e00-126">Response</span></span>

<span data-ttu-id="07e00-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07e00-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07e00-128">Пример</span><span class="sxs-lookup"><span data-stu-id="07e00-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="07e00-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="07e00-129">Request</span></span>
<span data-ttu-id="07e00-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07e00-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07e00-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="07e00-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascript"></a>[<span data-ttu-id="07e00-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07e00-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="07e00-133">C#</span><span class="sxs-lookup"><span data-stu-id="07e00-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07e00-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07e00-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="07e00-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="07e00-135">Response</span></span>

<span data-ttu-id="07e00-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07e00-136">The following is an example of the response.</span></span>

><span data-ttu-id="07e00-137">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="07e00-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07e00-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07e00-138">All the properties will be returned from an actual call.</span></span>

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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
