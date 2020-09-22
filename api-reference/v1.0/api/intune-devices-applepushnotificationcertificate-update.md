---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b26db969076896a8fb45dbe8d2c06894e50d0a9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009627"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="61a78-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="61a78-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="61a78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61a78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61a78-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61a78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61a78-106">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="61a78-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61a78-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="61a78-107">Prerequisites</span></span>
<span data-ttu-id="61a78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61a78-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61a78-110">Permission type</span></span>|<span data-ttu-id="61a78-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61a78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61a78-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61a78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61a78-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61a78-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61a78-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61a78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61a78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61a78-115">Not supported.</span></span>|
|<span data-ttu-id="61a78-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61a78-116">Application</span></span>|<span data-ttu-id="61a78-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61a78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61a78-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61a78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="61a78-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="61a78-119">Request headers</span></span>
|<span data-ttu-id="61a78-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61a78-120">Header</span></span>|<span data-ttu-id="61a78-121">Значение</span><span class="sxs-lookup"><span data-stu-id="61a78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61a78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61a78-122">Authorization</span></span>|<span data-ttu-id="61a78-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61a78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61a78-124">Accept</span><span class="sxs-lookup"><span data-stu-id="61a78-124">Accept</span></span>|<span data-ttu-id="61a78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61a78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61a78-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61a78-126">Request body</span></span>
<span data-ttu-id="61a78-127">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61a78-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="61a78-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="61a78-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="61a78-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="61a78-129">Property</span></span>|<span data-ttu-id="61a78-130">Тип</span><span class="sxs-lookup"><span data-stu-id="61a78-130">Type</span></span>|<span data-ttu-id="61a78-131">Описание</span><span class="sxs-lookup"><span data-stu-id="61a78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61a78-132">id</span><span class="sxs-lookup"><span data-stu-id="61a78-132">id</span></span>|<span data-ttu-id="61a78-133">String</span><span class="sxs-lookup"><span data-stu-id="61a78-133">String</span></span>|<span data-ttu-id="61a78-134">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="61a78-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="61a78-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="61a78-135">appleIdentifier</span></span>|<span data-ttu-id="61a78-136">String</span><span class="sxs-lookup"><span data-stu-id="61a78-136">String</span></span>|<span data-ttu-id="61a78-137">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="61a78-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="61a78-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="61a78-138">topicIdentifier</span></span>|<span data-ttu-id="61a78-139">String</span><span class="sxs-lookup"><span data-stu-id="61a78-139">String</span></span>|<span data-ttu-id="61a78-140">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="61a78-140">Topic Id.</span></span>|
|<span data-ttu-id="61a78-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61a78-141">lastModifiedDateTime</span></span>|<span data-ttu-id="61a78-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61a78-142">DateTimeOffset</span></span>|<span data-ttu-id="61a78-143">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="61a78-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="61a78-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="61a78-144">expirationDateTime</span></span>|<span data-ttu-id="61a78-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61a78-145">DateTimeOffset</span></span>|<span data-ttu-id="61a78-146">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="61a78-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="61a78-147">certificate</span><span class="sxs-lookup"><span data-stu-id="61a78-147">certificate</span></span>|<span data-ttu-id="61a78-148">String</span><span class="sxs-lookup"><span data-stu-id="61a78-148">String</span></span>|<span data-ttu-id="61a78-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="61a78-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="61a78-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="61a78-150">Response</span></span>
<span data-ttu-id="61a78-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61a78-151">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a78-152">Пример</span><span class="sxs-lookup"><span data-stu-id="61a78-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="61a78-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="61a78-153">Request</span></span>
<span data-ttu-id="61a78-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61a78-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="61a78-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="61a78-155">Response</span></span>
<span data-ttu-id="61a78-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61a78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```









