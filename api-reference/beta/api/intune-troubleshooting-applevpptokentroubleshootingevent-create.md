---
title: Создание Апплевпптокентраублешутинжевент
description: Создание нового объекта Апплевпптокентраублешутинжевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d64e5286ef68f56bfb33da3d470e8ee18260e15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993398"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="ee0a2-103">Создание Апплевпптокентраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="ee0a2-103">Create appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="ee0a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee0a2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee0a2-106">Создание нового объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="ee0a2-106">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee0a2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee0a2-107">Prerequisites</span></span>
<span data-ttu-id="ee0a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0a2-110">Permission type</span></span>|<span data-ttu-id="ee0a2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee0a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee0a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee0a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee0a2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0a2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee0a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee0a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee0a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-115">Not supported.</span></span>|
|<span data-ttu-id="ee0a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee0a2-116">Application</span></span>|<span data-ttu-id="ee0a2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee0a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee0a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ee0a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee0a2-119">Request headers</span></span>
|<span data-ttu-id="ee0a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee0a2-120">Header</span></span>|<span data-ttu-id="ee0a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee0a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee0a2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee0a2-122">Authorization</span></span>|<span data-ttu-id="ee0a2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee0a2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee0a2-124">Accept</span></span>|<span data-ttu-id="ee0a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee0a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0a2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee0a2-126">Request body</span></span>
<span data-ttu-id="ee0a2-127">В тексте запроса добавьте представление объекта Апплевпптокентраублешутинжевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-127">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="ee0a2-128">В следующей таблице приведены свойства, необходимые при создании Апплевпптокентраублешутинжевент.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-128">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="ee0a2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee0a2-129">Property</span></span>|<span data-ttu-id="ee0a2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee0a2-130">Type</span></span>|<span data-ttu-id="ee0a2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee0a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee0a2-132">id</span><span class="sxs-lookup"><span data-stu-id="ee0a2-132">id</span></span>|<span data-ttu-id="ee0a2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ee0a2-133">String</span></span>|<span data-ttu-id="ee0a2-134">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ee0a2-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ee0a2-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ee0a2-135">eventDateTime</span></span>|<span data-ttu-id="ee0a2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee0a2-136">DateTimeOffset</span></span>|<span data-ttu-id="ee0a2-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-137">Time when the event occurred .</span></span> <span data-ttu-id="ee0a2-138">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ee0a2-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ee0a2-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="ee0a2-139">correlationId</span></span>|<span data-ttu-id="ee0a2-140">String</span><span class="sxs-lookup"><span data-stu-id="ee0a2-140">String</span></span>|<span data-ttu-id="ee0a2-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="ee0a2-142">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ee0a2-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ee0a2-143">Траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="ee0a2-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="ee0a2-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ee0a2-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="ee0a2-145">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="ee0a2-146">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ee0a2-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ee0a2-147">eventName</span><span class="sxs-lookup"><span data-stu-id="ee0a2-147">eventName</span></span>|<span data-ttu-id="ee0a2-148">String</span><span class="sxs-lookup"><span data-stu-id="ee0a2-148">String</span></span>|<span data-ttu-id="ee0a2-149">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="ee0a2-150">Это необязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ee0a2-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ee0a2-151">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="ee0a2-151">additionalInformation</span></span>|<span data-ttu-id="ee0a2-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ee0a2-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ee0a2-153">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ee0a2-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ee0a2-154">Токенид</span><span class="sxs-lookup"><span data-stu-id="ee0a2-154">tokenId</span></span>|<span data-ttu-id="ee0a2-155">String</span><span class="sxs-lookup"><span data-stu-id="ee0a2-155">String</span></span>|<span data-ttu-id="ee0a2-156">Идентификатор токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="ee0a2-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0a2-157">Response</span></span>
<span data-ttu-id="ee0a2-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-158">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee0a2-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ee0a2-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee0a2-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee0a2-160">Request</span></span>
<span data-ttu-id="ee0a2-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="ee0a2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0a2-162">Response</span></span>
<span data-ttu-id="ee0a2-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee0a2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





