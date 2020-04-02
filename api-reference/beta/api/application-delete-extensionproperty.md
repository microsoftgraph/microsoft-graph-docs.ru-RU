---
title: Удаление Екстенсионпроперти
description: Удаление Екстенсионпроперти.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 405518b58bb3bc9a5270992c681aaf098660a61e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107201"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="ca69e-103">Удаление Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="ca69e-103">Delete extensionProperty</span></span>

<span data-ttu-id="ca69e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca69e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca69e-105">Удаление [екстенсионпроперти](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="ca69e-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca69e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca69e-106">Permissions</span></span>

<span data-ttu-id="ca69e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca69e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca69e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca69e-109">Permission type</span></span>      | <span data-ttu-id="ca69e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca69e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca69e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca69e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca69e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca69e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca69e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca69e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca69e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca69e-114">Not supported.</span></span>    |
|<span data-ttu-id="ca69e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca69e-115">Application</span></span> | <span data-ttu-id="ca69e-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca69e-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca69e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca69e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ca69e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca69e-118">Request headers</span></span>

| <span data-ttu-id="ca69e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ca69e-119">Name</span></span>       | <span data-ttu-id="ca69e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ca69e-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ca69e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca69e-121">Authorization</span></span>  | <span data-ttu-id="ca69e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca69e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca69e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca69e-124">Request body</span></span>

<span data-ttu-id="ca69e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca69e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca69e-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca69e-126">Response</span></span>

<span data-ttu-id="ca69e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ca69e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca69e-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca69e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca69e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca69e-130">Request</span></span>

<span data-ttu-id="ca69e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca69e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca69e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca69e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="ca69e-133">C#</span><span class="sxs-lookup"><span data-stu-id="ca69e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca69e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca69e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca69e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca69e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca69e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca69e-136">Response</span></span>

<span data-ttu-id="ca69e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ca69e-137">The following is an example of the response.</span></span>

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
