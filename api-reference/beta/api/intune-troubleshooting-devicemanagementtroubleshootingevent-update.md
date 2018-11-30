---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
ms.openlocfilehash: aba683521c34168c31991cda46ff3e965f73e320
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081045"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="c9b76-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c9b76-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="c9b76-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9b76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9b76-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9b76-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c9b76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9b76-107">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c9b76-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9b76-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9b76-108">Prerequisites</span></span>
<span data-ttu-id="c9b76-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9b76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b76-111">Permission type</span></span>|<span data-ttu-id="c9b76-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9b76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9b76-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9b76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9b76-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b76-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c9b76-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9b76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9b76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b76-116">Not supported.</span></span>|
|<span data-ttu-id="c9b76-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9b76-117">Application</span></span>|<span data-ttu-id="c9b76-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b76-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9b76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9b76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c9b76-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9b76-120">Request headers</span></span>
|<span data-ttu-id="c9b76-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9b76-121">Header</span></span>|<span data-ttu-id="c9b76-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9b76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9b76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9b76-123">Authorization</span></span>|<span data-ttu-id="c9b76-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c9b76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9b76-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9b76-125">Accept</span></span>|<span data-ttu-id="c9b76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9b76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b76-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9b76-127">Request body</span></span>
<span data-ttu-id="c9b76-128">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9b76-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="c9b76-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c9b76-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="c9b76-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9b76-130">Property</span></span>|<span data-ttu-id="c9b76-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9b76-131">Type</span></span>|<span data-ttu-id="c9b76-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9b76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b76-133">id</span><span class="sxs-lookup"><span data-stu-id="c9b76-133">id</span></span>|<span data-ttu-id="c9b76-134">String</span><span class="sxs-lookup"><span data-stu-id="c9b76-134">String</span></span>|<span data-ttu-id="c9b76-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c9b76-135">UUID for the object</span></span>|
|<span data-ttu-id="c9b76-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c9b76-136">eventDateTime</span></span>|<span data-ttu-id="c9b76-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9b76-137">DateTimeOffset</span></span>|<span data-ttu-id="c9b76-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="c9b76-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="c9b76-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="c9b76-139">correlationId</span></span>|<span data-ttu-id="c9b76-140">String</span><span class="sxs-lookup"><span data-stu-id="c9b76-140">String</span></span>|<span data-ttu-id="c9b76-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="c9b76-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="c9b76-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b76-142">Response</span></span>
<span data-ttu-id="c9b76-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9b76-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9b76-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c9b76-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9b76-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9b76-145">Request</span></span>
<span data-ttu-id="c9b76-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9b76-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="c9b76-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9b76-147">Response</span></span>
<span data-ttu-id="c9b76-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c9b76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





