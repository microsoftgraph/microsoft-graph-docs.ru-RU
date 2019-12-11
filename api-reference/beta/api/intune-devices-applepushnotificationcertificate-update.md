---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8690f583bff395f54f31b56e3480e29e1815e462
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945293"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="3dadd-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3dadd-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="3dadd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dadd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dadd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3dadd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dadd-106">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="3dadd-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dadd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3dadd-107">Prerequisites</span></span>
<span data-ttu-id="3dadd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dadd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dadd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dadd-110">Permission type</span></span>|<span data-ttu-id="3dadd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dadd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dadd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dadd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3dadd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dadd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3dadd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dadd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dadd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dadd-115">Not supported.</span></span>|
|<span data-ttu-id="3dadd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3dadd-116">Application</span></span>|<span data-ttu-id="3dadd-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dadd-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dadd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dadd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="3dadd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3dadd-119">Request headers</span></span>
|<span data-ttu-id="3dadd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3dadd-120">Header</span></span>|<span data-ttu-id="3dadd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3dadd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dadd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3dadd-122">Authorization</span></span>|<span data-ttu-id="3dadd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dadd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dadd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3dadd-124">Accept</span></span>|<span data-ttu-id="3dadd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3dadd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dadd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3dadd-126">Request body</span></span>
<span data-ttu-id="3dadd-127">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3dadd-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="3dadd-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="3dadd-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="3dadd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dadd-129">Property</span></span>|<span data-ttu-id="3dadd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3dadd-130">Type</span></span>|<span data-ttu-id="3dadd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3dadd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dadd-132">id</span><span class="sxs-lookup"><span data-stu-id="3dadd-132">id</span></span>|<span data-ttu-id="3dadd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3dadd-133">String</span></span>|<span data-ttu-id="3dadd-134">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="3dadd-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="3dadd-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="3dadd-135">appleIdentifier</span></span>|<span data-ttu-id="3dadd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3dadd-136">String</span></span>|<span data-ttu-id="3dadd-137">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="3dadd-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="3dadd-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="3dadd-138">topicIdentifier</span></span>|<span data-ttu-id="3dadd-139">String</span><span class="sxs-lookup"><span data-stu-id="3dadd-139">String</span></span>|<span data-ttu-id="3dadd-140">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="3dadd-140">Topic Id.</span></span>|
|<span data-ttu-id="3dadd-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dadd-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3dadd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dadd-142">DateTimeOffset</span></span>|<span data-ttu-id="3dadd-143">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="3dadd-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="3dadd-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3dadd-144">expirationDateTime</span></span>|<span data-ttu-id="3dadd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dadd-145">DateTimeOffset</span></span>|<span data-ttu-id="3dadd-146">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="3dadd-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="3dadd-147">цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="3dadd-147">certificateUploadStatus</span></span>|<span data-ttu-id="3dadd-148">Строка</span><span class="sxs-lookup"><span data-stu-id="3dadd-148">String</span></span>|<span data-ttu-id="3dadd-149">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="3dadd-149">The certificate upload status.</span></span>|
|<span data-ttu-id="3dadd-150">цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="3dadd-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="3dadd-151">Строка</span><span class="sxs-lookup"><span data-stu-id="3dadd-151">String</span></span>|<span data-ttu-id="3dadd-152">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="3dadd-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="3dadd-153">certificate</span><span class="sxs-lookup"><span data-stu-id="3dadd-153">certificate</span></span>|<span data-ttu-id="3dadd-154">String</span><span class="sxs-lookup"><span data-stu-id="3dadd-154">String</span></span>|<span data-ttu-id="3dadd-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3dadd-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3dadd-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dadd-156">Response</span></span>
<span data-ttu-id="3dadd-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3dadd-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dadd-158">Пример</span><span class="sxs-lookup"><span data-stu-id="3dadd-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dadd-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dadd-159">Request</span></span>
<span data-ttu-id="3dadd-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3dadd-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="3dadd-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dadd-161">Response</span></span>
<span data-ttu-id="3dadd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3dadd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
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
```





