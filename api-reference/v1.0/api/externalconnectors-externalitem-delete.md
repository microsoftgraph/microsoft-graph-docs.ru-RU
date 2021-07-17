---
title: Удаление externalItem
description: Удаляет объект externalItem.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6cf75898963765192ef5f380bddc10794c616a66
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467501"
---
# <a name="delete-externalitem"></a><span data-ttu-id="4d276-103">Удаление externalItem</span><span class="sxs-lookup"><span data-stu-id="4d276-103">Delete externalItem</span></span>
<span data-ttu-id="4d276-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="4d276-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="4d276-105">Удаляет [объект externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d276-105">Deletes an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d276-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d276-106">Permissions</span></span>
<span data-ttu-id="4d276-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d276-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d276-109">Permission type</span></span>|<span data-ttu-id="4d276-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d276-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d276-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d276-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d276-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="4d276-112">Not applicable</span></span>|
|<span data-ttu-id="4d276-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d276-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d276-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="4d276-114">Not applicable</span></span>|
|<span data-ttu-id="4d276-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4d276-115">Application</span></span>| <span data-ttu-id="4d276-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d276-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d276-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d276-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionsId}/items/{externalItemId}
```

## <a name="request-headers"></a><span data-ttu-id="4d276-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d276-118">Request headers</span></span>
|<span data-ttu-id="4d276-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4d276-119">Name</span></span>|<span data-ttu-id="4d276-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4d276-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4d276-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d276-121">Authorization</span></span>|<span data-ttu-id="4d276-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d276-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d276-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d276-124">Request body</span></span>
<span data-ttu-id="4d276-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d276-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d276-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d276-126">Response</span></span>

<span data-ttu-id="4d276-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d276-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4d276-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="4d276-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d276-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d276-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
```


### <a name="response"></a><span data-ttu-id="4d276-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d276-130">Response</span></span>
<span data-ttu-id="4d276-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4d276-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

