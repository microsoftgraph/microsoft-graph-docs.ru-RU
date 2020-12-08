---
title: 'Едисковерикасе: повторное открытие'
description: Повторное открытие закрытого случая обнаружения электронных данных.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: d3f8d4003c255a68458ace489548eb59c43ad710
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597799"
---
# <a name="ediscoverycase-reopen"></a><span data-ttu-id="002ce-103">Едисковерикасе: повторное открытие</span><span class="sxs-lookup"><span data-stu-id="002ce-103">ediscoveryCase: reopen</span></span>

<span data-ttu-id="002ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="002ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="002ce-105">Повторное открытие закрытого случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="002ce-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="002ce-106">Дополнительные сведения см. [в статье повторное открытие закрытого дела](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span><span class="sxs-lookup"><span data-stu-id="002ce-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="002ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="002ce-107">Permissions</span></span>
<span data-ttu-id="002ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="002ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="002ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="002ce-110">Permission type</span></span>|<span data-ttu-id="002ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="002ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="002ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="002ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="002ce-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="002ce-113">User.Read</span></span>|
|<span data-ttu-id="002ce-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="002ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="002ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="002ce-115">Not supported.</span></span>|
|<span data-ttu-id="002ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="002ce-116">Application</span></span>|<span data-ttu-id="002ce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="002ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="002ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="002ce-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="002ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="002ce-119">Request headers</span></span>

|<span data-ttu-id="002ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="002ce-120">Name</span></span>|<span data-ttu-id="002ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="002ce-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="002ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="002ce-122">Authorization</span></span>|<span data-ttu-id="002ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="002ce-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="002ce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="002ce-125">Request body</span></span>

<span data-ttu-id="002ce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="002ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="002ce-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="002ce-127">Response</span></span>

<span data-ttu-id="002ce-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="002ce-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="002ce-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="002ce-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="002ce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="002ce-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "ediscoverycase_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```

### <a name="response"></a><span data-ttu-id="002ce-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="002ce-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
