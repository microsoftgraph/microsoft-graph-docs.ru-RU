---
title: Создание объекта deviceManagementTroubleshootingEvent
description: Создание объекта deviceManagementTroubleshootingEvent.
ms.openlocfilehash: b6af29c77037c4da49d1593341718a8e798805c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026581"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="a6203-103">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a6203-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="a6203-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6203-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6203-105">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a6203-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6203-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a6203-106">Prerequisites</span></span>
<span data-ttu-id="a6203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6203-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6203-109">Permission type</span></span>|<span data-ttu-id="a6203-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6203-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6203-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6203-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6203-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6203-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a6203-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6203-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6203-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6203-114">Not supported.</span></span>|
|<span data-ttu-id="a6203-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6203-115">Application</span></span>|<span data-ttu-id="a6203-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6203-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6203-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6203-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="a6203-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6203-118">Request headers</span></span>
|<span data-ttu-id="a6203-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6203-119">Header</span></span>|<span data-ttu-id="a6203-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a6203-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6203-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6203-121">Authorization</span></span>|<span data-ttu-id="a6203-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a6203-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6203-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a6203-123">Accept</span></span>|<span data-ttu-id="a6203-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6203-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6203-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6203-125">Request body</span></span>
<span data-ttu-id="a6203-126">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6203-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="a6203-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="a6203-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="a6203-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6203-128">Property</span></span>|<span data-ttu-id="a6203-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a6203-129">Type</span></span>|<span data-ttu-id="a6203-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a6203-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6203-131">id</span><span class="sxs-lookup"><span data-stu-id="a6203-131">id</span></span>|<span data-ttu-id="a6203-132">String</span><span class="sxs-lookup"><span data-stu-id="a6203-132">String</span></span>|<span data-ttu-id="a6203-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="a6203-133">UUID for the object</span></span>|
|<span data-ttu-id="a6203-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a6203-134">eventDateTime</span></span>|<span data-ttu-id="a6203-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6203-135">DateTimeOffset</span></span>|<span data-ttu-id="a6203-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="a6203-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="a6203-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="a6203-137">correlationId</span></span>|<span data-ttu-id="a6203-138">String</span><span class="sxs-lookup"><span data-stu-id="a6203-138">String</span></span>|<span data-ttu-id="a6203-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="a6203-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="a6203-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6203-140">Response</span></span>
<span data-ttu-id="a6203-141">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a6203-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6203-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a6203-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6203-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6203-143">Request</span></span>
<span data-ttu-id="a6203-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6203-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6203-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6203-145">Response</span></span>
<span data-ttu-id="a6203-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a6203-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



