---
title: Обновление mobileAppTroubleshootingEvent
description: Описывает метод Update mobileAppTroubleshootingEvent API Microsoft Graph для Intune, который поддерживает несколько процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d159662ba7823560a321fae03e73b37721b44d4a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863691"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="884b5-103">Обновление mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="884b5-103">Update mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="884b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="884b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="884b5-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="884b5-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="884b5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884b5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="884b5-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="884b5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="884b5-108">Обновление свойств объекта [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="884b5-108">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="884b5-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="884b5-109">Prerequisites</span></span>
<span data-ttu-id="884b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="884b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="884b5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="884b5-112">Permission type</span></span>|<span data-ttu-id="884b5-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="884b5-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="884b5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="884b5-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="884b5-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="884b5-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="884b5-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884b5-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="884b5-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="884b5-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="884b5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884b5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="884b5-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="884b5-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="884b5-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884b5-120">Not supported.</span></span>|
|<span data-ttu-id="884b5-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="884b5-121">Application</span></span>||
|<span data-ttu-id="884b5-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="884b5-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="884b5-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884b5-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="884b5-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="884b5-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="884b5-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884b5-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="884b5-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="884b5-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="884b5-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="884b5-127">Request headers</span></span>
|<span data-ttu-id="884b5-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="884b5-128">Header</span></span>|<span data-ttu-id="884b5-129">Значение</span><span class="sxs-lookup"><span data-stu-id="884b5-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="884b5-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="884b5-130">Authorization</span></span>|<span data-ttu-id="884b5-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="884b5-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="884b5-132">Accept</span><span class="sxs-lookup"><span data-stu-id="884b5-132">Accept</span></span>|<span data-ttu-id="884b5-133">application/json</span><span class="sxs-lookup"><span data-stu-id="884b5-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="884b5-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="884b5-134">Request body</span></span>
<span data-ttu-id="884b5-135">В теле запроса поставляем представление JSON для [объекта mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="884b5-135">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="884b5-136">В следующей таблице показаны свойства, необходимые при создании [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="884b5-136">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="884b5-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="884b5-137">Property</span></span>|<span data-ttu-id="884b5-138">Тип</span><span class="sxs-lookup"><span data-stu-id="884b5-138">Type</span></span>|<span data-ttu-id="884b5-139">Описание</span><span class="sxs-lookup"><span data-stu-id="884b5-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="884b5-140">id</span><span class="sxs-lookup"><span data-stu-id="884b5-140">id</span></span>|<span data-ttu-id="884b5-141">String</span><span class="sxs-lookup"><span data-stu-id="884b5-141">String</span></span>|<span data-ttu-id="884b5-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="884b5-142">The GUID for the object</span></span>|
|<span data-ttu-id="884b5-143">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="884b5-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="884b5-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="884b5-144">additionalInformation</span></span>|<span data-ttu-id="884b5-145">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="884b5-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="884b5-146">Набор пар значений ключа строки и строк, которые предоставляют дополнительные сведения о событии устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="884b5-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="884b5-147">applicationId</span><span class="sxs-lookup"><span data-stu-id="884b5-147">applicationId</span></span>|<span data-ttu-id="884b5-148">String</span><span class="sxs-lookup"><span data-stu-id="884b5-148">String</span></span>|<span data-ttu-id="884b5-149">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="884b5-149">Intune application identifier.</span></span>|
|<span data-ttu-id="884b5-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="884b5-150">correlationId</span></span>|<span data-ttu-id="884b5-151">String</span><span class="sxs-lookup"><span data-stu-id="884b5-151">String</span></span>|<span data-ttu-id="884b5-152">ID, используемый для отслеживания сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="884b5-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="884b5-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="884b5-153">eventDateTime</span></span>|<span data-ttu-id="884b5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="884b5-154">DateTimeOffset</span></span>|<span data-ttu-id="884b5-155">Время, когда произошло событие.</span><span class="sxs-lookup"><span data-stu-id="884b5-155">Time when the event occurred.</span></span> |
|<span data-ttu-id="884b5-156">eventName</span><span class="sxs-lookup"><span data-stu-id="884b5-156">eventName</span></span>|<span data-ttu-id="884b5-157">String</span><span class="sxs-lookup"><span data-stu-id="884b5-157">String</span></span>|<span data-ttu-id="884b5-158">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="884b5-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="884b5-159">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="884b5-159">Optional.</span></span>|
|<span data-ttu-id="884b5-160">история</span><span class="sxs-lookup"><span data-stu-id="884b5-160">history</span></span>|<span data-ttu-id="884b5-161">[коллекция mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="884b5-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="884b5-162">Элемент истории устранения неполадок для мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="884b5-162">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="884b5-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="884b5-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="884b5-164">String</span><span class="sxs-lookup"><span data-stu-id="884b5-164">String</span></span>|<span data-ttu-id="884b5-165">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="884b5-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="884b5-166">устранение неполадокErrorDetails</span><span class="sxs-lookup"><span data-stu-id="884b5-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="884b5-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="884b5-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="884b5-168">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="884b5-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="884b5-169">userId</span><span class="sxs-lookup"><span data-stu-id="884b5-169">userId</span></span>|<span data-ttu-id="884b5-170">String</span><span class="sxs-lookup"><span data-stu-id="884b5-170">String</span></span>|<span data-ttu-id="884b5-171">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="884b5-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="884b5-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="884b5-172">Response</span></span>
<span data-ttu-id="884b5-173">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="884b5-173">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="884b5-174">Пример</span><span class="sxs-lookup"><span data-stu-id="884b5-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="884b5-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="884b5-175">Request</span></span>
<span data-ttu-id="884b5-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="884b5-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="884b5-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="884b5-177">Response</span></span>
<span data-ttu-id="884b5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="884b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```











