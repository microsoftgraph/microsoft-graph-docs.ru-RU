---
title: 'Приложение: Унсетверифиедпублишер'
description: Удаление проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 88bf73cbd90b5bf1eb2c4c8f22d11a232d1cc581
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634689"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="6f721-103">Приложение: Унсетверифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="6f721-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="6f721-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f721-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f721-105">Отмените настройку [верифиедпублишер](../resources/verifiedPublisher.md) , предварительно заданной для [приложения](../resources/application.md), удалив все проверенные свойства издателя.</span><span class="sxs-lookup"><span data-stu-id="6f721-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="6f721-106">Для получения дополнительных сведений см [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="6f721-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f721-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f721-107">Permissions</span></span>

|<span data-ttu-id="6f721-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f721-108">Permission type</span></span>      | <span data-ttu-id="6f721-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f721-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f721-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f721-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f721-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f721-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="6f721-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f721-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f721-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f721-113">Not supported</span></span> |
|<span data-ttu-id="6f721-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f721-114">Application</span></span> | <span data-ttu-id="6f721-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f721-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f721-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f721-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="6f721-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f721-117">Request headers</span></span>

| <span data-ttu-id="6f721-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6f721-118">Name</span></span>           | <span data-ttu-id="6f721-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6f721-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6f721-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f721-120">Authorization</span></span>  | <span data-ttu-id="6f721-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f721-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f721-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f721-123">Request body</span></span>

<span data-ttu-id="6f721-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f721-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f721-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f721-125">Response</span></span>

<span data-ttu-id="6f721-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f721-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6f721-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6f721-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f721-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f721-128">Request</span></span>

<span data-ttu-id="6f721-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f721-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f721-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f721-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="6f721-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f721-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f721-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f721-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6f721-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f721-133">Response</span></span>

<span data-ttu-id="6f721-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f721-134">The following is an example of the response.</span></span>

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
