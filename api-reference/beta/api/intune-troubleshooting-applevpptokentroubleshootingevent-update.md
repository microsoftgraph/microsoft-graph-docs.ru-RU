---
title: Обновление appleVppTokenTroubleshootingEvent
description: Обновление свойства объекта appleVppTokenTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3382eb7069be27fb47bf094d4a0688d7cd128de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430684"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="d66ab-103">Обновление appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="d66ab-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="d66ab-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d66ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d66ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d66ab-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d66ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d66ab-107">Обновление свойства объекта [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="d66ab-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d66ab-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d66ab-108">Prerequisites</span></span>
<span data-ttu-id="d66ab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d66ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d66ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d66ab-111">Permission type</span></span>|<span data-ttu-id="d66ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d66ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d66ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d66ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d66ab-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d66ab-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d66ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d66ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d66ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66ab-116">Not supported.</span></span>|
|<span data-ttu-id="d66ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d66ab-117">Application</span></span>|<span data-ttu-id="d66ab-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d66ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d66ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="d66ab-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d66ab-120">Request headers</span></span>
|<span data-ttu-id="d66ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d66ab-121">Header</span></span>|<span data-ttu-id="d66ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d66ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d66ab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d66ab-123">Authorization</span></span>|<span data-ttu-id="d66ab-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d66ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d66ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d66ab-125">Accept</span></span>|<span data-ttu-id="d66ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d66ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d66ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d66ab-127">Request body</span></span>
<span data-ttu-id="d66ab-128">В тексте запроса укажите представление JSON для объекта [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="d66ab-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="d66ab-129">В следующей таблице показаны свойства, которые необходимы для создания [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d66ab-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="d66ab-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d66ab-130">Property</span></span>|<span data-ttu-id="d66ab-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d66ab-131">Type</span></span>|<span data-ttu-id="d66ab-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d66ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d66ab-133">id</span><span class="sxs-lookup"><span data-stu-id="d66ab-133">id</span></span>|<span data-ttu-id="d66ab-134">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-134">String</span></span>|<span data-ttu-id="d66ab-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d66ab-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66ab-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="d66ab-136">eventDateTime</span></span>|<span data-ttu-id="d66ab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d66ab-137">DateTimeOffset</span></span>|<span data-ttu-id="d66ab-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="d66ab-138">Time when the event occurred .</span></span> <span data-ttu-id="d66ab-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d66ab-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66ab-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="d66ab-140">correlationId</span></span>|<span data-ttu-id="d66ab-141">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-141">String</span></span>|<span data-ttu-id="d66ab-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="d66ab-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="d66ab-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d66ab-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66ab-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d66ab-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="d66ab-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d66ab-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="d66ab-146">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="d66ab-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="d66ab-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d66ab-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66ab-148">элемент eventName</span><span class="sxs-lookup"><span data-stu-id="d66ab-148">eventName</span></span>|<span data-ttu-id="d66ab-149">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-149">String</span></span>|<span data-ttu-id="d66ab-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="d66ab-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="d66ab-151">Это необязательное поле унаследованные от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66ab-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66ab-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="d66ab-152">additionalInformation</span></span>|<span data-ttu-id="d66ab-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d66ab-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d66ab-154">Набор ключ строки и пар строковое значение которой содержатся дополнительные сведения на устранение неполадок события унаследованные от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="d66ab-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="d66ab-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="d66ab-155">tokenId</span></span>|<span data-ttu-id="d66ab-156">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-156">String</span></span>|<span data-ttu-id="d66ab-157">Apple покупки программа маркеров идентификатор тома.</span><span class="sxs-lookup"><span data-stu-id="d66ab-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="d66ab-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d66ab-158">Response</span></span>
<span data-ttu-id="d66ab-159">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d66ab-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d66ab-160">Пример</span><span class="sxs-lookup"><span data-stu-id="d66ab-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="d66ab-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d66ab-161">Request</span></span>
<span data-ttu-id="d66ab-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d66ab-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d66ab-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="d66ab-163">Response</span></span>
<span data-ttu-id="d66ab-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d66ab-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




