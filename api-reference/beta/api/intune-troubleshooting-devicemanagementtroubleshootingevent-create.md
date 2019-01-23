---
title: Создание объекта deviceManagementTroubleshootingEvent
description: Создание объекта deviceManagementTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b88d0474c7b332b91d447c963fa2a983b64035
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404430"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="7948a-103">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7948a-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="7948a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7948a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7948a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7948a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7948a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7948a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7948a-107">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7948a-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7948a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7948a-108">Prerequisites</span></span>
<span data-ttu-id="7948a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7948a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7948a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7948a-111">Permission type</span></span>|<span data-ttu-id="7948a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7948a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7948a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7948a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7948a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7948a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7948a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7948a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7948a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7948a-116">Not supported.</span></span>|
|<span data-ttu-id="7948a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7948a-117">Application</span></span>|<span data-ttu-id="7948a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7948a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7948a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7948a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="7948a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7948a-120">Request headers</span></span>
|<span data-ttu-id="7948a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7948a-121">Header</span></span>|<span data-ttu-id="7948a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7948a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7948a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7948a-123">Authorization</span></span>|<span data-ttu-id="7948a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7948a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7948a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7948a-125">Accept</span></span>|<span data-ttu-id="7948a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7948a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7948a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7948a-127">Request body</span></span>
<span data-ttu-id="7948a-128">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7948a-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="7948a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="7948a-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="7948a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7948a-130">Property</span></span>|<span data-ttu-id="7948a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7948a-131">Type</span></span>|<span data-ttu-id="7948a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7948a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7948a-133">id</span><span class="sxs-lookup"><span data-stu-id="7948a-133">id</span></span>|<span data-ttu-id="7948a-134">String</span><span class="sxs-lookup"><span data-stu-id="7948a-134">String</span></span>|<span data-ttu-id="7948a-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="7948a-135">UUID for the object</span></span>|
|<span data-ttu-id="7948a-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7948a-136">eventDateTime</span></span>|<span data-ttu-id="7948a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7948a-137">DateTimeOffset</span></span>|<span data-ttu-id="7948a-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="7948a-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="7948a-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="7948a-139">correlationId</span></span>|<span data-ttu-id="7948a-140">String</span><span class="sxs-lookup"><span data-stu-id="7948a-140">String</span></span>|<span data-ttu-id="7948a-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="7948a-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="7948a-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7948a-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="7948a-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7948a-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="7948a-144">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="7948a-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="7948a-145">элемент eventName</span><span class="sxs-lookup"><span data-stu-id="7948a-145">eventName</span></span>|<span data-ttu-id="7948a-146">String</span><span class="sxs-lookup"><span data-stu-id="7948a-146">String</span></span>|<span data-ttu-id="7948a-147">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="7948a-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="7948a-148">Это необязательное поле</span><span class="sxs-lookup"><span data-stu-id="7948a-148">It is an Optional field</span></span>|
|<span data-ttu-id="7948a-149">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="7948a-149">additionalInformation</span></span>|<span data-ttu-id="7948a-150">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7948a-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7948a-151">Набор ключ строки и пар строковое значение которой содержатся дополнительные сведения на события Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="7948a-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="7948a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7948a-152">Response</span></span>
<span data-ttu-id="7948a-153">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7948a-153">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7948a-154">Пример</span><span class="sxs-lookup"><span data-stu-id="7948a-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="7948a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="7948a-155">Request</span></span>
<span data-ttu-id="7948a-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7948a-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="7948a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="7948a-157">Response</span></span>
<span data-ttu-id="7948a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7948a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




