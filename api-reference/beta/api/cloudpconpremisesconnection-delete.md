---
title: Удаление Клаудпконпремисесконнектион
description: Удаление объекта Клаудпконпремисесконнектион.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 73c3f899a3c7fbc862ddb68a243dbddd33205ba4
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378482"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="ebd3b-103">Удаление Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="ebd3b-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="ebd3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebd3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebd3b-105">Удаление определенного объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="ebd3b-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="ebd3b-106">При удалении подключения удаляются разрешения для службы из указанных ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="ebd3b-107">Вы не можете удалить локальное подключение после того, как оно прошло проверку работоспособности, которое указывается `healthCheckStatus` свойством.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="ebd3b-108">Невозможно удалить подключение, если оно используется, как указано в `inUse` свойстве.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebd3b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebd3b-109">Permissions</span></span>

<span data-ttu-id="ebd3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebd3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebd3b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebd3b-112">Permission type</span></span>|<span data-ttu-id="ebd3b-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebd3b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebd3b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebd3b-114">Delegated (work or school account)</span></span>|<span data-ttu-id="ebd3b-115">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebd3b-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ebd3b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebd3b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebd3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-117">Not supported.</span></span>|
|<span data-ttu-id="ebd3b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebd3b-118">Application</span></span>|<span data-ttu-id="ebd3b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebd3b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebd3b-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ebd3b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebd3b-121">Request headers</span></span>

|<span data-ttu-id="ebd3b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ebd3b-122">Name</span></span>|<span data-ttu-id="ebd3b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ebd3b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ebd3b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebd3b-124">Authorization</span></span>|<span data-ttu-id="ebd3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebd3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebd3b-127">Request body</span></span>

<span data-ttu-id="ebd3b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebd3b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebd3b-129">Response</span></span>

<span data-ttu-id="ebd3b-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ebd3b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ebd3b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebd3b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebd3b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

### <a name="response"></a><span data-ttu-id="ebd3b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebd3b-133">Response</span></span>

<span data-ttu-id="ebd3b-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebd3b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
