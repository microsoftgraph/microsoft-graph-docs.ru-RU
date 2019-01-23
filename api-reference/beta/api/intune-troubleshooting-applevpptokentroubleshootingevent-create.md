---
title: Создание appleVppTokenTroubleshootingEvent
description: Создание нового объекта appleVppTokenTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2db5607059ca16d1b1df00f4f0f21d7233ab6db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431714"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="c83cd-103">Создание appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c83cd-103">Create appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="c83cd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c83cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c83cd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c83cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c83cd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c83cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c83cd-107">Создание нового объекта [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c83cd-107">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c83cd-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c83cd-108">Prerequisites</span></span>
<span data-ttu-id="c83cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c83cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c83cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c83cd-111">Permission type</span></span>|<span data-ttu-id="c83cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c83cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c83cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c83cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c83cd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83cd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c83cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c83cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c83cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c83cd-116">Not supported.</span></span>|
|<span data-ttu-id="c83cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c83cd-117">Application</span></span>|<span data-ttu-id="c83cd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c83cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c83cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c83cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="c83cd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c83cd-120">Request headers</span></span>
|<span data-ttu-id="c83cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c83cd-121">Header</span></span>|<span data-ttu-id="c83cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c83cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c83cd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c83cd-123">Authorization</span></span>|<span data-ttu-id="c83cd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c83cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c83cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c83cd-125">Accept</span></span>|<span data-ttu-id="c83cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c83cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c83cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c83cd-127">Request body</span></span>
<span data-ttu-id="c83cd-128">В тексте запроса укажите представление JSON для объекта appleVppTokenTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="c83cd-128">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="c83cd-129">В следующей таблице показаны свойства, которые необходимы для создания appleVppTokenTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="c83cd-129">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="c83cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c83cd-130">Property</span></span>|<span data-ttu-id="c83cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c83cd-131">Type</span></span>|<span data-ttu-id="c83cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c83cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c83cd-133">id</span><span class="sxs-lookup"><span data-stu-id="c83cd-133">id</span></span>|<span data-ttu-id="c83cd-134">String</span><span class="sxs-lookup"><span data-stu-id="c83cd-134">String</span></span>|<span data-ttu-id="c83cd-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c83cd-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c83cd-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c83cd-136">eventDateTime</span></span>|<span data-ttu-id="c83cd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83cd-137">DateTimeOffset</span></span>|<span data-ttu-id="c83cd-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="c83cd-138">Time when the event occurred .</span></span> <span data-ttu-id="c83cd-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c83cd-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c83cd-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="c83cd-140">correlationId</span></span>|<span data-ttu-id="c83cd-141">String</span><span class="sxs-lookup"><span data-stu-id="c83cd-141">String</span></span>|<span data-ttu-id="c83cd-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="c83cd-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c83cd-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c83cd-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c83cd-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c83cd-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c83cd-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c83cd-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c83cd-146">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="c83cd-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="c83cd-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c83cd-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c83cd-148">элемент eventName</span><span class="sxs-lookup"><span data-stu-id="c83cd-148">eventName</span></span>|<span data-ttu-id="c83cd-149">String</span><span class="sxs-lookup"><span data-stu-id="c83cd-149">String</span></span>|<span data-ttu-id="c83cd-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="c83cd-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c83cd-151">Это необязательное поле унаследованные от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c83cd-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c83cd-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="c83cd-152">additionalInformation</span></span>|<span data-ttu-id="c83cd-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c83cd-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c83cd-154">Набор ключ строки и пар строковое значение которой содержатся дополнительные сведения на устранение неполадок события унаследованные от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c83cd-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c83cd-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="c83cd-155">tokenId</span></span>|<span data-ttu-id="c83cd-156">String</span><span class="sxs-lookup"><span data-stu-id="c83cd-156">String</span></span>|<span data-ttu-id="c83cd-157">Apple покупки программа маркеров идентификатор тома.</span><span class="sxs-lookup"><span data-stu-id="c83cd-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="c83cd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c83cd-158">Response</span></span>
<span data-ttu-id="c83cd-159">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c83cd-159">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c83cd-160">Пример</span><span class="sxs-lookup"><span data-stu-id="c83cd-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c83cd-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c83cd-161">Request</span></span>
<span data-ttu-id="c83cd-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c83cd-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c83cd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c83cd-163">Response</span></span>
<span data-ttu-id="c83cd-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c83cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




