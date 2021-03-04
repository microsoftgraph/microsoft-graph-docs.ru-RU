---
title: Удаление проверки подлинностиListener
description: Удаляет аутентификациюListener из события, поддерживаемом проверкой подлинностиEventsPolicy.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c808aa161bacb2612c90a53f58b7163f663e4150
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438493"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="5e0a0-103">Удаление проверки подлинностиListener</span><span class="sxs-lookup"><span data-stu-id="5e0a0-103">Remove authenticationListener</span></span>

<span data-ttu-id="5e0a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e0a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e0a0-105">Удаление указанной [проверки подлинностиListener,](../resources/authenticationlistener.md) определенной для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e0a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e0a0-106">Permissions</span></span>

<span data-ttu-id="5e0a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e0a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e0a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e0a0-109">Permission type</span></span>|<span data-ttu-id="5e0a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e0a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e0a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e0a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e0a0-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e0a0-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="5e0a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e0a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e0a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-114">Not supported.</span></span>|
|<span data-ttu-id="5e0a0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5e0a0-115">Application</span></span>|<span data-ttu-id="5e0a0-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e0a0-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e0a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e0a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e0a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e0a0-118">Request headers</span></span>

|<span data-ttu-id="5e0a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5e0a0-119">Name</span></span>|<span data-ttu-id="5e0a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5e0a0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5e0a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e0a0-121">Authorization</span></span>|<span data-ttu-id="5e0a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e0a0-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e0a0-124">Request body</span></span>

<span data-ttu-id="5e0a0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e0a0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e0a0-126">Response</span></span>

<span data-ttu-id="5e0a0-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5e0a0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5e0a0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e0a0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e0a0-129">Request</span></span>

<span data-ttu-id="5e0a0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="5e0a0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e0a0-131">Response</span></span>

<span data-ttu-id="5e0a0-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5e0a0-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
