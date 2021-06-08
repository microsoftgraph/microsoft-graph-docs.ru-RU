---
title: 'servicePrincipal: Добавление владельца'
description: Добавление владельца для субъекта-службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fcca1742a5cb04f03a45d54b7104d46af35097c0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786126"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="24ea7-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="24ea7-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="24ea7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24ea7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24ea7-105">Добавление владельца для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="24ea7-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24ea7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24ea7-106">Permissions</span></span>
<span data-ttu-id="24ea7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24ea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24ea7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24ea7-109">Permission type</span></span>      | <span data-ttu-id="24ea7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24ea7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24ea7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24ea7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24ea7-112">Application.ReadWrite.All и Directory.Read.All, Application.ReadWrite.All и Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24ea7-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24ea7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24ea7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24ea7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24ea7-114">Not supported.</span></span>    |
|<span data-ttu-id="24ea7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24ea7-115">Application</span></span> | <span data-ttu-id="24ea7-116">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All, Application.ReadWrite.OwnedBy и Directory.ReadWrite.All, Application.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ea7-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="24ea7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24ea7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="24ea7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24ea7-118">Request headers</span></span>
| <span data-ttu-id="24ea7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="24ea7-119">Name</span></span>       | <span data-ttu-id="24ea7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="24ea7-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="24ea7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24ea7-121">Authorization</span></span> | <span data-ttu-id="24ea7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24ea7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24ea7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24ea7-124">Request body</span></span>
<span data-ttu-id="24ea7-125">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="24ea7-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="24ea7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="24ea7-126">Response</span></span>

<span data-ttu-id="24ea7-127">В случае успеха этот метод возвращает код отклика `204 No Content` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24ea7-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24ea7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="24ea7-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="24ea7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="24ea7-129">Request</span></span>
<span data-ttu-id="24ea7-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24ea7-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="24ea7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="24ea7-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="24ea7-132">C#</span><span class="sxs-lookup"><span data-stu-id="24ea7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24ea7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24ea7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24ea7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24ea7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24ea7-135">Java</span><span class="sxs-lookup"><span data-stu-id="24ea7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="24ea7-136">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="24ea7-136">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="24ea7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="24ea7-137">Response</span></span>
<span data-ttu-id="24ea7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="24ea7-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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



