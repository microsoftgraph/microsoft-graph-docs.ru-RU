---
title: Создание объекта deviceManagementTroubleshootingEvent
description: Создание объекта deviceManagementTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf2c339f69897b44512dc7317441aacf44f851d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511903"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="f4616-103">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f4616-103">Create deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="f4616-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4616-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4616-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4616-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4616-106">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="f4616-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4616-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4616-107">Prerequisites</span></span>
<span data-ttu-id="f4616-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4616-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4616-110">Permission type</span></span>|<span data-ttu-id="f4616-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4616-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4616-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4616-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4616-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4616-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4616-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4616-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4616-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4616-115">Not supported.</span></span>|
|<span data-ttu-id="f4616-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4616-116">Application</span></span>|<span data-ttu-id="f4616-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4616-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4616-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4616-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f4616-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4616-119">Request headers</span></span>
|<span data-ttu-id="f4616-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4616-120">Header</span></span>|<span data-ttu-id="f4616-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4616-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4616-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4616-122">Authorization</span></span>|<span data-ttu-id="f4616-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4616-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4616-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4616-124">Accept</span></span>|<span data-ttu-id="f4616-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4616-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4616-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4616-126">Request body</span></span>
<span data-ttu-id="f4616-127">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4616-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="f4616-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="f4616-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="f4616-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4616-129">Property</span></span>|<span data-ttu-id="f4616-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f4616-130">Type</span></span>|<span data-ttu-id="f4616-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f4616-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4616-132">id</span><span class="sxs-lookup"><span data-stu-id="f4616-132">id</span></span>|<span data-ttu-id="f4616-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f4616-133">String</span></span>|<span data-ttu-id="f4616-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="f4616-134">UUID for the object</span></span>|
|<span data-ttu-id="f4616-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f4616-135">eventDateTime</span></span>|<span data-ttu-id="f4616-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4616-136">DateTimeOffset</span></span>|<span data-ttu-id="f4616-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="f4616-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="f4616-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="f4616-138">correlationId</span></span>|<span data-ttu-id="f4616-139">String</span><span class="sxs-lookup"><span data-stu-id="f4616-139">String</span></span>|<span data-ttu-id="f4616-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="f4616-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="f4616-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4616-141">Response</span></span>
<span data-ttu-id="f4616-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4616-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4616-143">Пример</span><span class="sxs-lookup"><span data-stu-id="f4616-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4616-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4616-144">Request</span></span>
<span data-ttu-id="f4616-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4616-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4616-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4616-146">Response</span></span>
<span data-ttu-id="f4616-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4616-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




