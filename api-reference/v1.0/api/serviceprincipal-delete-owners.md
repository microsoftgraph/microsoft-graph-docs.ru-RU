---
title: Удаление владельца
description: Удаление владельца из службыPrincipals.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: db723a3dc0cfd3890e87690a6b1c232c594c7aa8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787135"
---
# <a name="remove-owner"></a><span data-ttu-id="1d8b5-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="1d8b5-103">Remove owner</span></span>

<span data-ttu-id="1d8b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d8b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d8b5-105">Удаление владельца из [объекта servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="1d8b5-105">Remove an owner from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d8b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d8b5-106">Permissions</span></span>
<span data-ttu-id="1d8b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d8b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d8b5-109">Permission type</span></span>      | <span data-ttu-id="1d8b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d8b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d8b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d8b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d8b5-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d8b5-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d8b5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d8b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d8b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-114">Not supported.</span></span>    |
|<span data-ttu-id="1d8b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d8b5-115">Application</span></span> | <span data-ttu-id="1d8b5-116">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1d8b5-116">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d8b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d8b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="1d8b5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d8b5-118">Request headers</span></span>
| <span data-ttu-id="1d8b5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1d8b5-119">Name</span></span> | <span data-ttu-id="1d8b5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1d8b5-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="1d8b5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d8b5-121">Authorization</span></span> | <span data-ttu-id="1d8b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d8b5-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d8b5-124">Request body</span></span>
<span data-ttu-id="1d8b5-125">В теле запроса укажи идентификатор объекта каталога, назначенного в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="1d8b5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d8b5-126">Response</span></span>

<span data-ttu-id="1d8b5-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1d8b5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1d8b5-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d8b5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d8b5-129">Request</span></span>

<span data-ttu-id="1d8b5-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d8b5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d8b5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="1d8b5-132">C#</span><span class="sxs-lookup"><span data-stu-id="1d8b5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d8b5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d8b5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d8b5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d8b5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d8b5-135">Java</span><span class="sxs-lookup"><span data-stu-id="1d8b5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d8b5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d8b5-136">Response</span></span>

<span data-ttu-id="1d8b5-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-137">The following is an example of the response.</span></span>

><span data-ttu-id="1d8b5-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d8b5-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

