---
title: Удаление Екстенсионпроперти
description: Удаление Екстенсионпроперти.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 744eb25753a6fd2945b5ae21ecea7a747dee4cff
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192535"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="e8eab-103">Удаление Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="e8eab-103">Delete extensionProperty</span></span>

<span data-ttu-id="e8eab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8eab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8eab-105">Удаление [екстенсионпроперти](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e8eab-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8eab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8eab-106">Permissions</span></span>

<span data-ttu-id="e8eab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8eab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8eab-109">Permission type</span></span>      | <span data-ttu-id="e8eab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8eab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8eab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8eab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8eab-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8eab-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e8eab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8eab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8eab-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eab-114">Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8eab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8eab-115">Application</span></span> | <span data-ttu-id="e8eab-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eab-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8eab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8eab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8eab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8eab-118">Request headers</span></span>

| <span data-ttu-id="e8eab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8eab-119">Name</span></span>       | <span data-ttu-id="e8eab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8eab-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e8eab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8eab-121">Authorization</span></span>  | <span data-ttu-id="e8eab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8eab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8eab-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8eab-124">Request body</span></span>

<span data-ttu-id="e8eab-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8eab-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8eab-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8eab-126">Response</span></span>

<span data-ttu-id="e8eab-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e8eab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8eab-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8eab-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8eab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8eab-130">Request</span></span>

<span data-ttu-id="e8eab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8eab-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8eab-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8eab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="e8eab-133">C#</span><span class="sxs-lookup"><span data-stu-id="e8eab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8eab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8eab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8eab-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8eab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8eab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8eab-136">Response</span></span>

<span data-ttu-id="e8eab-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8eab-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


