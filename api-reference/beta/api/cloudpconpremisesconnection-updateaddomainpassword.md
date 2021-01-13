---
title: 'cloudPcOnPremisesConnection: updateAdDomainPassword'
description: Обновление пароля домена AD для успешного подключения onPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ca47884a99b0feec3721708b7c16cbc426e53e90
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845110"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a><span data-ttu-id="46916-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="46916-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span></span>
<span data-ttu-id="46916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46916-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46916-105">Обновление пароля домена Active Directory для [onPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="46916-105">Update Active Directory domain password for an [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="46916-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46916-106">Permissions</span></span>
<span data-ttu-id="46916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46916-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46916-109">Permission type</span></span>|<span data-ttu-id="46916-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46916-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46916-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46916-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46916-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46916-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="46916-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46916-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46916-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46916-114">Not supported.</span></span>|
|<span data-ttu-id="46916-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46916-115">Application</span></span>|<span data-ttu-id="46916-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46916-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46916-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46916-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a><span data-ttu-id="46916-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46916-118">Request headers</span></span>
|<span data-ttu-id="46916-119">Имя</span><span class="sxs-lookup"><span data-stu-id="46916-119">Name</span></span>|<span data-ttu-id="46916-120">Описание</span><span class="sxs-lookup"><span data-stu-id="46916-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46916-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46916-121">Authorization</span></span>|<span data-ttu-id="46916-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46916-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="46916-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46916-124">Content-Type</span></span>|<span data-ttu-id="46916-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46916-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46916-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46916-127">Request body</span></span>
<span data-ttu-id="46916-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46916-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="46916-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="46916-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="46916-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="46916-130">Parameter</span></span>|<span data-ttu-id="46916-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46916-131">Type</span></span>|<span data-ttu-id="46916-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46916-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46916-133">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="46916-133">adDomainPassword</span></span>|<span data-ttu-id="46916-134">String</span><span class="sxs-lookup"><span data-stu-id="46916-134">String</span></span>|<span data-ttu-id="46916-135">Пароль, связанный с adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="46916-135">The password associated with adDomainUsername</span></span>|



## <a name="response"></a><span data-ttu-id="46916-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="46916-136">Response</span></span>

<span data-ttu-id="46916-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46916-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="46916-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="46916-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46916-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="46916-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="46916-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="46916-140">Response</span></span>
<span data-ttu-id="46916-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="46916-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
