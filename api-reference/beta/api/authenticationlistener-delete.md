---
title: Удаление authenticationListener
description: Удаляет authenticationListener из события, поддерживаемых authenticationEventsPolicy.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3db702f80e92ce475d0b3699236096d7d7b79392
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872326"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="7d0c5-103">Удаление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="7d0c5-103">Remove authenticationListener</span></span>

<span data-ttu-id="7d0c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d0c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d0c5-105">Удалите указанный [authenticationListener,](../resources/authenticationlistener.md) определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d0c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d0c5-106">Permissions</span></span>

<span data-ttu-id="7d0c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d0c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d0c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d0c5-109">Permission type</span></span>|<span data-ttu-id="7d0c5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d0c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d0c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d0c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d0c5-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d0c5-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="7d0c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d0c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d0c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-114">Not supported.</span></span>|
|<span data-ttu-id="7d0c5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d0c5-115">Application</span></span>|<span data-ttu-id="7d0c5-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d0c5-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d0c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d0c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7d0c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d0c5-118">Request headers</span></span>

|<span data-ttu-id="7d0c5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d0c5-119">Name</span></span>|<span data-ttu-id="7d0c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d0c5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7d0c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d0c5-121">Authorization</span></span>|<span data-ttu-id="7d0c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d0c5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d0c5-124">Request body</span></span>

<span data-ttu-id="7d0c5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d0c5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0c5-126">Response</span></span>

<span data-ttu-id="7d0c5-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7d0c5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d0c5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d0c5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d0c5-129">Request</span></span>

<span data-ttu-id="7d0c5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="7d0c5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0c5-131">Response</span></span>

<span data-ttu-id="7d0c5-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d0c5-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
