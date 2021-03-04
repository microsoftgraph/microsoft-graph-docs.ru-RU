---
title: Удаление legalHold
description: Удаление объекта legalHold.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 90a7600f972a08220579dec56b1e0f738459c283
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447014"
---
# <a name="delete-legalhold"></a><span data-ttu-id="cb662-103">Удаление legalHold</span><span class="sxs-lookup"><span data-stu-id="cb662-103">Delete legalHold</span></span>

<span data-ttu-id="cb662-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="cb662-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb662-105">Удаление [объекта legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="cb662-105">Delete a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb662-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb662-106">Permissions</span></span>

<span data-ttu-id="cb662-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb662-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb662-109">Permission type</span></span>|<span data-ttu-id="cb662-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb662-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb662-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb662-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb662-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb662-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="cb662-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb662-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb662-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb662-114">Not supported.</span></span>|
|<span data-ttu-id="cb662-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb662-115">Application</span></span>|<span data-ttu-id="cb662-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb662-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb662-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb662-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/legalHolds/{legalHoldId}
```

## <a name="request-headers"></a><span data-ttu-id="cb662-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb662-118">Request headers</span></span>

|<span data-ttu-id="cb662-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cb662-119">Name</span></span>|<span data-ttu-id="cb662-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb662-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb662-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb662-121">Authorization</span></span>|<span data-ttu-id="cb662-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb662-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb662-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb662-124">Request body</span></span>

<span data-ttu-id="cb662-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb662-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb662-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb662-126">Response</span></span>

<span data-ttu-id="cb662-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cb662-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cb662-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb662-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb662-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb662-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_legalhold"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

### <a name="response"></a><span data-ttu-id="cb662-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb662-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
