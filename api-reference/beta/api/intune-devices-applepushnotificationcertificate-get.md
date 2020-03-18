---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 818759464e40cffc3ad101ae9bdf8bce152917f9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814794"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="f6f95-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f6f95-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="f6f95-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6f95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6f95-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6f95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f95-106">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="f6f95-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6f95-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6f95-107">Prerequisites</span></span>
<span data-ttu-id="f6f95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6f95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f95-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6f95-110">Permission type</span></span>|<span data-ttu-id="f6f95-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6f95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6f95-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6f95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6f95-113">Девицеманажементсервицеконфиг. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f6f95-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f6f95-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6f95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6f95-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6f95-115">Not supported.</span></span>|
|<span data-ttu-id="f6f95-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6f95-116">Application</span></span>|<span data-ttu-id="f6f95-117">Девицеманажементсервицеконфиг. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f6f95-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6f95-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6f95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6f95-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6f95-119">Optional query parameters</span></span>
<span data-ttu-id="f6f95-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6f95-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6f95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6f95-121">Request headers</span></span>
|<span data-ttu-id="f6f95-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6f95-122">Header</span></span>|<span data-ttu-id="f6f95-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f6f95-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6f95-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6f95-124">Authorization</span></span>|<span data-ttu-id="f6f95-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6f95-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6f95-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f6f95-126">Accept</span></span>|<span data-ttu-id="f6f95-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6f95-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6f95-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6f95-128">Request body</span></span>
<span data-ttu-id="f6f95-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6f95-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6f95-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6f95-130">Response</span></span>
<span data-ttu-id="f6f95-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f6f95-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6f95-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f6f95-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6f95-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6f95-133">Request</span></span>
<span data-ttu-id="f6f95-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6f95-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="f6f95-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6f95-135">Response</span></span>
<span data-ttu-id="f6f95-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6f95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 633

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificateUploadStatus": "Certificate Upload Status value",
    "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificate": "Certificate value"
  }
}
```




