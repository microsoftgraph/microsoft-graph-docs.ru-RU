---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d635d7158926061f94e8304c6d18c8d989f19f5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470044"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="a1506-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a1506-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="a1506-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1506-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1506-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1506-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1506-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1506-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1506-107">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="a1506-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1506-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a1506-108">Prerequisites</span></span>
<span data-ttu-id="a1506-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1506-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1506-111">Permission type</span></span>|<span data-ttu-id="a1506-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1506-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1506-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1506-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1506-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1506-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1506-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1506-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1506-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1506-116">Not supported.</span></span>|
|<span data-ttu-id="a1506-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1506-117">Application</span></span>|<span data-ttu-id="a1506-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1506-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1506-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1506-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="a1506-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1506-120">Request headers</span></span>
|<span data-ttu-id="a1506-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1506-121">Header</span></span>|<span data-ttu-id="a1506-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a1506-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1506-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1506-123">Authorization</span></span>|<span data-ttu-id="a1506-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1506-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1506-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1506-125">Accept</span></span>|<span data-ttu-id="a1506-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1506-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1506-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1506-127">Request body</span></span>
<span data-ttu-id="a1506-128">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1506-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="a1506-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="a1506-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="a1506-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1506-130">Property</span></span>|<span data-ttu-id="a1506-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a1506-131">Type</span></span>|<span data-ttu-id="a1506-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a1506-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1506-133">id</span><span class="sxs-lookup"><span data-stu-id="a1506-133">id</span></span>|<span data-ttu-id="a1506-134">String</span><span class="sxs-lookup"><span data-stu-id="a1506-134">String</span></span>|<span data-ttu-id="a1506-135">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="a1506-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="a1506-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1506-136">appleIdentifier</span></span>|<span data-ttu-id="a1506-137">String</span><span class="sxs-lookup"><span data-stu-id="a1506-137">String</span></span>|<span data-ttu-id="a1506-138">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="a1506-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="a1506-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1506-139">topicIdentifier</span></span>|<span data-ttu-id="a1506-140">String</span><span class="sxs-lookup"><span data-stu-id="a1506-140">String</span></span>|<span data-ttu-id="a1506-141">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="a1506-141">Topic Id.</span></span>|
|<span data-ttu-id="a1506-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1506-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a1506-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1506-143">DateTimeOffset</span></span>|<span data-ttu-id="a1506-144">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="a1506-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a1506-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1506-145">expirationDateTime</span></span>|<span data-ttu-id="a1506-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1506-146">DateTimeOffset</span></span>|<span data-ttu-id="a1506-147">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="a1506-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a1506-148">цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="a1506-148">certificateUploadStatus</span></span>|<span data-ttu-id="a1506-149">String</span><span class="sxs-lookup"><span data-stu-id="a1506-149">String</span></span>|<span data-ttu-id="a1506-150">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="a1506-150">The certificate upload status.</span></span>|
|<span data-ttu-id="a1506-151">цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="a1506-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="a1506-152">String</span><span class="sxs-lookup"><span data-stu-id="a1506-152">String</span></span>|<span data-ttu-id="a1506-153">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="a1506-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="a1506-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="a1506-154">certificateSerialNumber</span></span>|<span data-ttu-id="a1506-155">String</span><span class="sxs-lookup"><span data-stu-id="a1506-155">String</span></span>|<span data-ttu-id="a1506-156">Серийный номер сертификата.</span><span class="sxs-lookup"><span data-stu-id="a1506-156">Certificate serial number.</span></span> <span data-ttu-id="a1506-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1506-157">This property is read-only.</span></span>|
|<span data-ttu-id="a1506-158">certificate</span><span class="sxs-lookup"><span data-stu-id="a1506-158">certificate</span></span>|<span data-ttu-id="a1506-159">String</span><span class="sxs-lookup"><span data-stu-id="a1506-159">String</span></span>|<span data-ttu-id="a1506-160">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a1506-160">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1506-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1506-161">Response</span></span>
<span data-ttu-id="a1506-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1506-162">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1506-163">Пример</span><span class="sxs-lookup"><span data-stu-id="a1506-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1506-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1506-164">Request</span></span>
<span data-ttu-id="a1506-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1506-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 481

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="a1506-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1506-166">Response</span></span>
<span data-ttu-id="a1506-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1506-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
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
```





