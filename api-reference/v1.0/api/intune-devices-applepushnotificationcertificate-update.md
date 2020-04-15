---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34254267440a80701f27583a64df6dfae608655e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456829"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="0c271-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0c271-103">Update applePushNotificationCertificate</span></span>

<span data-ttu-id="0c271-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c271-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c271-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c271-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c271-106">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0c271-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c271-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0c271-107">Prerequisites</span></span>
<span data-ttu-id="0c271-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c271-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c271-110">Permission type</span></span>|<span data-ttu-id="0c271-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c271-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c271-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c271-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c271-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c271-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c271-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c271-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c271-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c271-115">Not supported.</span></span>|
|<span data-ttu-id="0c271-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c271-116">Application</span></span>|<span data-ttu-id="0c271-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c271-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c271-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c271-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="0c271-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c271-119">Request headers</span></span>
|<span data-ttu-id="0c271-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c271-120">Header</span></span>|<span data-ttu-id="0c271-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c271-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c271-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c271-122">Authorization</span></span>|<span data-ttu-id="0c271-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c271-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c271-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0c271-124">Accept</span></span>|<span data-ttu-id="0c271-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c271-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c271-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c271-126">Request body</span></span>
<span data-ttu-id="0c271-127">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c271-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="0c271-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0c271-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="0c271-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c271-129">Property</span></span>|<span data-ttu-id="0c271-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c271-130">Type</span></span>|<span data-ttu-id="0c271-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c271-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c271-132">id</span><span class="sxs-lookup"><span data-stu-id="0c271-132">id</span></span>|<span data-ttu-id="0c271-133">String</span><span class="sxs-lookup"><span data-stu-id="0c271-133">String</span></span>|<span data-ttu-id="0c271-134">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="0c271-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="0c271-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c271-135">appleIdentifier</span></span>|<span data-ttu-id="0c271-136">String</span><span class="sxs-lookup"><span data-stu-id="0c271-136">String</span></span>|<span data-ttu-id="0c271-137">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="0c271-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="0c271-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c271-138">topicIdentifier</span></span>|<span data-ttu-id="0c271-139">String</span><span class="sxs-lookup"><span data-stu-id="0c271-139">String</span></span>|<span data-ttu-id="0c271-140">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="0c271-140">Topic Id.</span></span>|
|<span data-ttu-id="0c271-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c271-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0c271-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c271-142">DateTimeOffset</span></span>|<span data-ttu-id="0c271-143">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="0c271-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="0c271-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c271-144">expirationDateTime</span></span>|<span data-ttu-id="0c271-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c271-145">DateTimeOffset</span></span>|<span data-ttu-id="0c271-146">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="0c271-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="0c271-147">certificate</span><span class="sxs-lookup"><span data-stu-id="0c271-147">certificate</span></span>|<span data-ttu-id="0c271-148">String</span><span class="sxs-lookup"><span data-stu-id="0c271-148">String</span></span>|<span data-ttu-id="0c271-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0c271-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0c271-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c271-150">Response</span></span>
<span data-ttu-id="0c271-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c271-151">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c271-152">Пример</span><span class="sxs-lookup"><span data-stu-id="0c271-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c271-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c271-153">Request</span></span>
<span data-ttu-id="0c271-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c271-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c271-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c271-155">Response</span></span>
<span data-ttu-id="0c271-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c271-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






