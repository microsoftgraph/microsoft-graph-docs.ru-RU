---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf13a36bf2e690396afe90f8e2ddac6287b8fd3f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731122"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="a7a7c-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7a7c-103">Update deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="a7a7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7a7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7a7c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7a7c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7a7c-107">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a7a7c-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7a7c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a7a7c-108">Prerequisites</span></span>
<span data-ttu-id="a7a7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7a7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7a7c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7a7c-111">Permission type</span></span>|<span data-ttu-id="a7a7c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7a7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7a7c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7a7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7a7c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7a7c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a7a7c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7a7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7a7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-116">Not supported.</span></span>|
|<span data-ttu-id="a7a7c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7a7c-117">Application</span></span>|<span data-ttu-id="a7a7c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7a7c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7a7c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7a7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a7a7c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7a7c-120">Request headers</span></span>
|<span data-ttu-id="a7a7c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7a7c-121">Header</span></span>|<span data-ttu-id="a7a7c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7a7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7a7c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7a7c-123">Authorization</span></span>|<span data-ttu-id="a7a7c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7a7c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7a7c-125">Accept</span></span>|<span data-ttu-id="a7a7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7a7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7a7c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7a7c-127">Request body</span></span>
<span data-ttu-id="a7a7c-128">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="a7a7c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a7a7c-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="a7a7c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7a7c-130">Property</span></span>|<span data-ttu-id="a7a7c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a7a7c-131">Type</span></span>|<span data-ttu-id="a7a7c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a7a7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7a7c-133">id</span><span class="sxs-lookup"><span data-stu-id="a7a7c-133">id</span></span>|<span data-ttu-id="a7a7c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a7a7c-134">String</span></span>|<span data-ttu-id="a7a7c-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-135">UUID for the object</span></span>|
|<span data-ttu-id="a7a7c-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a7a7c-136">eventDateTime</span></span>|<span data-ttu-id="a7a7c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7a7c-137">DateTimeOffset</span></span>|<span data-ttu-id="a7a7c-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="a7a7c-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="a7a7c-139">correlationId</span></span>|<span data-ttu-id="a7a7c-140">String</span><span class="sxs-lookup"><span data-stu-id="a7a7c-140">String</span></span>|<span data-ttu-id="a7a7c-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="a7a7c-142">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="a7a7c-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="a7a7c-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a7a7c-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="a7a7c-144">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="a7a7c-145">eventName</span><span class="sxs-lookup"><span data-stu-id="a7a7c-145">eventName</span></span>|<span data-ttu-id="a7a7c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a7a7c-146">String</span></span>|<span data-ttu-id="a7a7c-147">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="a7a7c-148">Это необязательное поле</span><span class="sxs-lookup"><span data-stu-id="a7a7c-148">It is an Optional field</span></span>|
|<span data-ttu-id="a7a7c-149">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="a7a7c-149">additionalInformation</span></span>|<span data-ttu-id="a7a7c-150">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a7a7c-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a7a7c-151">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок</span><span class="sxs-lookup"><span data-stu-id="a7a7c-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="a7a7c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7a7c-152">Response</span></span>
<span data-ttu-id="a7a7c-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7a7c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="a7a7c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7a7c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7a7c-155">Request</span></span>
<span data-ttu-id="a7a7c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7a7c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7a7c-157">Response</span></span>
<span data-ttu-id="a7a7c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7a7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





