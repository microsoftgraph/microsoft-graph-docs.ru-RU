---
title: Обновление объекта deviceManagementTroubleshootingEvent
description: Обновление свойств объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 496404d4a12080c9809d47f834e18e7cd5c793df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978349"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="5b4ca-103">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="5b4ca-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="5b4ca-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b4ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b4ca-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b4ca-107">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5b4ca-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b4ca-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b4ca-108">Prerequisites</span></span>
<span data-ttu-id="5b4ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b4ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b4ca-111">Permission type</span></span>|<span data-ttu-id="5b4ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b4ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b4ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b4ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b4ca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4ca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5b4ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b4ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b4ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-116">Not supported.</span></span>|
|<span data-ttu-id="5b4ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b4ca-117">Application</span></span>|<span data-ttu-id="5b4ca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b4ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b4ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="5b4ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b4ca-120">Request headers</span></span>
|<span data-ttu-id="5b4ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b4ca-121">Header</span></span>|<span data-ttu-id="5b4ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b4ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b4ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b4ca-123">Authorization</span></span>|<span data-ttu-id="5b4ca-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5b4ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b4ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b4ca-125">Accept</span></span>|<span data-ttu-id="5b4ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b4ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b4ca-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b4ca-127">Request body</span></span>
<span data-ttu-id="5b4ca-128">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="5b4ca-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5b4ca-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="5b4ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b4ca-130">Property</span></span>|<span data-ttu-id="5b4ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b4ca-131">Type</span></span>|<span data-ttu-id="5b4ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b4ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b4ca-133">id</span><span class="sxs-lookup"><span data-stu-id="5b4ca-133">id</span></span>|<span data-ttu-id="5b4ca-134">String</span><span class="sxs-lookup"><span data-stu-id="5b4ca-134">String</span></span>|<span data-ttu-id="5b4ca-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-135">UUID for the object</span></span>|
|<span data-ttu-id="5b4ca-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="5b4ca-136">eventDateTime</span></span>|<span data-ttu-id="5b4ca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b4ca-137">DateTimeOffset</span></span>|<span data-ttu-id="5b4ca-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="5b4ca-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="5b4ca-139">correlationId</span></span>|<span data-ttu-id="5b4ca-140">String</span><span class="sxs-lookup"><span data-stu-id="5b4ca-140">String</span></span>|<span data-ttu-id="5b4ca-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="5b4ca-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4ca-142">Response</span></span>
<span data-ttu-id="5b4ca-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b4ca-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5b4ca-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b4ca-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b4ca-145">Request</span></span>
<span data-ttu-id="5b4ca-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="5b4ca-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b4ca-147">Response</span></span>
<span data-ttu-id="5b4ca-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5b4ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





