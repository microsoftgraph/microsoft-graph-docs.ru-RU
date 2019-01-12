---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6cc1b113b964dbc2f2ffdaae1e52639ec2463f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964839"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="e49bc-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e49bc-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="e49bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e49bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e49bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e49bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e49bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e49bc-107">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e49bc-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e49bc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e49bc-108">Prerequisites</span></span>
<span data-ttu-id="e49bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e49bc-111">Permission type</span></span>|<span data-ttu-id="e49bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e49bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e49bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e49bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e49bc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49bc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e49bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e49bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e49bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49bc-116">Not supported.</span></span>|
|<span data-ttu-id="e49bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e49bc-117">Application</span></span>|<span data-ttu-id="e49bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e49bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e49bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e49bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e49bc-120">Request headers</span></span>
|<span data-ttu-id="e49bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e49bc-121">Header</span></span>|<span data-ttu-id="e49bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e49bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e49bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e49bc-123">Authorization</span></span>|<span data-ttu-id="e49bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e49bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e49bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e49bc-125">Accept</span></span>|<span data-ttu-id="e49bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e49bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49bc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e49bc-127">Request body</span></span>
<span data-ttu-id="e49bc-128">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e49bc-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="e49bc-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e49bc-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="e49bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e49bc-130">Property</span></span>|<span data-ttu-id="e49bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e49bc-131">Type</span></span>|<span data-ttu-id="e49bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e49bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e49bc-133">id</span><span class="sxs-lookup"><span data-stu-id="e49bc-133">id</span></span>|<span data-ttu-id="e49bc-134">String</span><span class="sxs-lookup"><span data-stu-id="e49bc-134">String</span></span>|<span data-ttu-id="e49bc-135">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="e49bc-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="e49bc-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e49bc-136">appleIdentifier</span></span>|<span data-ttu-id="e49bc-137">String</span><span class="sxs-lookup"><span data-stu-id="e49bc-137">String</span></span>|<span data-ttu-id="e49bc-138">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="e49bc-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="e49bc-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="e49bc-139">topicIdentifier</span></span>|<span data-ttu-id="e49bc-140">String</span><span class="sxs-lookup"><span data-stu-id="e49bc-140">String</span></span>|<span data-ttu-id="e49bc-141">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="e49bc-141">Topic Id.</span></span>|
|<span data-ttu-id="e49bc-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e49bc-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e49bc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49bc-143">DateTimeOffset</span></span>|<span data-ttu-id="e49bc-144">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="e49bc-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e49bc-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e49bc-145">expirationDateTime</span></span>|<span data-ttu-id="e49bc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49bc-146">DateTimeOffset</span></span>|<span data-ttu-id="e49bc-147">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="e49bc-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e49bc-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="e49bc-148">certificateUploadStatus</span></span>|<span data-ttu-id="e49bc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="e49bc-149">String</span></span>|<span data-ttu-id="e49bc-150">Состояние загрузки сертификата.</span><span class="sxs-lookup"><span data-stu-id="e49bc-150">The certificate upload status.</span></span>|
|<span data-ttu-id="e49bc-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="e49bc-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="e49bc-152">Строка</span><span class="sxs-lookup"><span data-stu-id="e49bc-152">String</span></span>|<span data-ttu-id="e49bc-153">Не удалось причине отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="e49bc-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="e49bc-154">certificate</span><span class="sxs-lookup"><span data-stu-id="e49bc-154">certificate</span></span>|<span data-ttu-id="e49bc-155">String</span><span class="sxs-lookup"><span data-stu-id="e49bc-155">String</span></span>|<span data-ttu-id="e49bc-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e49bc-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e49bc-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49bc-157">Response</span></span>
<span data-ttu-id="e49bc-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e49bc-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e49bc-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e49bc-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="e49bc-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e49bc-160">Request</span></span>
<span data-ttu-id="e49bc-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e49bc-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 409

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="e49bc-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="e49bc-162">Response</span></span>
<span data-ttu-id="e49bc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e49bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





