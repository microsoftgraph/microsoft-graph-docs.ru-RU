---
title: Обновление Апплевпптокентраублешутинжевент
description: Обновление свойств объекта Апплевпптокентраублешутинжевент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d55c771aabcc7bd83f35b7c8f58acdac5d198ac4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448160"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="3ec5c-103">Обновление Апплевпптокентраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="3ec5c-103">Update appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="3ec5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ec5c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ec5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ec5c-107">Обновление свойств объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="3ec5c-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ec5c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ec5c-108">Prerequisites</span></span>
<span data-ttu-id="3ec5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec5c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec5c-111">Permission type</span></span>|<span data-ttu-id="3ec5c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ec5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ec5c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ec5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ec5c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec5c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3ec5c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ec5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ec5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-116">Not supported.</span></span>|
|<span data-ttu-id="3ec5c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ec5c-117">Application</span></span>|<span data-ttu-id="3ec5c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec5c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ec5c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ec5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3ec5c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ec5c-120">Request headers</span></span>
|<span data-ttu-id="3ec5c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ec5c-121">Header</span></span>|<span data-ttu-id="3ec5c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ec5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ec5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec5c-123">Authorization</span></span>|<span data-ttu-id="3ec5c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ec5c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ec5c-125">Accept</span></span>|<span data-ttu-id="3ec5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ec5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec5c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ec5c-127">Request body</span></span>
<span data-ttu-id="3ec5c-128">В тексте запроса добавьте представление объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="3ec5c-129">В следующей таблице приведены свойства, необходимые при создании [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3ec5c-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="3ec5c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ec5c-130">Property</span></span>|<span data-ttu-id="3ec5c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3ec5c-131">Type</span></span>|<span data-ttu-id="3ec5c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ec5c-133">id</span><span class="sxs-lookup"><span data-stu-id="3ec5c-133">id</span></span>|<span data-ttu-id="3ec5c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3ec5c-134">String</span></span>|<span data-ttu-id="3ec5c-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3ec5c-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3ec5c-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3ec5c-136">eventDateTime</span></span>|<span data-ttu-id="3ec5c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ec5c-137">DateTimeOffset</span></span>|<span data-ttu-id="3ec5c-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-138">Time when the event occurred .</span></span> <span data-ttu-id="3ec5c-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3ec5c-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3ec5c-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="3ec5c-140">correlationId</span></span>|<span data-ttu-id="3ec5c-141">String</span><span class="sxs-lookup"><span data-stu-id="3ec5c-141">String</span></span>|<span data-ttu-id="3ec5c-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="3ec5c-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3ec5c-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3ec5c-144">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="3ec5c-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3ec5c-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3ec5c-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3ec5c-146">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="3ec5c-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3ec5c-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3ec5c-148">eventName</span><span class="sxs-lookup"><span data-stu-id="3ec5c-148">eventName</span></span>|<span data-ttu-id="3ec5c-149">String</span><span class="sxs-lookup"><span data-stu-id="3ec5c-149">String</span></span>|<span data-ttu-id="3ec5c-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="3ec5c-151">Это необязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3ec5c-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3ec5c-152">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="3ec5c-152">additionalInformation</span></span>|<span data-ttu-id="3ec5c-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3ec5c-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3ec5c-154">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="3ec5c-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3ec5c-155">токенид</span><span class="sxs-lookup"><span data-stu-id="3ec5c-155">tokenId</span></span>|<span data-ttu-id="3ec5c-156">String</span><span class="sxs-lookup"><span data-stu-id="3ec5c-156">String</span></span>|<span data-ttu-id="3ec5c-157">Идентификатор токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="3ec5c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec5c-158">Response</span></span>
<span data-ttu-id="3ec5c-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec5c-160">Пример</span><span class="sxs-lookup"><span data-stu-id="3ec5c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ec5c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec5c-161">Request</span></span>
<span data-ttu-id="3ec5c-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ec5c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec5c-163">Response</span></span>
<span data-ttu-id="3ec5c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ec5c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



