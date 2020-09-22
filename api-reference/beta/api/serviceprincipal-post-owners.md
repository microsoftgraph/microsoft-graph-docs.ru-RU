---
title: 'servicePrincipal: Добавление владельца'
description: Добавление владельца для субъекта-службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2618223235fbc7f81eab110d272d1b02c0e14054
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076773"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="3650e-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="3650e-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="3650e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3650e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3650e-105">Добавление владельца для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="3650e-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3650e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3650e-106">Permissions</span></span>
<span data-ttu-id="3650e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3650e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3650e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3650e-109">Permission type</span></span>      | <span data-ttu-id="3650e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3650e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3650e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3650e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3650e-112">Application.ReadWrite.All и Directory.Read.All, Application.ReadWrite.All и Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3650e-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3650e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3650e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3650e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3650e-114">Not supported.</span></span>    |
|<span data-ttu-id="3650e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3650e-115">Application</span></span> | <span data-ttu-id="3650e-116">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All, Application.ReadWrite.OwnedBy и Directory.ReadWrite.All, Application.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3650e-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3650e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3650e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="3650e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3650e-118">Request headers</span></span>
| <span data-ttu-id="3650e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3650e-119">Name</span></span>       | <span data-ttu-id="3650e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3650e-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="3650e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3650e-121">Authorization</span></span> | <span data-ttu-id="3650e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3650e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3650e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3650e-124">Request body</span></span>
<span data-ttu-id="3650e-125">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3650e-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3650e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3650e-126">Response</span></span>

<span data-ttu-id="3650e-127">В случае успеха этот метод возвращает код отклика `204 No Content` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3650e-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3650e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3650e-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="3650e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3650e-129">Request</span></span>
<span data-ttu-id="3650e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3650e-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3650e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3650e-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3650e-132">C#</span><span class="sxs-lookup"><span data-stu-id="3650e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3650e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3650e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3650e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3650e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3650e-135">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3650e-135">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="3650e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3650e-136">Response</span></span>
<span data-ttu-id="3650e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3650e-137">The following is an example of the response.</span></span>

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


