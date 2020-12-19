---
title: Удаление authenticationListener
description: Удаляет authenticationListener из события, поддерживаемый authenticationEventsPolicy.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb6c12bbba8d5b458ed2dbf6829a88d8e0885e2b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720334"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="fb316-103">Удаление authenticationListener</span><span class="sxs-lookup"><span data-stu-id="fb316-103">Remove authenticationListener</span></span>

<span data-ttu-id="fb316-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb316-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb316-105">Удалите указанный [authenticationListener,](../resources/authenticationlistener.md) определенный для события onSignupStart в конвейере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fb316-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb316-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb316-106">Permissions</span></span>

<span data-ttu-id="fb316-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb316-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb316-109">Permission type</span></span>|<span data-ttu-id="fb316-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb316-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb316-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb316-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb316-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb316-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="fb316-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb316-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb316-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb316-114">Not supported.</span></span>|
|<span data-ttu-id="fb316-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fb316-115">Application</span></span>|<span data-ttu-id="fb316-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb316-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb316-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb316-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb316-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb316-118">Request headers</span></span>

|<span data-ttu-id="fb316-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fb316-119">Name</span></span>|<span data-ttu-id="fb316-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fb316-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb316-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb316-121">Authorization</span></span>|<span data-ttu-id="fb316-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb316-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb316-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb316-124">Request body</span></span>

<span data-ttu-id="fb316-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb316-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb316-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb316-126">Response</span></span>

<span data-ttu-id="fb316-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb316-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fb316-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fb316-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb316-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb316-129">Request</span></span>

<span data-ttu-id="fb316-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb316-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="fb316-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb316-131">Response</span></span>

<span data-ttu-id="fb316-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fb316-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
