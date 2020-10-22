---
title: 'Приложение: Унсетверифиедпублишер'
description: Удаление проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dca739f5086e10fecdfba56cfd1338a9230b4d4d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635519"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="422d8-103">Приложение: Унсетверифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="422d8-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="422d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="422d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="422d8-105">Отмените настройку [верифиедпублишер](../resources/verifiedPublisher.md) , предварительно заданной для [приложения](../resources/application.md), удалив все проверенные свойства издателя.</span><span class="sxs-lookup"><span data-stu-id="422d8-105">Unset the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="422d8-106">Для получения дополнительных сведений см [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="422d8-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="422d8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="422d8-107">Permissions</span></span>

|<span data-ttu-id="422d8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="422d8-108">Permission type</span></span>      | <span data-ttu-id="422d8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="422d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="422d8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="422d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="422d8-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422d8-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="422d8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="422d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="422d8-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="422d8-113">Not supported</span></span> |
|<span data-ttu-id="422d8-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="422d8-114">Application</span></span> | <span data-ttu-id="422d8-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="422d8-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="422d8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="422d8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="422d8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="422d8-117">Request headers</span></span>

| <span data-ttu-id="422d8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="422d8-118">Name</span></span>           | <span data-ttu-id="422d8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="422d8-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="422d8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="422d8-120">Authorization</span></span>  | <span data-ttu-id="422d8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422d8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="422d8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="422d8-123">Request body</span></span>

<span data-ttu-id="422d8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="422d8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="422d8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="422d8-125">Response</span></span>

<span data-ttu-id="422d8-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="422d8-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="422d8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="422d8-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="422d8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="422d8-128">Request</span></span>

<span data-ttu-id="422d8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="422d8-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="422d8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="422d8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="422d8-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="422d8-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="422d8-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="422d8-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="422d8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="422d8-133">Response</span></span>

<span data-ttu-id="422d8-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="422d8-134">The following is an example of the response.</span></span>

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
