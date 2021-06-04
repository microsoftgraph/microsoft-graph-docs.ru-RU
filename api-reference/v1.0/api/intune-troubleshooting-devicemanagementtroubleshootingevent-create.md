---
title: Создание объекта deviceManagementTroubleshootingEvent
description: Создание объекта deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdc73c027bdaf8cefabc738620331c8102a63830
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732878"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="af91b-103">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="af91b-103">Create deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="af91b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af91b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af91b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af91b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af91b-106">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="af91b-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af91b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af91b-107">Prerequisites</span></span>
<span data-ttu-id="af91b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af91b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af91b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af91b-110">Permission type</span></span>|<span data-ttu-id="af91b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af91b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af91b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af91b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af91b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af91b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af91b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af91b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af91b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af91b-115">Not supported.</span></span>|
|<span data-ttu-id="af91b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af91b-116">Application</span></span>|<span data-ttu-id="af91b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af91b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af91b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af91b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="af91b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af91b-119">Request headers</span></span>
|<span data-ttu-id="af91b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af91b-120">Header</span></span>|<span data-ttu-id="af91b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="af91b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af91b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af91b-122">Authorization</span></span>|<span data-ttu-id="af91b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af91b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af91b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="af91b-124">Accept</span></span>|<span data-ttu-id="af91b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af91b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af91b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af91b-126">Request body</span></span>
<span data-ttu-id="af91b-127">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af91b-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="af91b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="af91b-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="af91b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="af91b-129">Property</span></span>|<span data-ttu-id="af91b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="af91b-130">Type</span></span>|<span data-ttu-id="af91b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="af91b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af91b-132">id</span><span class="sxs-lookup"><span data-stu-id="af91b-132">id</span></span>|<span data-ttu-id="af91b-133">String</span><span class="sxs-lookup"><span data-stu-id="af91b-133">String</span></span>|<span data-ttu-id="af91b-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="af91b-134">UUID for the object</span></span>|
|<span data-ttu-id="af91b-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="af91b-135">eventDateTime</span></span>|<span data-ttu-id="af91b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af91b-136">DateTimeOffset</span></span>|<span data-ttu-id="af91b-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="af91b-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="af91b-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="af91b-138">correlationId</span></span>|<span data-ttu-id="af91b-139">String</span><span class="sxs-lookup"><span data-stu-id="af91b-139">String</span></span>|<span data-ttu-id="af91b-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="af91b-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="af91b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="af91b-141">Response</span></span>
<span data-ttu-id="af91b-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="af91b-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af91b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="af91b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="af91b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="af91b-144">Request</span></span>
<span data-ttu-id="af91b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af91b-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="af91b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="af91b-146">Response</span></span>
<span data-ttu-id="af91b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af91b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```









