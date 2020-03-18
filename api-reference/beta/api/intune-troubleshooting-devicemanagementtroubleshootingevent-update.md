---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f19fbd92c0abc6ff00fb3025956485afa2782451
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800167"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="18cc6-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="18cc6-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="18cc6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18cc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18cc6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18cc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18cc6-106">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="18cc6-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18cc6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="18cc6-107">Prerequisites</span></span>
<span data-ttu-id="18cc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18cc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18cc6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18cc6-110">Permission type</span></span>|<span data-ttu-id="18cc6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18cc6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18cc6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18cc6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18cc6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18cc6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="18cc6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18cc6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18cc6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18cc6-115">Not supported.</span></span>|
|<span data-ttu-id="18cc6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="18cc6-116">Application</span></span>|<span data-ttu-id="18cc6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18cc6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18cc6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18cc6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="18cc6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18cc6-119">Request headers</span></span>
|<span data-ttu-id="18cc6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18cc6-120">Header</span></span>|<span data-ttu-id="18cc6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18cc6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18cc6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18cc6-122">Authorization</span></span>|<span data-ttu-id="18cc6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18cc6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18cc6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18cc6-124">Accept</span></span>|<span data-ttu-id="18cc6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18cc6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18cc6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18cc6-126">Request body</span></span>
<span data-ttu-id="18cc6-127">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18cc6-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="18cc6-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="18cc6-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="18cc6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18cc6-129">Property</span></span>|<span data-ttu-id="18cc6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18cc6-130">Type</span></span>|<span data-ttu-id="18cc6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18cc6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18cc6-132">id</span><span class="sxs-lookup"><span data-stu-id="18cc6-132">id</span></span>|<span data-ttu-id="18cc6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="18cc6-133">String</span></span>|<span data-ttu-id="18cc6-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="18cc6-134">UUID for the object</span></span>|
|<span data-ttu-id="18cc6-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="18cc6-135">eventDateTime</span></span>|<span data-ttu-id="18cc6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18cc6-136">DateTimeOffset</span></span>|<span data-ttu-id="18cc6-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="18cc6-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="18cc6-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="18cc6-138">correlationId</span></span>|<span data-ttu-id="18cc6-139">String</span><span class="sxs-lookup"><span data-stu-id="18cc6-139">String</span></span>|<span data-ttu-id="18cc6-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="18cc6-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="18cc6-141">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="18cc6-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="18cc6-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="18cc6-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="18cc6-143">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="18cc6-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="18cc6-144">eventName</span><span class="sxs-lookup"><span data-stu-id="18cc6-144">eventName</span></span>|<span data-ttu-id="18cc6-145">String</span><span class="sxs-lookup"><span data-stu-id="18cc6-145">String</span></span>|<span data-ttu-id="18cc6-146">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="18cc6-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="18cc6-147">Это необязательное поле</span><span class="sxs-lookup"><span data-stu-id="18cc6-147">It is an Optional field</span></span>|
|<span data-ttu-id="18cc6-148">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="18cc6-148">additionalInformation</span></span>|<span data-ttu-id="18cc6-149">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="18cc6-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="18cc6-150">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="18cc6-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="18cc6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="18cc6-151">Response</span></span>
<span data-ttu-id="18cc6-152">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18cc6-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18cc6-153">Пример</span><span class="sxs-lookup"><span data-stu-id="18cc6-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="18cc6-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="18cc6-154">Request</span></span>
<span data-ttu-id="18cc6-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18cc6-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 852

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="18cc6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="18cc6-156">Response</span></span>
<span data-ttu-id="18cc6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18cc6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




