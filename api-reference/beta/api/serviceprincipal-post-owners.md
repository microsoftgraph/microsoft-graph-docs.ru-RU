---
title: 'servicePrincipal: Добавление владельца'
description: Добавьте владельца для субъекта службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 555d2341d68ff48d34c3bf56b112b6a7ab501c9d
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382729"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="667f2-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="667f2-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="667f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="667f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="667f2-105">Добавьте владельца для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="667f2-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="667f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="667f2-106">Permissions</span></span>
<span data-ttu-id="667f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="667f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="667f2-109">Permission type</span></span>      | <span data-ttu-id="667f2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="667f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="667f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="667f2-112">Application. ReadWrite. ALL и Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="667f2-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="667f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="667f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667f2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667f2-114">Not supported.</span></span>    |
|<span data-ttu-id="667f2-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="667f2-115">Application</span></span> | <span data-ttu-id="667f2-116">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL, Application. ReadWrite. Овнедби и Directory. ReadWrite. ALL, Application. ReadWrite. ALL и Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="667f2-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="667f2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="667f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="667f2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="667f2-118">Request headers</span></span>
| <span data-ttu-id="667f2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="667f2-119">Name</span></span>       | <span data-ttu-id="667f2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="667f2-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="667f2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="667f2-121">Authorization</span></span> | <span data-ttu-id="667f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667f2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="667f2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="667f2-124">Request body</span></span>
<span data-ttu-id="667f2-125">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667f2-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="667f2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="667f2-126">Response</span></span>

<span data-ttu-id="667f2-127">В случае успеха этот метод возвращает код отклика `204 No Content` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="667f2-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="667f2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="667f2-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="667f2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="667f2-129">Request</span></span>
<span data-ttu-id="667f2-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="667f2-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="667f2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="667f2-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="667f2-132">C#</span><span class="sxs-lookup"><span data-stu-id="667f2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="667f2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="667f2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="667f2-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="667f2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="667f2-135">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667f2-135">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="667f2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="667f2-136">Response</span></span>
<span data-ttu-id="667f2-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="667f2-137">The following is an example of the response.</span></span>

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
