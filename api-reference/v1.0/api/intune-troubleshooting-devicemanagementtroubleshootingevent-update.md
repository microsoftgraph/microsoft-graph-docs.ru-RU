---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3219a86b2d7788217b26d640443807a4818c66a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251715"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="4a43e-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4a43e-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="4a43e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a43e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a43e-105">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4a43e-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a43e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4a43e-106">Prerequisites</span></span>
<span data-ttu-id="4a43e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a43e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a43e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a43e-109">Permission type</span></span>|<span data-ttu-id="4a43e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a43e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a43e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a43e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a43e-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a43e-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4a43e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a43e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a43e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a43e-114">Not supported.</span></span>|
|<span data-ttu-id="4a43e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a43e-115">Application</span></span>|<span data-ttu-id="4a43e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a43e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a43e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a43e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="4a43e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a43e-118">Request headers</span></span>
|<span data-ttu-id="4a43e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a43e-119">Header</span></span>|<span data-ttu-id="4a43e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4a43e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a43e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a43e-121">Authorization</span></span>|<span data-ttu-id="4a43e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4a43e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a43e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4a43e-123">Accept</span></span>|<span data-ttu-id="4a43e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a43e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a43e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a43e-125">Request body</span></span>
<span data-ttu-id="4a43e-126">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a43e-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="4a43e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4a43e-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="4a43e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a43e-128">Property</span></span>|<span data-ttu-id="4a43e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4a43e-129">Type</span></span>|<span data-ttu-id="4a43e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4a43e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a43e-131">id</span><span class="sxs-lookup"><span data-stu-id="4a43e-131">id</span></span>|<span data-ttu-id="4a43e-132">String</span><span class="sxs-lookup"><span data-stu-id="4a43e-132">String</span></span>|<span data-ttu-id="4a43e-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="4a43e-133">UUID for the object</span></span>|
|<span data-ttu-id="4a43e-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4a43e-134">eventDateTime</span></span>|<span data-ttu-id="4a43e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a43e-135">DateTimeOffset</span></span>|<span data-ttu-id="4a43e-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="4a43e-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="4a43e-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="4a43e-137">correlationId</span></span>|<span data-ttu-id="4a43e-138">String</span><span class="sxs-lookup"><span data-stu-id="4a43e-138">String</span></span>|<span data-ttu-id="4a43e-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="4a43e-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="4a43e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a43e-140">Response</span></span>
<span data-ttu-id="4a43e-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4a43e-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a43e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4a43e-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a43e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a43e-143">Request</span></span>
<span data-ttu-id="4a43e-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a43e-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="4a43e-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a43e-145">Response</span></span>
<span data-ttu-id="4a43e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4a43e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



