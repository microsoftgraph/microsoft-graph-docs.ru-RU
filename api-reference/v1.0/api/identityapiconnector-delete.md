---
title: Удаление identityApiConnector
description: Удаление объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37217db3bce0a8cf9c7b7d998a88ca4d63e5d41e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883121"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="9e4ba-103">Удаление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="9e4ba-103">Delete identityApiConnector</span></span>

<span data-ttu-id="9e4ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e4ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e4ba-105">Удаление [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="9e4ba-105">Delete an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e4ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e4ba-106">Permissions</span></span>

<span data-ttu-id="9e4ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e4ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e4ba-109">Permission type</span></span>                        | <span data-ttu-id="9e4ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e4ba-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9e4ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e4ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e4ba-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e4ba-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="9e4ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e4ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e4ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e4ba-114">Not supported.</span></span>  |
| <span data-ttu-id="9e4ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e4ba-115">Application</span></span>                            | <span data-ttu-id="9e4ba-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e4ba-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="9e4ba-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="9e4ba-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9e4ba-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9e4ba-118">Global administrator</span></span>
* <span data-ttu-id="9e4ba-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="9e4ba-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9e4ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e4ba-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="9e4ba-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e4ba-121">Request headers</span></span>

|<span data-ttu-id="9e4ba-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9e4ba-122">Name</span></span>|<span data-ttu-id="9e4ba-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9e4ba-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9e4ba-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e4ba-124">Authorization</span></span>|<span data-ttu-id="9e4ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e4ba-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e4ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e4ba-127">Request body</span></span>

<span data-ttu-id="9e4ba-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e4ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e4ba-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e4ba-129">Response</span></span>

<span data-ttu-id="9e4ba-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9e4ba-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9e4ba-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e4ba-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e4ba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e4ba-132">Request</span></span>

<span data-ttu-id="9e4ba-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e4ba-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321
```

### <a name="response"></a><span data-ttu-id="9e4ba-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e4ba-134">Response</span></span>

<span data-ttu-id="9e4ba-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9e4ba-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
