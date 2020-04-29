---
title: Создание объекта deviceManagementTroubleshootingEvent
description: Создание объекта deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c135b669428b763568306aea7187b718f88ac32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450455"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="44d80-103">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="44d80-103">Create deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="44d80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44d80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44d80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44d80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44d80-106">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="44d80-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44d80-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44d80-107">Prerequisites</span></span>
<span data-ttu-id="44d80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44d80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44d80-110">Permission type</span></span>|<span data-ttu-id="44d80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44d80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44d80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44d80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44d80-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d80-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44d80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44d80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44d80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d80-115">Not supported.</span></span>|
|<span data-ttu-id="44d80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44d80-116">Application</span></span>|<span data-ttu-id="44d80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44d80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44d80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="44d80-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44d80-119">Request headers</span></span>
|<span data-ttu-id="44d80-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44d80-120">Header</span></span>|<span data-ttu-id="44d80-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44d80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44d80-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44d80-122">Authorization</span></span>|<span data-ttu-id="44d80-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44d80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44d80-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44d80-124">Accept</span></span>|<span data-ttu-id="44d80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44d80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44d80-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44d80-126">Request body</span></span>
<span data-ttu-id="44d80-127">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44d80-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="44d80-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="44d80-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="44d80-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44d80-129">Property</span></span>|<span data-ttu-id="44d80-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44d80-130">Type</span></span>|<span data-ttu-id="44d80-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44d80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d80-132">id</span><span class="sxs-lookup"><span data-stu-id="44d80-132">id</span></span>|<span data-ttu-id="44d80-133">Строка</span><span class="sxs-lookup"><span data-stu-id="44d80-133">String</span></span>|<span data-ttu-id="44d80-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="44d80-134">UUID for the object</span></span>|
|<span data-ttu-id="44d80-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="44d80-135">eventDateTime</span></span>|<span data-ttu-id="44d80-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44d80-136">DateTimeOffset</span></span>|<span data-ttu-id="44d80-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="44d80-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="44d80-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="44d80-138">correlationId</span></span>|<span data-ttu-id="44d80-139">String</span><span class="sxs-lookup"><span data-stu-id="44d80-139">String</span></span>|<span data-ttu-id="44d80-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="44d80-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="44d80-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d80-141">Response</span></span>
<span data-ttu-id="44d80-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="44d80-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44d80-143">Пример</span><span class="sxs-lookup"><span data-stu-id="44d80-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="44d80-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d80-144">Request</span></span>
<span data-ttu-id="44d80-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d80-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44d80-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d80-146">Response</span></span>
<span data-ttu-id="44d80-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44d80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






