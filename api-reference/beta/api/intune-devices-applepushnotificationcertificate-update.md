---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecdbcf1bf5d33f8a7b6157d5b121e72b206fe4c9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310768"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="dacd7-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="dacd7-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="dacd7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dacd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dacd7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dacd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dacd7-106">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="dacd7-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dacd7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dacd7-107">Prerequisites</span></span>
<span data-ttu-id="dacd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dacd7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dacd7-110">Permission type</span></span>|<span data-ttu-id="dacd7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dacd7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dacd7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dacd7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dacd7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dacd7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dacd7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dacd7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dacd7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dacd7-115">Not supported.</span></span>|
|<span data-ttu-id="dacd7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dacd7-116">Application</span></span>|<span data-ttu-id="dacd7-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dacd7-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dacd7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dacd7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="dacd7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dacd7-119">Request headers</span></span>
|<span data-ttu-id="dacd7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dacd7-120">Header</span></span>|<span data-ttu-id="dacd7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dacd7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dacd7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dacd7-122">Authorization</span></span>|<span data-ttu-id="dacd7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dacd7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dacd7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dacd7-124">Accept</span></span>|<span data-ttu-id="dacd7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dacd7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dacd7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dacd7-126">Request body</span></span>
<span data-ttu-id="dacd7-127">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dacd7-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="dacd7-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="dacd7-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="dacd7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dacd7-129">Property</span></span>|<span data-ttu-id="dacd7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dacd7-130">Type</span></span>|<span data-ttu-id="dacd7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dacd7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dacd7-132">id</span><span class="sxs-lookup"><span data-stu-id="dacd7-132">id</span></span>|<span data-ttu-id="dacd7-133">String</span><span class="sxs-lookup"><span data-stu-id="dacd7-133">String</span></span>|<span data-ttu-id="dacd7-134">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="dacd7-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="dacd7-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="dacd7-135">appleIdentifier</span></span>|<span data-ttu-id="dacd7-136">String</span><span class="sxs-lookup"><span data-stu-id="dacd7-136">String</span></span>|<span data-ttu-id="dacd7-137">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="dacd7-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="dacd7-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="dacd7-138">topicIdentifier</span></span>|<span data-ttu-id="dacd7-139">String</span><span class="sxs-lookup"><span data-stu-id="dacd7-139">String</span></span>|<span data-ttu-id="dacd7-140">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="dacd7-140">Topic Id.</span></span>|
|<span data-ttu-id="dacd7-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dacd7-141">lastModifiedDateTime</span></span>|<span data-ttu-id="dacd7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacd7-142">DateTimeOffset</span></span>|<span data-ttu-id="dacd7-143">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="dacd7-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="dacd7-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dacd7-144">expirationDateTime</span></span>|<span data-ttu-id="dacd7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacd7-145">DateTimeOffset</span></span>|<span data-ttu-id="dacd7-146">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="dacd7-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="dacd7-147">цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="dacd7-147">certificateUploadStatus</span></span>|<span data-ttu-id="dacd7-148">String</span><span class="sxs-lookup"><span data-stu-id="dacd7-148">String</span></span>|<span data-ttu-id="dacd7-149">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="dacd7-149">The certificate upload status.</span></span>|
|<span data-ttu-id="dacd7-150">цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="dacd7-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="dacd7-151">String</span><span class="sxs-lookup"><span data-stu-id="dacd7-151">String</span></span>|<span data-ttu-id="dacd7-152">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="dacd7-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="dacd7-153">certificate</span><span class="sxs-lookup"><span data-stu-id="dacd7-153">certificate</span></span>|<span data-ttu-id="dacd7-154">String</span><span class="sxs-lookup"><span data-stu-id="dacd7-154">String</span></span>|<span data-ttu-id="dacd7-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dacd7-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dacd7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="dacd7-156">Response</span></span>
<span data-ttu-id="dacd7-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dacd7-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dacd7-158">Пример</span><span class="sxs-lookup"><span data-stu-id="dacd7-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="dacd7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="dacd7-159">Request</span></span>
<span data-ttu-id="dacd7-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dacd7-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dacd7-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="dacd7-161">Response</span></span>
<span data-ttu-id="dacd7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dacd7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






