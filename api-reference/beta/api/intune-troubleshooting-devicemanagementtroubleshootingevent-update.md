---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd948ef890605aae399dd4d9a300ef949136f78d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134097"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="c19a0-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c19a0-103">Update deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="c19a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c19a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c19a0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c19a0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c19a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c19a0-107">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c19a0-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c19a0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c19a0-108">Prerequisites</span></span>
<span data-ttu-id="c19a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c19a0-111">Permission type</span></span>|<span data-ttu-id="c19a0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c19a0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c19a0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c19a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c19a0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19a0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c19a0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c19a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c19a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19a0-116">Not supported.</span></span>|
|<span data-ttu-id="c19a0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c19a0-117">Application</span></span>|<span data-ttu-id="c19a0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19a0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c19a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c19a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c19a0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c19a0-120">Request headers</span></span>
|<span data-ttu-id="c19a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c19a0-121">Header</span></span>|<span data-ttu-id="c19a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c19a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c19a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c19a0-123">Authorization</span></span>|<span data-ttu-id="c19a0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c19a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c19a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c19a0-125">Accept</span></span>|<span data-ttu-id="c19a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c19a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c19a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c19a0-127">Request body</span></span>
<span data-ttu-id="c19a0-128">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c19a0-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="c19a0-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c19a0-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="c19a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c19a0-130">Property</span></span>|<span data-ttu-id="c19a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c19a0-131">Type</span></span>|<span data-ttu-id="c19a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c19a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c19a0-133">id</span><span class="sxs-lookup"><span data-stu-id="c19a0-133">id</span></span>|<span data-ttu-id="c19a0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c19a0-134">String</span></span>|<span data-ttu-id="c19a0-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c19a0-135">UUID for the object</span></span>|
|<span data-ttu-id="c19a0-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c19a0-136">eventDateTime</span></span>|<span data-ttu-id="c19a0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c19a0-137">DateTimeOffset</span></span>|<span data-ttu-id="c19a0-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="c19a0-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="c19a0-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="c19a0-139">correlationId</span></span>|<span data-ttu-id="c19a0-140">String</span><span class="sxs-lookup"><span data-stu-id="c19a0-140">String</span></span>|<span data-ttu-id="c19a0-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="c19a0-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="c19a0-142">устранение неполадокErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c19a0-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c19a0-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c19a0-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c19a0-144">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="c19a0-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="c19a0-145">eventName</span><span class="sxs-lookup"><span data-stu-id="c19a0-145">eventName</span></span>|<span data-ttu-id="c19a0-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c19a0-146">String</span></span>|<span data-ttu-id="c19a0-147">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="c19a0-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c19a0-148">Это необязательный поле</span><span class="sxs-lookup"><span data-stu-id="c19a0-148">It is an Optional field</span></span>|
|<span data-ttu-id="c19a0-149">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="c19a0-149">additionalInformation</span></span>|<span data-ttu-id="c19a0-150">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c19a0-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c19a0-151">Набор пар значений ключа строки и строк, которые предоставляют дополнительные сведения о событии устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="c19a0-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="c19a0-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c19a0-152">Response</span></span>
<span data-ttu-id="c19a0-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c19a0-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c19a0-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c19a0-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c19a0-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c19a0-155">Request</span></span>
<span data-ttu-id="c19a0-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c19a0-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c19a0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c19a0-157">Response</span></span>
<span data-ttu-id="c19a0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c19a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




