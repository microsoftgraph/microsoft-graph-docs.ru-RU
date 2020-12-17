---
title: 'servicePrincipal: Добавление владельца'
description: Используйте этот API для добавления владельца для субъекта-службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8a1c063046d9d0deab8acfec7a78d9c28507a9fa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980075"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="e1426-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="e1426-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="e1426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1426-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1426-105">Используйте этот API для добавления владельца для [субъекта-службы](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="e1426-105">Use this API to add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1426-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1426-106">Permissions</span></span>
<span data-ttu-id="e1426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1426-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1426-109">Permission type</span></span>      | <span data-ttu-id="e1426-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1426-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1426-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1426-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1426-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1426-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1426-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1426-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1426-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1426-114">Not supported.</span></span>    |
|<span data-ttu-id="e1426-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1426-115">Application</span></span> | <span data-ttu-id="e1426-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1426-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1426-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1426-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="e1426-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1426-118">Request headers</span></span>
| <span data-ttu-id="e1426-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e1426-119">Name</span></span>       | <span data-ttu-id="e1426-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e1426-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e1426-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1426-121">Authorization</span></span> | <span data-ttu-id="e1426-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1426-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1426-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1426-124">Content-Type</span></span> | <span data-ttu-id="e1426-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1426-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1426-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1426-127">Request body</span></span>
<span data-ttu-id="e1426-128">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1426-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1426-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1426-129">Response</span></span>

<span data-ttu-id="e1426-130">В случае успеха этот метод возвращает код отклика `204 No Content` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1426-130">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1426-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1426-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="e1426-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1426-132">Request</span></span>
<span data-ttu-id="e1426-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1426-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e1426-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1426-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e1426-135">C#</span><span class="sxs-lookup"><span data-stu-id="e1426-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1426-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1426-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1426-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1426-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1426-138">Java</span><span class="sxs-lookup"><span data-stu-id="e1426-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e1426-139">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1426-139">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="e1426-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1426-140">Response</span></span>
<span data-ttu-id="e1426-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e1426-141">The following is an example of the response.</span></span>

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

