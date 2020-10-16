---
title: 'Приложение: Сетверифиедпублишер'
description: Установка проверенного издателя приложения.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b9f56a4bf020003f71679c07f380c992b48db491
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471538"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="40a51-103">Приложение: Сетверифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="40a51-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="40a51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40a51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40a51-105">Задайте [верифиедпублишер](../resources/verifiedPublisher.md) для [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="40a51-105">Set the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="40a51-106">Дополнительные сведения, включая предварительные требования для настройки проверенного издателя, можно найти в статье [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="40a51-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="40a51-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40a51-107">Permissions</span></span>

|<span data-ttu-id="40a51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40a51-108">Permission type</span></span>      | <span data-ttu-id="40a51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40a51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40a51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40a51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40a51-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40a51-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="40a51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40a51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40a51-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="40a51-113">Not supported</span></span> |
|<span data-ttu-id="40a51-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="40a51-114">Application</span></span> | <span data-ttu-id="40a51-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="40a51-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="40a51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40a51-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="40a51-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40a51-117">Request headers</span></span>

| <span data-ttu-id="40a51-118">Имя</span><span class="sxs-lookup"><span data-stu-id="40a51-118">Name</span></span>           | <span data-ttu-id="40a51-119">Описание</span><span class="sxs-lookup"><span data-stu-id="40a51-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="40a51-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40a51-120">Authorization</span></span>  | <span data-ttu-id="40a51-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40a51-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40a51-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40a51-123">Content-Type</span></span>   | <span data-ttu-id="40a51-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40a51-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40a51-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40a51-126">Request body</span></span>

<span data-ttu-id="40a51-127">В тексте запроса укажите следующие обязательные свойства.</span><span class="sxs-lookup"><span data-stu-id="40a51-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="40a51-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="40a51-128">Property</span></span>     | <span data-ttu-id="40a51-129">Тип</span><span class="sxs-lookup"><span data-stu-id="40a51-129">Type</span></span>   |<span data-ttu-id="40a51-130">Описание</span><span class="sxs-lookup"><span data-stu-id="40a51-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40a51-131">верифиедпублишерид</span><span class="sxs-lookup"><span data-stu-id="40a51-131">verifiedPublisherId</span></span> | <span data-ttu-id="40a51-132">Строка</span><span class="sxs-lookup"><span data-stu-id="40a51-132">string</span></span> | <span data-ttu-id="40a51-133">Идентификатор сети партнерской сети (МПНИД) проверенного издателя, который необходимо задать для приложения, из учетной записи центра партнера издателя.</span><span class="sxs-lookup"><span data-stu-id="40a51-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="40a51-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="40a51-134">Response</span></span>

<span data-ttu-id="40a51-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40a51-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40a51-136">Пример</span><span class="sxs-lookup"><span data-stu-id="40a51-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="40a51-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="40a51-137">Request</span></span>

<span data-ttu-id="40a51-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40a51-138">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="40a51-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="40a51-139">Response</span></span>

<span data-ttu-id="40a51-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40a51-140">The following is an example of the response.</span></span>

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
