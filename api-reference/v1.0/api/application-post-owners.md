---
title: Добавление владельца
description: Добавление владельца в приложение.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2623453363ae26cce4d1912f8492b3d55b4479e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518863"
---
# <a name="add-owner"></a><span data-ttu-id="e4ee3-103">Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="e4ee3-103">Add owner</span></span>

<span data-ttu-id="e4ee3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4ee3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4ee3-105">Добавление владельца в [приложение](../resources/application.md) путем публикации в коллекции Owners.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-105">Add an owner to an [application](../resources/application.md) by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4ee3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4ee3-106">Permissions</span></span>
<span data-ttu-id="e4ee3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4ee3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4ee3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4ee3-109">Permission type</span></span>      | <span data-ttu-id="e4ee3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4ee3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4ee3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4ee3-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e4ee3-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4ee3-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4ee3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4ee3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4ee3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-114">Not supported.</span></span>    |
|<span data-ttu-id="e4ee3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4ee3-115">Application</span></span> | <span data-ttu-id="e4ee3-116">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="e4ee3-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4ee3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4ee3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="e4ee3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4ee3-118">Request headers</span></span>
| <span data-ttu-id="e4ee3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e4ee3-119">Name</span></span> | <span data-ttu-id="e4ee3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4ee3-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="e4ee3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4ee3-121">Authorization</span></span> | <span data-ttu-id="e4ee3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4ee3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4ee3-124">Request body</span></span>
<span data-ttu-id="e4ee3-125">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="e4ee3-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4ee3-126">Response</span></span>

<span data-ttu-id="e4ee3-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4ee3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e4ee3-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4ee3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4ee3-129">Request</span></span>
<span data-ttu-id="e4ee3-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-130">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4ee3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4ee3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="e4ee3-132">C#</span><span class="sxs-lookup"><span data-stu-id="e4ee3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4ee3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4ee3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4ee3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4ee3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4ee3-135">Java</span><span class="sxs-lookup"><span data-stu-id="e4ee3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4ee3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4ee3-136">Response</span></span>

<span data-ttu-id="e4ee3-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-137">The following is an example of the response.</span></span>

><span data-ttu-id="e4ee3-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e4ee3-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4ee3-139">All the properties will be returned from an actual call.</span></span>

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
