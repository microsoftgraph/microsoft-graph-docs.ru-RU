---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6681ef7f4cd0082d411a2f5559a5733c9fe55be2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988989"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="6c9da-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6c9da-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="6c9da-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c9da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c9da-105">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="6c9da-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c9da-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6c9da-106">Prerequisites</span></span>
<span data-ttu-id="6c9da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c9da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c9da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c9da-109">Permission type</span></span>|<span data-ttu-id="6c9da-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c9da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c9da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c9da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c9da-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9da-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6c9da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c9da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c9da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c9da-114">Not supported.</span></span>|
|<span data-ttu-id="6c9da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c9da-115">Application</span></span>|<span data-ttu-id="6c9da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c9da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c9da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c9da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="6c9da-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c9da-118">Request headers</span></span>
|<span data-ttu-id="6c9da-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c9da-119">Header</span></span>|<span data-ttu-id="6c9da-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6c9da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c9da-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c9da-121">Authorization</span></span>|<span data-ttu-id="6c9da-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c9da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c9da-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6c9da-123">Accept</span></span>|<span data-ttu-id="6c9da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c9da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c9da-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c9da-125">Request body</span></span>
<span data-ttu-id="6c9da-126">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c9da-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="6c9da-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="6c9da-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="6c9da-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c9da-128">Property</span></span>|<span data-ttu-id="6c9da-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6c9da-129">Type</span></span>|<span data-ttu-id="6c9da-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6c9da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c9da-131">id</span><span class="sxs-lookup"><span data-stu-id="6c9da-131">id</span></span>|<span data-ttu-id="6c9da-132">String</span><span class="sxs-lookup"><span data-stu-id="6c9da-132">String</span></span>|<span data-ttu-id="6c9da-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="6c9da-133">UUID for the object</span></span>|
|<span data-ttu-id="6c9da-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9da-134">eventDateTime</span></span>|<span data-ttu-id="6c9da-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9da-135">DateTimeOffset</span></span>|<span data-ttu-id="6c9da-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="6c9da-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="6c9da-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="6c9da-137">correlationId</span></span>|<span data-ttu-id="6c9da-138">String</span><span class="sxs-lookup"><span data-stu-id="6c9da-138">String</span></span>|<span data-ttu-id="6c9da-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="6c9da-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="6c9da-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9da-140">Response</span></span>
<span data-ttu-id="6c9da-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c9da-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c9da-142">Пример</span><span class="sxs-lookup"><span data-stu-id="6c9da-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c9da-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c9da-143">Request</span></span>
<span data-ttu-id="6c9da-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c9da-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c9da-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9da-145">Response</span></span>
<span data-ttu-id="6c9da-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c9da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



