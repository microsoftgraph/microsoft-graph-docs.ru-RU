---
title: Обновление объекта applePushNotificationCertificate
description: Обновление свойств объекта applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bd100c743a79cb5a622e047dd4dcdac8441f6eb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956942"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="2fab7-103">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="2fab7-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="2fab7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fab7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fab7-105">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2fab7-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fab7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2fab7-106">Prerequisites</span></span>
<span data-ttu-id="2fab7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fab7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fab7-109">Permission type</span></span>|<span data-ttu-id="2fab7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fab7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fab7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fab7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2fab7-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fab7-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2fab7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fab7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fab7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fab7-114">Not supported.</span></span>|
|<span data-ttu-id="2fab7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fab7-115">Application</span></span>|<span data-ttu-id="2fab7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fab7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fab7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fab7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="2fab7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fab7-118">Request headers</span></span>
|<span data-ttu-id="2fab7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fab7-119">Header</span></span>|<span data-ttu-id="2fab7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2fab7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fab7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fab7-121">Authorization</span></span>|<span data-ttu-id="2fab7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fab7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fab7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2fab7-123">Accept</span></span>|<span data-ttu-id="2fab7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2fab7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fab7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fab7-125">Request body</span></span>
<span data-ttu-id="2fab7-126">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fab7-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="2fab7-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2fab7-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="2fab7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fab7-128">Property</span></span>|<span data-ttu-id="2fab7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2fab7-129">Type</span></span>|<span data-ttu-id="2fab7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2fab7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fab7-131">id</span><span class="sxs-lookup"><span data-stu-id="2fab7-131">id</span></span>|<span data-ttu-id="2fab7-132">String</span><span class="sxs-lookup"><span data-stu-id="2fab7-132">String</span></span>|<span data-ttu-id="2fab7-133">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="2fab7-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="2fab7-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="2fab7-134">appleIdentifier</span></span>|<span data-ttu-id="2fab7-135">String</span><span class="sxs-lookup"><span data-stu-id="2fab7-135">String</span></span>|<span data-ttu-id="2fab7-136">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="2fab7-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="2fab7-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="2fab7-137">topicIdentifier</span></span>|<span data-ttu-id="2fab7-138">String</span><span class="sxs-lookup"><span data-stu-id="2fab7-138">String</span></span>|<span data-ttu-id="2fab7-139">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="2fab7-139">Topic Id.</span></span>|
|<span data-ttu-id="2fab7-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fab7-140">lastModifiedDateTime</span></span>|<span data-ttu-id="2fab7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fab7-141">DateTimeOffset</span></span>|<span data-ttu-id="2fab7-142">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="2fab7-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="2fab7-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2fab7-143">expirationDateTime</span></span>|<span data-ttu-id="2fab7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fab7-144">DateTimeOffset</span></span>|<span data-ttu-id="2fab7-145">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="2fab7-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="2fab7-146">certificate</span><span class="sxs-lookup"><span data-stu-id="2fab7-146">certificate</span></span>|<span data-ttu-id="2fab7-147">String</span><span class="sxs-lookup"><span data-stu-id="2fab7-147">String</span></span>|<span data-ttu-id="2fab7-148">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2fab7-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2fab7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fab7-149">Response</span></span>
<span data-ttu-id="2fab7-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2fab7-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fab7-151">Пример</span><span class="sxs-lookup"><span data-stu-id="2fab7-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fab7-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fab7-152">Request</span></span>
<span data-ttu-id="2fab7-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fab7-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fab7-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fab7-154">Response</span></span>
<span data-ttu-id="2fab7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fab7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



