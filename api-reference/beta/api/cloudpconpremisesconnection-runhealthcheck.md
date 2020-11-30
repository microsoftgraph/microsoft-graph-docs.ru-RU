---
title: CloudPcOnPremisesConnection-RunHealthChecks
description: Выполнение проверок работоспособности для локального подключения к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 484d48f0400c328090d66bbcf7a930a485a9d950
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378470"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="74f7b-103">Клаудпконпремисесконнектион: Рунхеалсчеккс</span><span class="sxs-lookup"><span data-stu-id="74f7b-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="74f7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74f7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74f7b-105">Выполните проверки работоспособности для объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="74f7b-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="74f7b-106">При этом будет активирована новая проверка работоспособности для объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) и свойства Хеалсчеккстатус и [хеалсчеккстатусдетаилс](../resources/cloudpconpremisesconnectionstatusdetails.md) будут изменены при завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="74f7b-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

## <a name="permissions"></a><span data-ttu-id="74f7b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74f7b-107">Permissions</span></span>

<span data-ttu-id="74f7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74f7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74f7b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74f7b-110">Permission type</span></span>|<span data-ttu-id="74f7b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74f7b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74f7b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74f7b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74f7b-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f7b-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="74f7b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74f7b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f7b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74f7b-115">Not supported.</span></span>|
|<span data-ttu-id="74f7b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74f7b-116">Application</span></span>|<span data-ttu-id="74f7b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74f7b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74f7b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74f7b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="74f7b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74f7b-119">Request headers</span></span>

|<span data-ttu-id="74f7b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="74f7b-120">Name</span></span>|<span data-ttu-id="74f7b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="74f7b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="74f7b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74f7b-122">Authorization</span></span>|<span data-ttu-id="74f7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74f7b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74f7b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74f7b-125">Request body</span></span>

<span data-ttu-id="74f7b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74f7b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74f7b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="74f7b-127">Response</span></span>

<span data-ttu-id="74f7b-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74f7b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="74f7b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="74f7b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74f7b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="74f7b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

### <a name="response"></a><span data-ttu-id="74f7b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="74f7b-131">Response</span></span>

<span data-ttu-id="74f7b-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74f7b-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
