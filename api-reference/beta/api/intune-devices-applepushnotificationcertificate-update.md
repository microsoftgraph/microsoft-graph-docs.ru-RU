---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e14e4056f0428548e0b910c8647dc4442efe4abd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397486"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="a8e9a-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a8e9a-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="a8e9a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8e9a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8e9a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8e9a-107">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="a8e9a-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8e9a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8e9a-108">Prerequisites</span></span>
<span data-ttu-id="a8e9a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8e9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a8e9a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8e9a-111">Permission type</span></span>|<span data-ttu-id="a8e9a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8e9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8e9a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8e9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8e9a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e9a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a8e9a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8e9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8e9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-116">Not supported.</span></span>|
|<span data-ttu-id="a8e9a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8e9a-117">Application</span></span>|<span data-ttu-id="a8e9a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8e9a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8e9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="a8e9a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8e9a-120">Request headers</span></span>
|<span data-ttu-id="a8e9a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8e9a-121">Header</span></span>|<span data-ttu-id="a8e9a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8e9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8e9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8e9a-123">Authorization</span></span>|<span data-ttu-id="a8e9a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a8e9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8e9a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8e9a-125">Accept</span></span>|<span data-ttu-id="a8e9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8e9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8e9a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8e9a-127">Request body</span></span>
<span data-ttu-id="a8e9a-128">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="a8e9a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="a8e9a-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="a8e9a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8e9a-130">Property</span></span>|<span data-ttu-id="a8e9a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a8e9a-131">Type</span></span>|<span data-ttu-id="a8e9a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e9a-133">id</span><span class="sxs-lookup"><span data-stu-id="a8e9a-133">id</span></span>|<span data-ttu-id="a8e9a-134">String</span><span class="sxs-lookup"><span data-stu-id="a8e9a-134">String</span></span>|<span data-ttu-id="a8e9a-135">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="a8e9a-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="a8e9a-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8e9a-136">appleIdentifier</span></span>|<span data-ttu-id="a8e9a-137">String</span><span class="sxs-lookup"><span data-stu-id="a8e9a-137">String</span></span>|<span data-ttu-id="a8e9a-138">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="a8e9a-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8e9a-139">topicIdentifier</span></span>|<span data-ttu-id="a8e9a-140">String</span><span class="sxs-lookup"><span data-stu-id="a8e9a-140">String</span></span>|<span data-ttu-id="a8e9a-141">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-141">Topic Id.</span></span>|
|<span data-ttu-id="a8e9a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e9a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a8e9a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e9a-143">DateTimeOffset</span></span>|<span data-ttu-id="a8e9a-144">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a8e9a-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e9a-145">expirationDateTime</span></span>|<span data-ttu-id="a8e9a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e9a-146">DateTimeOffset</span></span>|<span data-ttu-id="a8e9a-147">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="a8e9a-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a8e9a-148">certificateUploadStatus</span></span>|<span data-ttu-id="a8e9a-149">String</span><span class="sxs-lookup"><span data-stu-id="a8e9a-149">String</span></span>|<span data-ttu-id="a8e9a-150">Состояние загрузки сертификата.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-150">The certificate upload status.</span></span>|
|<span data-ttu-id="a8e9a-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="a8e9a-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="a8e9a-152">String</span><span class="sxs-lookup"><span data-stu-id="a8e9a-152">String</span></span>|<span data-ttu-id="a8e9a-153">Не удалось причине отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="a8e9a-154">certificate</span><span class="sxs-lookup"><span data-stu-id="a8e9a-154">certificate</span></span>|<span data-ttu-id="a8e9a-155">String</span><span class="sxs-lookup"><span data-stu-id="a8e9a-155">String</span></span>|<span data-ttu-id="a8e9a-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a8e9a-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a8e9a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8e9a-157">Response</span></span>
<span data-ttu-id="a8e9a-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e9a-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a8e9a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8e9a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8e9a-160">Request</span></span>
<span data-ttu-id="a8e9a-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8e9a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8e9a-162">Response</span></span>
<span data-ttu-id="a8e9a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a8e9a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




