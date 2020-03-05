---
title: Обновление Апплевпптокентраублешутинжевент
description: Обновление свойств объекта Апплевпптокентраублешутинжевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b17abfe8424a0c7ab9cb50dd9a7ac1f87145ed3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457750"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="25490-103">Обновление Апплевпптокентраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="25490-103">Update appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="25490-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="25490-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25490-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25490-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25490-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25490-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25490-107">Обновление свойств объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="25490-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25490-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25490-108">Prerequisites</span></span>
<span data-ttu-id="25490-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25490-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25490-111">Permission type</span></span>|<span data-ttu-id="25490-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25490-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25490-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25490-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25490-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25490-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="25490-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25490-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25490-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25490-116">Not supported.</span></span>|
|<span data-ttu-id="25490-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25490-117">Application</span></span>|<span data-ttu-id="25490-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25490-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25490-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25490-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="25490-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25490-120">Request headers</span></span>
|<span data-ttu-id="25490-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25490-121">Header</span></span>|<span data-ttu-id="25490-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25490-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25490-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25490-123">Authorization</span></span>|<span data-ttu-id="25490-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25490-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25490-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25490-125">Accept</span></span>|<span data-ttu-id="25490-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25490-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25490-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25490-127">Request body</span></span>
<span data-ttu-id="25490-128">В тексте запроса добавьте представление объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25490-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="25490-129">В следующей таблице приведены свойства, необходимые при создании [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="25490-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="25490-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="25490-130">Property</span></span>|<span data-ttu-id="25490-131">Тип</span><span class="sxs-lookup"><span data-stu-id="25490-131">Type</span></span>|<span data-ttu-id="25490-132">Описание</span><span class="sxs-lookup"><span data-stu-id="25490-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25490-133">id</span><span class="sxs-lookup"><span data-stu-id="25490-133">id</span></span>|<span data-ttu-id="25490-134">Строка</span><span class="sxs-lookup"><span data-stu-id="25490-134">String</span></span>|<span data-ttu-id="25490-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="25490-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="25490-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="25490-136">eventDateTime</span></span>|<span data-ttu-id="25490-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25490-137">DateTimeOffset</span></span>|<span data-ttu-id="25490-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="25490-138">Time when the event occurred .</span></span> <span data-ttu-id="25490-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="25490-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="25490-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="25490-140">correlationId</span></span>|<span data-ttu-id="25490-141">String</span><span class="sxs-lookup"><span data-stu-id="25490-141">String</span></span>|<span data-ttu-id="25490-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="25490-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="25490-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="25490-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="25490-144">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="25490-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="25490-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="25490-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="25490-146">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="25490-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="25490-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="25490-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="25490-148">eventName</span><span class="sxs-lookup"><span data-stu-id="25490-148">eventName</span></span>|<span data-ttu-id="25490-149">String</span><span class="sxs-lookup"><span data-stu-id="25490-149">String</span></span>|<span data-ttu-id="25490-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="25490-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="25490-151">Это необязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="25490-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="25490-152">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="25490-152">additionalInformation</span></span>|<span data-ttu-id="25490-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="25490-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="25490-154">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="25490-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="25490-155">токенид</span><span class="sxs-lookup"><span data-stu-id="25490-155">tokenId</span></span>|<span data-ttu-id="25490-156">String</span><span class="sxs-lookup"><span data-stu-id="25490-156">String</span></span>|<span data-ttu-id="25490-157">Идентификатор токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="25490-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="25490-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="25490-158">Response</span></span>
<span data-ttu-id="25490-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25490-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25490-160">Пример</span><span class="sxs-lookup"><span data-stu-id="25490-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="25490-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="25490-161">Request</span></span>
<span data-ttu-id="25490-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25490-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25490-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="25490-163">Response</span></span>
<span data-ttu-id="25490-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25490-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





