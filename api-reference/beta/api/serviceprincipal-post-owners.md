---
title: 'servicePrincipal: Добавление владельца'
description: Добавление владельца для субъекта-службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58c994132cbda2159587f0f48ccdce59d79505cb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134178"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="c0c81-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="c0c81-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="c0c81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0c81-105">Добавление владельца для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c0c81-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c81-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c81-106">Permissions</span></span>
<span data-ttu-id="c0c81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c81-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c81-109">Permission type</span></span>      | <span data-ttu-id="c0c81-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0c81-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c81-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0c81-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c81-112">Application.ReadWrite.All и Directory.Read.All, Application.ReadWrite.All и Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0c81-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0c81-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0c81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c81-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c81-114">Not supported.</span></span>    |
|<span data-ttu-id="c0c81-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0c81-115">Application</span></span> | <span data-ttu-id="c0c81-116">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All, Application.ReadWrite.OwnedBy и Directory.ReadWrite.All, Application.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c81-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c0c81-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0c81-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c0c81-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0c81-118">Request headers</span></span>
| <span data-ttu-id="c0c81-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0c81-119">Name</span></span>       | <span data-ttu-id="c0c81-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c81-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c0c81-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0c81-121">Authorization</span></span> | <span data-ttu-id="c0c81-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0c81-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0c81-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0c81-124">Request body</span></span>
<span data-ttu-id="c0c81-125">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c81-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c0c81-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c81-126">Response</span></span>

<span data-ttu-id="c0c81-127">В случае успеха этот метод возвращает код отклика `204 No Content` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0c81-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0c81-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0c81-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c0c81-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0c81-129">Request</span></span>
<span data-ttu-id="c0c81-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c81-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0c81-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c81-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="c0c81-132">C#</span><span class="sxs-lookup"><span data-stu-id="c0c81-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0c81-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0c81-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0c81-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0c81-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0c81-135">Java</span><span class="sxs-lookup"><span data-stu-id="c0c81-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c0c81-136">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c81-136">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="c0c81-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c81-137">Response</span></span>
<span data-ttu-id="c0c81-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0c81-138">The following is an example of the response.</span></span>

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



