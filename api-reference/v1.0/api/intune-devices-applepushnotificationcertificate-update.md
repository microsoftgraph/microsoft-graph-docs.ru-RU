---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b0726ba347e9dd2c74e2c35c16f60935ac39465
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884891"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="d7283-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d7283-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="d7283-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7283-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7283-105">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d7283-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7283-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d7283-106">Prerequisites</span></span>
<span data-ttu-id="d7283-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7283-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7283-109">Permission type</span></span>|<span data-ttu-id="d7283-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7283-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7283-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7283-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7283-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7283-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d7283-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7283-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7283-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7283-114">Not supported.</span></span>|
|<span data-ttu-id="d7283-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7283-115">Application</span></span>|<span data-ttu-id="d7283-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7283-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7283-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7283-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="d7283-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7283-118">Request headers</span></span>
|<span data-ttu-id="d7283-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7283-119">Header</span></span>|<span data-ttu-id="d7283-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d7283-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7283-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7283-121">Authorization</span></span>|<span data-ttu-id="d7283-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7283-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7283-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d7283-123">Accept</span></span>|<span data-ttu-id="d7283-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d7283-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7283-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d7283-125">Request body</span></span>
<span data-ttu-id="d7283-126">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7283-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="d7283-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d7283-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="d7283-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7283-128">Property</span></span>|<span data-ttu-id="d7283-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d7283-129">Type</span></span>|<span data-ttu-id="d7283-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d7283-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7283-131">id</span><span class="sxs-lookup"><span data-stu-id="d7283-131">id</span></span>|<span data-ttu-id="d7283-132">String</span><span class="sxs-lookup"><span data-stu-id="d7283-132">String</span></span>|<span data-ttu-id="d7283-133">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="d7283-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="d7283-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7283-134">appleIdentifier</span></span>|<span data-ttu-id="d7283-135">String</span><span class="sxs-lookup"><span data-stu-id="d7283-135">String</span></span>|<span data-ttu-id="d7283-136">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="d7283-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="d7283-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7283-137">topicIdentifier</span></span>|<span data-ttu-id="d7283-138">String</span><span class="sxs-lookup"><span data-stu-id="d7283-138">String</span></span>|<span data-ttu-id="d7283-139">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="d7283-139">Topic Id.</span></span>|
|<span data-ttu-id="d7283-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7283-140">lastModifiedDateTime</span></span>|<span data-ttu-id="d7283-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7283-141">DateTimeOffset</span></span>|<span data-ttu-id="d7283-142">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="d7283-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d7283-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d7283-143">expirationDateTime</span></span>|<span data-ttu-id="d7283-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7283-144">DateTimeOffset</span></span>|<span data-ttu-id="d7283-145">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="d7283-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d7283-146">certificate</span><span class="sxs-lookup"><span data-stu-id="d7283-146">certificate</span></span>|<span data-ttu-id="d7283-147">String</span><span class="sxs-lookup"><span data-stu-id="d7283-147">String</span></span>|<span data-ttu-id="d7283-148">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d7283-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d7283-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7283-149">Response</span></span>
<span data-ttu-id="d7283-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7283-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7283-151">Пример</span><span class="sxs-lookup"><span data-stu-id="d7283-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7283-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7283-152">Request</span></span>
<span data-ttu-id="d7283-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7283-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7283-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7283-154">Response</span></span>
<span data-ttu-id="d7283-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7283-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



