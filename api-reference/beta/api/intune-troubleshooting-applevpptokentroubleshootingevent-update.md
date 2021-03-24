---
title: Обновление appleVppTokenTroubleshootingEvent
description: Обновление свойств объекта appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57bd6638e03dea35a47fc894c3789ea2004a21f5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123422"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="3cd78-103">Обновление appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3cd78-103">Update appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="3cd78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cd78-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cd78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cd78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3cd78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cd78-107">Обновление свойств объекта [appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3cd78-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cd78-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3cd78-108">Prerequisites</span></span>
<span data-ttu-id="3cd78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cd78-111">Permission type</span></span>|<span data-ttu-id="3cd78-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cd78-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cd78-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cd78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cd78-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd78-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3cd78-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cd78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cd78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cd78-116">Not supported.</span></span>|
|<span data-ttu-id="3cd78-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3cd78-117">Application</span></span>|<span data-ttu-id="3cd78-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd78-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cd78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cd78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3cd78-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3cd78-120">Request headers</span></span>
|<span data-ttu-id="3cd78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cd78-121">Header</span></span>|<span data-ttu-id="3cd78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3cd78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cd78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cd78-123">Authorization</span></span>|<span data-ttu-id="3cd78-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cd78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cd78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3cd78-125">Accept</span></span>|<span data-ttu-id="3cd78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cd78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cd78-127">Request body</span></span>
<span data-ttu-id="3cd78-128">В теле запроса поставляем представление JSON для [объекта appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3cd78-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="3cd78-129">В следующей таблице показаны свойства, необходимые при создании [appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3cd78-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="3cd78-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cd78-130">Property</span></span>|<span data-ttu-id="3cd78-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3cd78-131">Type</span></span>|<span data-ttu-id="3cd78-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3cd78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd78-133">id</span><span class="sxs-lookup"><span data-stu-id="3cd78-133">id</span></span>|<span data-ttu-id="3cd78-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3cd78-134">String</span></span>|<span data-ttu-id="3cd78-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3cd78-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3cd78-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd78-136">eventDateTime</span></span>|<span data-ttu-id="3cd78-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd78-137">DateTimeOffset</span></span>|<span data-ttu-id="3cd78-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="3cd78-138">Time when the event occurred .</span></span> <span data-ttu-id="3cd78-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3cd78-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3cd78-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="3cd78-140">correlationId</span></span>|<span data-ttu-id="3cd78-141">String</span><span class="sxs-lookup"><span data-stu-id="3cd78-141">String</span></span>|<span data-ttu-id="3cd78-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="3cd78-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="3cd78-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3cd78-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3cd78-144">устранение неполадокErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3cd78-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3cd78-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3cd78-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3cd78-146">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="3cd78-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="3cd78-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3cd78-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3cd78-148">eventName</span><span class="sxs-lookup"><span data-stu-id="3cd78-148">eventName</span></span>|<span data-ttu-id="3cd78-149">Строка</span><span class="sxs-lookup"><span data-stu-id="3cd78-149">String</span></span>|<span data-ttu-id="3cd78-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="3cd78-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="3cd78-151">Это необязательный поле, унаследованный от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3cd78-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3cd78-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="3cd78-152">additionalInformation</span></span>|<span data-ttu-id="3cd78-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3cd78-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3cd78-154">Набор пар строк и пар значений строк, которые предоставляют дополнительные сведения о событии устранения неполадок, унаследованных от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3cd78-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3cd78-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="3cd78-155">tokenId</span></span>|<span data-ttu-id="3cd78-156">Строка</span><span class="sxs-lookup"><span data-stu-id="3cd78-156">String</span></span>|<span data-ttu-id="3cd78-157">Идентификатор маркера программы покупки тома Apple.</span><span class="sxs-lookup"><span data-stu-id="3cd78-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="3cd78-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cd78-158">Response</span></span>
<span data-ttu-id="3cd78-159">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3cd78-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd78-160">Пример</span><span class="sxs-lookup"><span data-stu-id="3cd78-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cd78-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cd78-161">Request</span></span>
<span data-ttu-id="3cd78-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cd78-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
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
  ],
  "tokenId": "Token Id value"
}
```

### <a name="response"></a><span data-ttu-id="3cd78-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cd78-163">Response</span></span>
<span data-ttu-id="3cd78-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cd78-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "09295f26-5f26-0929-265f-2909265f2909",
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
  ],
  "tokenId": "Token Id value"
}
```




