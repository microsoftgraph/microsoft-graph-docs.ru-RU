---
title: Удаление externalConnection
description: Удаляет объект externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e365c09fca03a97894a53b23eef2d500527a774f
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467434"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="ada5d-103">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="ada5d-103">Delete externalConnection</span></span>
<span data-ttu-id="ada5d-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="ada5d-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="ada5d-105">Удаляет объект [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="ada5d-105">Deletes an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ada5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ada5d-106">Permissions</span></span>
<span data-ttu-id="ada5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ada5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ada5d-109">Permission type</span></span>|<span data-ttu-id="ada5d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ada5d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ada5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ada5d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ada5d-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="ada5d-112">Not applicable</span></span>|
|<span data-ttu-id="ada5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ada5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ada5d-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="ada5d-114">Not applicable</span></span>|
|<span data-ttu-id="ada5d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ada5d-115">Application</span></span>| <span data-ttu-id="ada5d-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ada5d-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="ada5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ada5d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionsId}
```

## <a name="request-headers"></a><span data-ttu-id="ada5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ada5d-118">Request headers</span></span>
|<span data-ttu-id="ada5d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ada5d-119">Name</span></span>|<span data-ttu-id="ada5d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ada5d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ada5d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ada5d-121">Authorization</span></span>|<span data-ttu-id="ada5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ada5d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ada5d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ada5d-124">Request body</span></span>
<span data-ttu-id="ada5d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ada5d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ada5d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada5d-126">Response</span></span>

<span data-ttu-id="ada5d-p103">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ada5d-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ada5d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ada5d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ada5d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ada5d-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalconnection"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/connections/contosohr
```


### <a name="response"></a><span data-ttu-id="ada5d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada5d-131">Response</span></span>
<span data-ttu-id="ada5d-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ada5d-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

