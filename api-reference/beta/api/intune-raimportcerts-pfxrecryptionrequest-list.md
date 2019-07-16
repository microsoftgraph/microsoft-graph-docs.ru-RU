---
title: Список Пфксрекриптионрекуестс
description: Список свойств и связей объектов Пфксрекриптионрекуест.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04c052932213720c5270e6b27c89851f7959cb33
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741500"
---
# <a name="list-pfxrecryptionrequests"></a><span data-ttu-id="00f43-103">Список Пфксрекриптионрекуестс</span><span class="sxs-lookup"><span data-stu-id="00f43-103">List pfxRecryptionRequests</span></span>

> <span data-ttu-id="00f43-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00f43-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00f43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00f43-106">Список свойств и связей объектов [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="00f43-106">List properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00f43-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00f43-107">Prerequisites</span></span>
<span data-ttu-id="00f43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f43-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f43-110">Permission type</span></span>|<span data-ttu-id="00f43-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00f43-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f43-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00f43-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00f43-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="00f43-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f43-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00f43-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f43-115">Not supported.</span></span>|
|<span data-ttu-id="00f43-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00f43-116">Application</span></span>|<span data-ttu-id="00f43-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f43-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00f43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f43-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="00f43-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00f43-119">Request headers</span></span>
|<span data-ttu-id="00f43-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00f43-120">Header</span></span>|<span data-ttu-id="00f43-121">Значение</span><span class="sxs-lookup"><span data-stu-id="00f43-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00f43-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00f43-122">Authorization</span></span>|<span data-ttu-id="00f43-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f43-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00f43-124">Accept</span><span class="sxs-lookup"><span data-stu-id="00f43-124">Accept</span></span>|<span data-ttu-id="00f43-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00f43-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00f43-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00f43-126">Request body</span></span>
<span data-ttu-id="00f43-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00f43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00f43-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="00f43-128">Response</span></span>
<span data-ttu-id="00f43-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00f43-129">If successful, this method returns a `200 OK` response code and a collection of [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00f43-130">Пример</span><span class="sxs-lookup"><span data-stu-id="00f43-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="00f43-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f43-131">Request</span></span>
<span data-ttu-id="00f43-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00f43-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests
```

### <a name="response"></a><span data-ttu-id="00f43-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f43-133">Response</span></span>
<span data-ttu-id="00f43-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00f43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
      "profileId": "6389d896-d896-6389-96d8-896396d88963",
      "thumbprint": "Thumbprint value",
      "deviceKeyThumbprint": "Device Key Thumbprint value",
      "status": 6,
      "sourceType": 10,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "isDeleted": true,
      "eTag": "ETag value"
    }
  ]
}
```





