---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b81a3997902d2fae346d4ede7bfd701e8eae2ef3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723247"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="18975-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="18975-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="18975-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18975-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18975-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18975-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18975-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18975-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18975-107">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="18975-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18975-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="18975-108">Prerequisites</span></span>
<span data-ttu-id="18975-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18975-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18975-111">Permission type</span></span>|<span data-ttu-id="18975-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18975-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18975-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18975-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18975-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18975-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18975-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18975-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18975-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18975-116">Not supported.</span></span>|
|<span data-ttu-id="18975-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18975-117">Application</span></span>|<span data-ttu-id="18975-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18975-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18975-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18975-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="18975-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18975-120">Request headers</span></span>
|<span data-ttu-id="18975-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18975-121">Header</span></span>|<span data-ttu-id="18975-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18975-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18975-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18975-123">Authorization</span></span>|<span data-ttu-id="18975-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18975-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18975-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18975-125">Accept</span></span>|<span data-ttu-id="18975-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18975-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18975-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18975-127">Request body</span></span>
<span data-ttu-id="18975-128">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18975-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="18975-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="18975-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="18975-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18975-130">Property</span></span>|<span data-ttu-id="18975-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18975-131">Type</span></span>|<span data-ttu-id="18975-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18975-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18975-133">id</span><span class="sxs-lookup"><span data-stu-id="18975-133">id</span></span>|<span data-ttu-id="18975-134">Строка</span><span class="sxs-lookup"><span data-stu-id="18975-134">String</span></span>|<span data-ttu-id="18975-135">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="18975-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="18975-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="18975-136">appleIdentifier</span></span>|<span data-ttu-id="18975-137">String</span><span class="sxs-lookup"><span data-stu-id="18975-137">String</span></span>|<span data-ttu-id="18975-138">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="18975-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="18975-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="18975-139">topicIdentifier</span></span>|<span data-ttu-id="18975-140">String</span><span class="sxs-lookup"><span data-stu-id="18975-140">String</span></span>|<span data-ttu-id="18975-141">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="18975-141">Topic Id.</span></span>|
|<span data-ttu-id="18975-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18975-142">lastModifiedDateTime</span></span>|<span data-ttu-id="18975-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18975-143">DateTimeOffset</span></span>|<span data-ttu-id="18975-144">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="18975-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="18975-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18975-145">expirationDateTime</span></span>|<span data-ttu-id="18975-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18975-146">DateTimeOffset</span></span>|<span data-ttu-id="18975-147">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="18975-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="18975-148">цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="18975-148">certificateUploadStatus</span></span>|<span data-ttu-id="18975-149">Строка</span><span class="sxs-lookup"><span data-stu-id="18975-149">String</span></span>|<span data-ttu-id="18975-150">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="18975-150">The certificate upload status.</span></span>|
|<span data-ttu-id="18975-151">цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="18975-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="18975-152">Строка</span><span class="sxs-lookup"><span data-stu-id="18975-152">String</span></span>|<span data-ttu-id="18975-153">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="18975-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="18975-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="18975-154">certificateSerialNumber</span></span>|<span data-ttu-id="18975-155">Строка</span><span class="sxs-lookup"><span data-stu-id="18975-155">String</span></span>|<span data-ttu-id="18975-156">Серийный номер сертификата.</span><span class="sxs-lookup"><span data-stu-id="18975-156">Certificate serial number.</span></span> <span data-ttu-id="18975-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18975-157">This property is read-only.</span></span>|
|<span data-ttu-id="18975-158">certificate</span><span class="sxs-lookup"><span data-stu-id="18975-158">certificate</span></span>|<span data-ttu-id="18975-159">String</span><span class="sxs-lookup"><span data-stu-id="18975-159">String</span></span>|<span data-ttu-id="18975-160">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="18975-160">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="18975-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="18975-161">Response</span></span>
<span data-ttu-id="18975-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18975-162">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18975-163">Пример</span><span class="sxs-lookup"><span data-stu-id="18975-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="18975-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="18975-164">Request</span></span>
<span data-ttu-id="18975-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18975-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18975-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="18975-166">Response</span></span>
<span data-ttu-id="18975-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18975-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





