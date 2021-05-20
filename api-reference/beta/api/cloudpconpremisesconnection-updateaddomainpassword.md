---
title: 'cloudPcOnPremisesConnection: updateAdDomainPassword'
description: Обновление пароля домена AD для успешного подключения к доменуPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6a7420574c8dc1a4231f9854a10b76b7291b3ad4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546835"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a><span data-ttu-id="68cef-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="68cef-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span></span>
<span data-ttu-id="68cef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68cef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68cef-105">Обновление пароля домена Active Directory для [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span><span class="sxs-lookup"><span data-stu-id="68cef-105">Update Active Directory domain password for an [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="68cef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68cef-106">Permissions</span></span>
<span data-ttu-id="68cef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68cef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68cef-109">Permission type</span></span>|<span data-ttu-id="68cef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68cef-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68cef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68cef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68cef-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cef-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="68cef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68cef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68cef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68cef-114">Not supported.</span></span>|
|<span data-ttu-id="68cef-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="68cef-115">Application</span></span>|<span data-ttu-id="68cef-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cef-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68cef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68cef-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a><span data-ttu-id="68cef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68cef-118">Request headers</span></span>
|<span data-ttu-id="68cef-119">Имя</span><span class="sxs-lookup"><span data-stu-id="68cef-119">Name</span></span>|<span data-ttu-id="68cef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="68cef-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68cef-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68cef-121">Authorization</span></span>|<span data-ttu-id="68cef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68cef-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="68cef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68cef-124">Content-Type</span></span>|<span data-ttu-id="68cef-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68cef-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68cef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68cef-127">Request body</span></span>
<span data-ttu-id="68cef-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68cef-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="68cef-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="68cef-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="68cef-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="68cef-130">Parameter</span></span>|<span data-ttu-id="68cef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68cef-131">Type</span></span>|<span data-ttu-id="68cef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68cef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68cef-133">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="68cef-133">adDomainPassword</span></span>|<span data-ttu-id="68cef-134">String</span><span class="sxs-lookup"><span data-stu-id="68cef-134">String</span></span>|<span data-ttu-id="68cef-135">Пароль, связанный с adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="68cef-135">The password associated with adDomainUsername</span></span>|



## <a name="response"></a><span data-ttu-id="68cef-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="68cef-136">Response</span></span>

<span data-ttu-id="68cef-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68cef-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="68cef-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="68cef-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68cef-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="68cef-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="68cef-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="68cef-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_updateaddomainpassword"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
Content-Type: application/json
Content-length: 36

{
  "adDomainPassword": "AdDomainPassword value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="68cef-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68cef-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-updateaddomainpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68cef-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68cef-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-updateaddomainpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="68cef-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="68cef-143">Response</span></span>
<span data-ttu-id="68cef-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68cef-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
