---
title: 'приложение: unsetVerifiedPublisher'
description: Удаление проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3741529b51912a077bfb7abe217a6828f64d199f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761320"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="d7c54-103">приложение: unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="d7c54-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="d7c54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7c54-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7c54-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application,](../resources/application.md)removing all verified publisher properties.</span><span class="sxs-lookup"><span data-stu-id="d7c54-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="d7c54-106">Дополнительные сведения см. в [книге Проверка publisher.](/azure/active-directory/develop/publisher-verification-overview)</span><span class="sxs-lookup"><span data-stu-id="d7c54-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7c54-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c54-107">Permissions</span></span>

|<span data-ttu-id="d7c54-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c54-108">Permission type</span></span>      | <span data-ttu-id="d7c54-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7c54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7c54-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7c54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7c54-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c54-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="d7c54-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7c54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7c54-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d7c54-113">Not supported</span></span> |
|<span data-ttu-id="d7c54-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7c54-114">Application</span></span> | <span data-ttu-id="d7c54-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d7c54-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7c54-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7c54-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="d7c54-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7c54-117">Request headers</span></span>

| <span data-ttu-id="d7c54-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d7c54-118">Name</span></span>           | <span data-ttu-id="d7c54-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d7c54-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d7c54-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7c54-120">Authorization</span></span>  | <span data-ttu-id="d7c54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7c54-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7c54-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7c54-123">Request body</span></span>

<span data-ttu-id="d7c54-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7c54-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7c54-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c54-125">Response</span></span>

<span data-ttu-id="d7c54-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d7c54-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d7c54-127">Пример</span><span class="sxs-lookup"><span data-stu-id="d7c54-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7c54-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7c54-128">Request</span></span>

<span data-ttu-id="d7c54-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7c54-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7c54-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c54-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="d7c54-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7c54-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7c54-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7c54-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7c54-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c54-133">Response</span></span>

<span data-ttu-id="d7c54-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d7c54-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: db9f2d4d-e668-4eda-9d88-776b6ca6ca20
2020-09-09 21:29:08 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
