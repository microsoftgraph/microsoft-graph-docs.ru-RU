---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58c7a0a262fc1207c6e81a2b051f0d2e36a3fecd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910548"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="7c847-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7c847-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="7c847-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c847-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c847-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c847-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c847-106">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7c847-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c847-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c847-107">Prerequisites</span></span>
<span data-ttu-id="7c847-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c847-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c847-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c847-110">Permission type</span></span>|<span data-ttu-id="7c847-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c847-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c847-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c847-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c847-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c847-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7c847-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c847-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c847-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c847-115">Not supported.</span></span>|
|<span data-ttu-id="7c847-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c847-116">Application</span></span>|<span data-ttu-id="7c847-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c847-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c847-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c847-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c847-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c847-119">Optional query parameters</span></span>
<span data-ttu-id="7c847-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7c847-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c847-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c847-121">Request headers</span></span>
|<span data-ttu-id="7c847-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c847-122">Header</span></span>|<span data-ttu-id="7c847-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7c847-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c847-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c847-124">Authorization</span></span>|<span data-ttu-id="7c847-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c847-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c847-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7c847-126">Accept</span></span>|<span data-ttu-id="7c847-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c847-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c847-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c847-128">Request body</span></span>
<span data-ttu-id="7c847-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c847-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c847-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c847-130">Response</span></span>
<span data-ttu-id="7c847-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c847-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c847-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7c847-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c847-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c847-133">Request</span></span>
<span data-ttu-id="7c847-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c847-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="7c847-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c847-135">Response</span></span>
<span data-ttu-id="7c847-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c847-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

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
    "certificate": "Certificate value"
  }
}
```




