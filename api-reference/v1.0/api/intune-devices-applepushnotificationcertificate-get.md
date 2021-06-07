---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6361eba675cc180bb76eef733594471cb2f5f60
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752646"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="a4624-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a4624-103">Get applePushNotificationCertificate</span></span>

<span data-ttu-id="a4624-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4624-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4624-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4624-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4624-106">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="a4624-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4624-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a4624-107">Prerequisites</span></span>
<span data-ttu-id="a4624-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4624-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4624-110">Permission type</span></span>|<span data-ttu-id="a4624-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4624-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4624-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4624-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4624-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4624-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a4624-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4624-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4624-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4624-115">Not supported.</span></span>|
|<span data-ttu-id="a4624-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4624-116">Application</span></span>|<span data-ttu-id="a4624-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4624-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4624-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4624-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4624-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4624-119">Optional query parameters</span></span>
<span data-ttu-id="a4624-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4624-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4624-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4624-121">Request headers</span></span>
|<span data-ttu-id="a4624-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4624-122">Header</span></span>|<span data-ttu-id="a4624-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a4624-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4624-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4624-124">Authorization</span></span>|<span data-ttu-id="a4624-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4624-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4624-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a4624-126">Accept</span></span>|<span data-ttu-id="a4624-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a4624-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4624-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4624-128">Request body</span></span>
<span data-ttu-id="a4624-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4624-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4624-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4624-130">Response</span></span>
<span data-ttu-id="a4624-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4624-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4624-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a4624-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4624-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4624-133">Request</span></span>
<span data-ttu-id="a4624-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4624-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="a4624-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4624-135">Response</span></span>
<span data-ttu-id="a4624-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4624-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificate": "Certificate value"
  }
}
```




