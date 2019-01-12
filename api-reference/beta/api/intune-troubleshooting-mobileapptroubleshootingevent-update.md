---
title: Обновление mobileAppTroubleshootingEvent
description: Обновление свойства объекта mobileAppTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ec0c30cc2c37e65fa0a6adebf0bd3a171530640d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940073"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="a5704-103">Обновление mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a5704-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="a5704-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5704-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5704-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5704-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5704-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a5704-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5704-107">Обновление свойства объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="a5704-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5704-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a5704-108">Prerequisites</span></span>
<span data-ttu-id="a5704-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5704-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5704-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5704-111">Permission type</span></span>|<span data-ttu-id="a5704-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5704-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5704-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5704-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5704-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5704-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a5704-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5704-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5704-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5704-116">Not supported.</span></span>|
|<span data-ttu-id="a5704-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5704-117">Application</span></span>|<span data-ttu-id="a5704-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5704-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5704-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5704-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a5704-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5704-120">Request headers</span></span>
|<span data-ttu-id="a5704-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5704-121">Header</span></span>|<span data-ttu-id="a5704-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5704-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5704-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5704-123">Authorization</span></span>|<span data-ttu-id="a5704-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a5704-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5704-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5704-125">Accept</span></span>|<span data-ttu-id="a5704-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5704-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5704-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5704-127">Request body</span></span>
<span data-ttu-id="a5704-128">В тексте запроса укажите представление JSON для объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="a5704-128">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="a5704-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a5704-129">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="a5704-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5704-130">Property</span></span>|<span data-ttu-id="a5704-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5704-131">Type</span></span>|<span data-ttu-id="a5704-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5704-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5704-133">id</span><span class="sxs-lookup"><span data-stu-id="a5704-133">id</span></span>|<span data-ttu-id="a5704-134">String</span><span class="sxs-lookup"><span data-stu-id="a5704-134">String</span></span>|<span data-ttu-id="a5704-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a5704-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a5704-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a5704-136">eventDateTime</span></span>|<span data-ttu-id="a5704-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5704-137">DateTimeOffset</span></span>|<span data-ttu-id="a5704-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="a5704-138">Time when the event occurred .</span></span> <span data-ttu-id="a5704-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a5704-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a5704-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="a5704-140">correlationId</span></span>|<span data-ttu-id="a5704-141">String</span><span class="sxs-lookup"><span data-stu-id="a5704-141">String</span></span>|<span data-ttu-id="a5704-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="a5704-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="a5704-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a5704-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a5704-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a5704-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="a5704-145">String</span><span class="sxs-lookup"><span data-stu-id="a5704-145">String</span></span>|<span data-ttu-id="a5704-146">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="a5704-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="a5704-147">userId</span><span class="sxs-lookup"><span data-stu-id="a5704-147">userId</span></span>|<span data-ttu-id="a5704-148">String</span><span class="sxs-lookup"><span data-stu-id="a5704-148">String</span></span>|<span data-ttu-id="a5704-149">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="a5704-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="a5704-150">applicationId</span><span class="sxs-lookup"><span data-stu-id="a5704-150">applicationId</span></span>|<span data-ttu-id="a5704-151">String</span><span class="sxs-lookup"><span data-stu-id="a5704-151">String</span></span>|<span data-ttu-id="a5704-152">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="a5704-152">Intune application identifier.</span></span>|
|<span data-ttu-id="a5704-153">журнал</span><span class="sxs-lookup"><span data-stu-id="a5704-153">history</span></span>|<span data-ttu-id="a5704-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a5704-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="a5704-155">Устранение неполадок в элемент журнала Intune мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="a5704-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="a5704-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5704-156">Response</span></span>
<span data-ttu-id="a5704-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a5704-157">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5704-158">Пример</span><span class="sxs-lookup"><span data-stu-id="a5704-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5704-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5704-159">Request</span></span>
<span data-ttu-id="a5704-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5704-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 421

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a5704-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5704-161">Response</span></span>
<span data-ttu-id="a5704-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a5704-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 538

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```





