---
title: 'CloudPcOnPremisesConnection: runHealthChecks'
description: Запустите проверки состояния здоровья на локальном подключении облачного компьютера.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: da78bd5117f8795b7fc26c3be0d45d24d83e0acc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947623"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="434a8-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="434a8-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="434a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="434a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="434a8-105">Запустите проверки состояния [на объекте cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="434a8-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="434a8-106">Это вызовет новую проверку состояния для этого [объекта cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) и изменит свойства healthCheckStatus и [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) по завершению проверки.</span><span class="sxs-lookup"><span data-stu-id="434a8-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="434a8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="434a8-107">Permissions</span></span>

<span data-ttu-id="434a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="434a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="434a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="434a8-110">Permission type</span></span>|<span data-ttu-id="434a8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="434a8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="434a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="434a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="434a8-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="434a8-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="434a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="434a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="434a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="434a8-115">Not supported.</span></span>|
|<span data-ttu-id="434a8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="434a8-116">Application</span></span>|<span data-ttu-id="434a8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="434a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="434a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="434a8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="434a8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="434a8-119">Request headers</span></span>

|<span data-ttu-id="434a8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="434a8-120">Name</span></span>|<span data-ttu-id="434a8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="434a8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="434a8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="434a8-122">Authorization</span></span>|<span data-ttu-id="434a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="434a8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="434a8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="434a8-125">Request body</span></span>

<span data-ttu-id="434a8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="434a8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="434a8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="434a8-127">Response</span></span>

<span data-ttu-id="434a8-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="434a8-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="434a8-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="434a8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="434a8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="434a8-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="434a8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="434a8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck_2"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="434a8-132">C#</span><span class="sxs-lookup"><span data-stu-id="434a8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="434a8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="434a8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="434a8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="434a8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="434a8-135">Java</span><span class="sxs-lookup"><span data-stu-id="434a8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="434a8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="434a8-136">Response</span></span>

<span data-ttu-id="434a8-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="434a8-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
