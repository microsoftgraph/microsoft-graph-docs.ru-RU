---
title: 'Едисковерикасе: Close'
description: Закройте дело обнаружения электронных данных.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 627c8c1547e8df03c6736f00a5cb571d1c8c93bb
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597787"
---
# <a name="ediscoverycase-close"></a><span data-ttu-id="09b18-103">Едисковерикасе: Close</span><span class="sxs-lookup"><span data-stu-id="09b18-103">ediscoveryCase: close</span></span>

<span data-ttu-id="09b18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09b18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09b18-105">Закройте дело обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="09b18-105">Close an eDiscovery case.</span></span> <span data-ttu-id="09b18-106">Подробнее о том, [как закрыть обращение](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span><span class="sxs-lookup"><span data-stu-id="09b18-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="09b18-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09b18-107">Permissions</span></span>

<span data-ttu-id="09b18-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09b18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09b18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09b18-110">Permission type</span></span>|<span data-ttu-id="09b18-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09b18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09b18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09b18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09b18-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="09b18-113">User.Read</span></span>|
|<span data-ttu-id="09b18-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09b18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09b18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09b18-115">Not supported.</span></span>|
|<span data-ttu-id="09b18-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09b18-116">Application</span></span>|<span data-ttu-id="09b18-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09b18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09b18-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09b18-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="09b18-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09b18-119">Request headers</span></span>

|<span data-ttu-id="09b18-120">Имя</span><span class="sxs-lookup"><span data-stu-id="09b18-120">Name</span></span>|<span data-ttu-id="09b18-121">Описание</span><span class="sxs-lookup"><span data-stu-id="09b18-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="09b18-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09b18-122">Authorization</span></span>|<span data-ttu-id="09b18-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09b18-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09b18-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09b18-125">Request body</span></span>

<span data-ttu-id="09b18-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09b18-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09b18-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="09b18-127">Response</span></span>

<span data-ttu-id="09b18-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="09b18-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="09b18-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="09b18-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09b18-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="09b18-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "ediscoverycase_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```

### <a name="response"></a><span data-ttu-id="09b18-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="09b18-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
