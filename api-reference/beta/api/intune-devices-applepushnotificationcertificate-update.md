---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9730ba7ff6d2b876533fda89232749064354d5f6
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162255"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="cd8fc-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="cd8fc-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="cd8fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd8fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd8fc-106">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="cd8fc-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd8fc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cd8fc-107">Prerequisites</span></span>
<span data-ttu-id="cd8fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd8fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd8fc-110">Permission type</span></span>|<span data-ttu-id="cd8fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd8fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd8fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd8fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd8fc-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd8fc-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cd8fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd8fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd8fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-115">Not supported.</span></span>|
|<span data-ttu-id="cd8fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd8fc-116">Application</span></span>|<span data-ttu-id="cd8fc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd8fc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd8fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd8fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="cd8fc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd8fc-119">Request headers</span></span>
|<span data-ttu-id="cd8fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd8fc-120">Header</span></span>|<span data-ttu-id="cd8fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd8fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd8fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd8fc-122">Authorization</span></span>|<span data-ttu-id="cd8fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd8fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd8fc-124">Accept</span></span>|<span data-ttu-id="cd8fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd8fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd8fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd8fc-126">Request body</span></span>
<span data-ttu-id="cd8fc-127">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="cd8fc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="cd8fc-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="cd8fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd8fc-129">Property</span></span>|<span data-ttu-id="cd8fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd8fc-130">Type</span></span>|<span data-ttu-id="cd8fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd8fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd8fc-132">id</span><span class="sxs-lookup"><span data-stu-id="cd8fc-132">id</span></span>|<span data-ttu-id="cd8fc-133">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-133">String</span></span>|<span data-ttu-id="cd8fc-134">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="cd8fc-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="cd8fc-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd8fc-135">appleIdentifier</span></span>|<span data-ttu-id="cd8fc-136">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-136">String</span></span>|<span data-ttu-id="cd8fc-137">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="cd8fc-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd8fc-138">topicIdentifier</span></span>|<span data-ttu-id="cd8fc-139">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-139">String</span></span>|<span data-ttu-id="cd8fc-140">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-140">Topic Id.</span></span>|
|<span data-ttu-id="cd8fc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd8fc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="cd8fc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd8fc-142">DateTimeOffset</span></span>|<span data-ttu-id="cd8fc-143">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="cd8fc-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cd8fc-144">expirationDateTime</span></span>|<span data-ttu-id="cd8fc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd8fc-145">DateTimeOffset</span></span>|<span data-ttu-id="cd8fc-146">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="cd8fc-147">цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="cd8fc-147">certificateUploadStatus</span></span>|<span data-ttu-id="cd8fc-148">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-148">String</span></span>|<span data-ttu-id="cd8fc-149">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-149">The certificate upload status.</span></span>|
|<span data-ttu-id="cd8fc-150">цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="cd8fc-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="cd8fc-151">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-151">String</span></span>|<span data-ttu-id="cd8fc-152">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="cd8fc-153">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="cd8fc-153">certificateSerialNumber</span></span>|<span data-ttu-id="cd8fc-154">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-154">String</span></span>|<span data-ttu-id="cd8fc-155">Серийный номер сертификата.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-155">Certificate serial number.</span></span> <span data-ttu-id="cd8fc-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-156">This property is read-only.</span></span>|
|<span data-ttu-id="cd8fc-157">certificate</span><span class="sxs-lookup"><span data-stu-id="cd8fc-157">certificate</span></span>|<span data-ttu-id="cd8fc-158">String</span><span class="sxs-lookup"><span data-stu-id="cd8fc-158">String</span></span>|<span data-ttu-id="cd8fc-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd8fc-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd8fc-160">Response</span></span>
<span data-ttu-id="cd8fc-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-161">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd8fc-162">Пример</span><span class="sxs-lookup"><span data-stu-id="cd8fc-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd8fc-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd8fc-163">Request</span></span>
<span data-ttu-id="cd8fc-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd8fc-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd8fc-165">Response</span></span>
<span data-ttu-id="cd8fc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd8fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





