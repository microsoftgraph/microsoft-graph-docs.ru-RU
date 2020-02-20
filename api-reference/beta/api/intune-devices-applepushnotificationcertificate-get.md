---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d778ac8f19864fac47c69ff81aacf8df2f0039e6
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162262"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="c3b33-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="c3b33-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="c3b33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3b33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3b33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3b33-106">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c3b33-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3b33-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3b33-107">Prerequisites</span></span>
<span data-ttu-id="c3b33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b33-110">Permission type</span></span>|<span data-ttu-id="c3b33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3b33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3b33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3b33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3b33-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b33-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c3b33-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3b33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3b33-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b33-115">Not supported.</span></span>|
|<span data-ttu-id="c3b33-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3b33-116">Application</span></span>|<span data-ttu-id="c3b33-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b33-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3b33-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3b33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3b33-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3b33-119">Optional query parameters</span></span>
<span data-ttu-id="c3b33-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3b33-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3b33-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3b33-121">Request headers</span></span>
|<span data-ttu-id="c3b33-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3b33-122">Header</span></span>|<span data-ttu-id="c3b33-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c3b33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3b33-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3b33-124">Authorization</span></span>|<span data-ttu-id="c3b33-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3b33-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c3b33-126">Accept</span></span>|<span data-ttu-id="c3b33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3b33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3b33-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3b33-128">Request body</span></span>
<span data-ttu-id="c3b33-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3b33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3b33-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3b33-130">Response</span></span>
<span data-ttu-id="c3b33-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3b33-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3b33-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c3b33-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3b33-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3b33-133">Request</span></span>
<span data-ttu-id="c3b33-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3b33-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="c3b33-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b33-135">Response</span></span>
<span data-ttu-id="c3b33-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3b33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





