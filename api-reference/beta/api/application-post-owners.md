---
title: Добавление владельца
description: Этот API используется для добавления владельца в приложение.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ee3483bec89eef7651ce415fb9506e27b400b60f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129095"
---
# <a name="add-owner"></a><span data-ttu-id="57823-103">Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="57823-103">Add owner</span></span>

<span data-ttu-id="57823-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57823-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57823-105">Этот API используется для добавления владельца в приложение путем добавления в коллекцию владельцев.</span><span class="sxs-lookup"><span data-stu-id="57823-105">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="57823-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57823-106">Permissions</span></span>
<span data-ttu-id="57823-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57823-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57823-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57823-109">Permission type</span></span>      | <span data-ttu-id="57823-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57823-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57823-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57823-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="57823-112">Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57823-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57823-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57823-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57823-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57823-114">Not supported.</span></span>    |
|<span data-ttu-id="57823-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57823-115">Application</span></span> | <span data-ttu-id="57823-116">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57823-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57823-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57823-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="57823-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57823-118">Request headers</span></span>
| <span data-ttu-id="57823-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57823-119">Name</span></span> | <span data-ttu-id="57823-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57823-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="57823-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57823-121">Authorization</span></span> | <span data-ttu-id="57823-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57823-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57823-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57823-124">Request body</span></span>
<span data-ttu-id="57823-125">В теле запроса укавите идентификатор объекта каталога, который должен быть назначен владельцем.</span><span class="sxs-lookup"><span data-stu-id="57823-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="57823-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="57823-126">Response</span></span>

<span data-ttu-id="57823-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57823-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="57823-128">Пример</span><span class="sxs-lookup"><span data-stu-id="57823-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="57823-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="57823-129">Request</span></span>
<span data-ttu-id="57823-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57823-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57823-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="57823-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="57823-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57823-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="57823-133">C#</span><span class="sxs-lookup"><span data-stu-id="57823-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57823-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57823-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57823-135">Java</span><span class="sxs-lookup"><span data-stu-id="57823-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="57823-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="57823-136">Response</span></span>

<span data-ttu-id="57823-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57823-137">The following is an example of the response.</span></span>

><span data-ttu-id="57823-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57823-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



