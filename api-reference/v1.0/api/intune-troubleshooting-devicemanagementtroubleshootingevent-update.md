---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7afaf97d6329a3926bfa44be80793f07ee9fd890
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361100"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="3b2d5-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3b2d5-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="3b2d5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b2d5-105">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3b2d5-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b2d5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3b2d5-106">Prerequisites</span></span>
<span data-ttu-id="3b2d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b2d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b2d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b2d5-109">Permission type</span></span>|<span data-ttu-id="3b2d5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b2d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b2d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b2d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b2d5-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b2d5-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b2d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b2d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b2d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-114">Not supported.</span></span>|
|<span data-ttu-id="3b2d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b2d5-115">Application</span></span>|<span data-ttu-id="3b2d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b2d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b2d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3b2d5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b2d5-118">Request headers</span></span>
|<span data-ttu-id="3b2d5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b2d5-119">Header</span></span>|<span data-ttu-id="3b2d5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3b2d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b2d5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b2d5-121">Authorization</span></span>|<span data-ttu-id="3b2d5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b2d5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3b2d5-123">Accept</span></span>|<span data-ttu-id="3b2d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b2d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b2d5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b2d5-125">Request body</span></span>
<span data-ttu-id="3b2d5-126">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="3b2d5-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3b2d5-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="3b2d5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b2d5-128">Property</span></span>|<span data-ttu-id="3b2d5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3b2d5-129">Type</span></span>|<span data-ttu-id="3b2d5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b2d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b2d5-131">id</span><span class="sxs-lookup"><span data-stu-id="3b2d5-131">id</span></span>|<span data-ttu-id="3b2d5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3b2d5-132">String</span></span>|<span data-ttu-id="3b2d5-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-133">UUID for the object</span></span>|
|<span data-ttu-id="3b2d5-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3b2d5-134">eventDateTime</span></span>|<span data-ttu-id="3b2d5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b2d5-135">DateTimeOffset</span></span>|<span data-ttu-id="3b2d5-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="3b2d5-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="3b2d5-137">correlationId</span></span>|<span data-ttu-id="3b2d5-138">String</span><span class="sxs-lookup"><span data-stu-id="3b2d5-138">String</span></span>|<span data-ttu-id="3b2d5-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="3b2d5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b2d5-140">Response</span></span>
<span data-ttu-id="3b2d5-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b2d5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3b2d5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b2d5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b2d5-143">Request</span></span>
<span data-ttu-id="3b2d5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b2d5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b2d5-145">Response</span></span>
<span data-ttu-id="3b2d5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b2d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




