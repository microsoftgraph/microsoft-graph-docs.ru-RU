---
title: 'приложение: unsetVerifiedPublisher'
description: Удаление проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7560d9935a2cf35bcf67637ce2353932ba522d2b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759925"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="0e035-103">приложение: unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="0e035-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="0e035-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e035-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e035-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application,](../resources/application.md)removing all verified publisher properties.</span><span class="sxs-lookup"><span data-stu-id="0e035-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="0e035-106">Дополнительные сведения см. в [книге Проверка publisher.](/azure/active-directory/develop/publisher-verification-overview)</span><span class="sxs-lookup"><span data-stu-id="0e035-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e035-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e035-107">Permissions</span></span>

|<span data-ttu-id="0e035-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e035-108">Permission type</span></span>      | <span data-ttu-id="0e035-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e035-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e035-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e035-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e035-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e035-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="0e035-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e035-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e035-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0e035-113">Not supported</span></span> |
|<span data-ttu-id="0e035-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e035-114">Application</span></span> | <span data-ttu-id="0e035-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0e035-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e035-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e035-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="0e035-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e035-117">Request headers</span></span>

| <span data-ttu-id="0e035-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0e035-118">Name</span></span>           | <span data-ttu-id="0e035-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0e035-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0e035-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e035-120">Authorization</span></span>  | <span data-ttu-id="0e035-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e035-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e035-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e035-123">Request body</span></span>

<span data-ttu-id="0e035-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e035-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e035-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e035-125">Response</span></span>

<span data-ttu-id="0e035-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e035-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e035-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0e035-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e035-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e035-128">Request</span></span>

<span data-ttu-id="0e035-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e035-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e035-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e035-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="0e035-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e035-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e035-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e035-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e035-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e035-133">Response</span></span>

<span data-ttu-id="0e035-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0e035-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: b0ed721f-7e6a-446c-89bc-2d03e1744dfe
2020-09-09 21:26:11 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
