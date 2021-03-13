---
title: 'приложение: setVerifiedPublisher'
description: Установка проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ff0558f8618020eca6437d7528f1f6d0f17eafa6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761151"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="19e2b-103">приложение: setVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="19e2b-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="19e2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19e2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19e2b-105">Установите [verifiedPublisher](../resources/verifiedPublisher.md) в [приложении.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="19e2b-105">Set the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="19e2b-106">Дополнительные сведения, в том числе необходимые для установки проверенного издателя, см. в книге [Проверка Publisher.](/azure/active-directory/develop/publisher-verification-overview)</span><span class="sxs-lookup"><span data-stu-id="19e2b-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="19e2b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19e2b-107">Permissions</span></span>

|<span data-ttu-id="19e2b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19e2b-108">Permission type</span></span>      | <span data-ttu-id="19e2b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19e2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19e2b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19e2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19e2b-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e2b-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="19e2b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19e2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e2b-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="19e2b-113">Not supported</span></span> |
|<span data-ttu-id="19e2b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19e2b-114">Application</span></span> | <span data-ttu-id="19e2b-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="19e2b-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="19e2b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19e2b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="19e2b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19e2b-117">Request headers</span></span>

| <span data-ttu-id="19e2b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="19e2b-118">Name</span></span>           | <span data-ttu-id="19e2b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="19e2b-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="19e2b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19e2b-120">Authorization</span></span>  | <span data-ttu-id="19e2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19e2b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="19e2b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19e2b-123">Content-Type</span></span>   | <span data-ttu-id="19e2b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19e2b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19e2b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19e2b-126">Request body</span></span>

<span data-ttu-id="19e2b-127">В теле запроса укажи следующие необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="19e2b-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="19e2b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="19e2b-128">Property</span></span>     | <span data-ttu-id="19e2b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="19e2b-129">Type</span></span>   |<span data-ttu-id="19e2b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="19e2b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19e2b-131">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="19e2b-131">verifiedPublisherId</span></span> | <span data-ttu-id="19e2b-132">string</span><span class="sxs-lookup"><span data-stu-id="19e2b-132">string</span></span> | <span data-ttu-id="19e2b-133">ID microsoft Partner Network (MPNID) проверенного издателя, который будет задат в приложении, из учетной записи Центра партнеров издателя.</span><span class="sxs-lookup"><span data-stu-id="19e2b-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="19e2b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e2b-134">Response</span></span>

<span data-ttu-id="19e2b-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="19e2b-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19e2b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="19e2b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="19e2b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="19e2b-137">Request</span></span>

<span data-ttu-id="19e2b-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19e2b-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="19e2b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e2b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_setverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/setVerifiedPublisher
Content-type: application/json

{
    "verifiedPublisherId": "1234567"
}
```
# <a name="javascript"></a>[<span data-ttu-id="19e2b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19e2b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-setverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19e2b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e2b-141">Response</span></span>

<span data-ttu-id="19e2b-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="19e2b-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8c7a28dd-cebd-4dc0-b195-b2c7476e7a65
2020-09-09 21:28:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
