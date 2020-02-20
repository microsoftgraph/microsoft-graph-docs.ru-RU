---
title: Получение Пфксрекриптионрекуест
description: Чтение свойств и связей объекта Пфксрекриптионрекуест.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 401ae1b85868488552cea924b4e873d32d8a5224
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161309"
---
# <a name="get-pfxrecryptionrequest"></a><span data-ttu-id="c54ef-103">Получение Пфксрекриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="c54ef-103">Get pfxRecryptionRequest</span></span>

> <span data-ttu-id="c54ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c54ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c54ef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c54ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c54ef-106">Чтение свойств и связей объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c54ef-106">Read properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c54ef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c54ef-107">Prerequisites</span></span>
<span data-ttu-id="c54ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c54ef-110">Permission type</span></span>|<span data-ttu-id="c54ef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c54ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c54ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c54ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c54ef-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c54ef-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c54ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c54ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c54ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c54ef-115">Not supported.</span></span>|
|<span data-ttu-id="c54ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c54ef-116">Application</span></span>|<span data-ttu-id="c54ef-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c54ef-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c54ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c54ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c54ef-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c54ef-119">Optional query parameters</span></span>
<span data-ttu-id="c54ef-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c54ef-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c54ef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c54ef-121">Request headers</span></span>
|<span data-ttu-id="c54ef-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c54ef-122">Header</span></span>|<span data-ttu-id="c54ef-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c54ef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c54ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c54ef-124">Authorization</span></span>|<span data-ttu-id="c54ef-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c54ef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c54ef-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c54ef-126">Accept</span></span>|<span data-ttu-id="c54ef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c54ef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c54ef-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c54ef-128">Request body</span></span>
<span data-ttu-id="c54ef-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c54ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c54ef-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c54ef-130">Response</span></span>
<span data-ttu-id="c54ef-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c54ef-131">If successful, this method returns a `200 OK` response code and [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c54ef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c54ef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c54ef-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c54ef-133">Request</span></span>
<span data-ttu-id="c54ef-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c54ef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

### <a name="response"></a><span data-ttu-id="c54ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c54ef-135">Response</span></span>
<span data-ttu-id="c54ef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c54ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
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
}
```





