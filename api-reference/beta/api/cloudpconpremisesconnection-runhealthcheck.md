---
title: 'CloudPcOnPremisesConnection: runHealthChecks'
description: Запустите проверки состояния на локальном подключении к облачному компьютеру.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b207be1da6585adcabb76c8f51f048db1e159d77
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705846"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="ea099-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="ea099-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="ea099-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea099-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea099-105">Запустите проверки состояния объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="ea099-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="ea099-106">Это инициирует новую проверку состояния для этого объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) и изменит свойства healthCheckStatus и [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) после завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="ea099-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ea099-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea099-107">Permissions</span></span>

<span data-ttu-id="ea099-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea099-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea099-110">Permission type</span></span>|<span data-ttu-id="ea099-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea099-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea099-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea099-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea099-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea099-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ea099-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea099-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea099-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea099-115">Not supported.</span></span>|
|<span data-ttu-id="ea099-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea099-116">Application</span></span>|<span data-ttu-id="ea099-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea099-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea099-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea099-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="ea099-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea099-119">Request headers</span></span>

|<span data-ttu-id="ea099-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ea099-120">Name</span></span>|<span data-ttu-id="ea099-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ea099-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ea099-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea099-122">Authorization</span></span>|<span data-ttu-id="ea099-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea099-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea099-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea099-125">Request body</span></span>

<span data-ttu-id="ea099-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea099-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea099-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea099-127">Response</span></span>

<span data-ttu-id="ea099-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea099-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ea099-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ea099-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea099-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea099-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ea099-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea099-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="ea099-132">C#</span><span class="sxs-lookup"><span data-stu-id="ea099-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea099-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea099-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea099-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea099-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea099-135">Java</span><span class="sxs-lookup"><span data-stu-id="ea099-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea099-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea099-136">Response</span></span>

<span data-ttu-id="ea099-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea099-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
