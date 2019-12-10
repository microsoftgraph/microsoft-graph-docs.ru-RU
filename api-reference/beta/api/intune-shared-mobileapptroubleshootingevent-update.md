---
title: Обновление Мобилеапптраублешутинжевент
description: Описывает метод обновления Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5666fe1799161aeb864e5d4e65044c22cb2f493f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939636"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="03cf2-103">Обновление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="03cf2-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="03cf2-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03cf2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03cf2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03cf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03cf2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03cf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03cf2-107">Обновление свойств объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="03cf2-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03cf2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03cf2-108">Prerequisites</span></span>
<span data-ttu-id="03cf2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03cf2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03cf2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03cf2-111">Permission type</span></span>|<span data-ttu-id="03cf2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03cf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03cf2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03cf2-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="03cf2-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="03cf2-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="03cf2-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03cf2-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03cf2-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="03cf2-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="03cf2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03cf2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03cf2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03cf2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03cf2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03cf2-119">Not supported.</span></span>|
|<span data-ttu-id="03cf2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03cf2-120">Application</span></span>||
|<span data-ttu-id="03cf2-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="03cf2-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="03cf2-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03cf2-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03cf2-123">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="03cf2-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="03cf2-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03cf2-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03cf2-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03cf2-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="03cf2-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03cf2-126">Request headers</span></span>
|<span data-ttu-id="03cf2-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03cf2-127">Header</span></span>|<span data-ttu-id="03cf2-128">Значение</span><span class="sxs-lookup"><span data-stu-id="03cf2-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03cf2-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03cf2-129">Authorization</span></span>|<span data-ttu-id="03cf2-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03cf2-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03cf2-131">Accept</span><span class="sxs-lookup"><span data-stu-id="03cf2-131">Accept</span></span>|<span data-ttu-id="03cf2-132">application/json</span><span class="sxs-lookup"><span data-stu-id="03cf2-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03cf2-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03cf2-133">Request body</span></span>
<span data-ttu-id="03cf2-134">В тексте запроса добавьте представление объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03cf2-134">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="03cf2-135">В следующей таблице приведены свойства, необходимые при создании [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="03cf2-135">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="03cf2-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="03cf2-136">Property</span></span>|<span data-ttu-id="03cf2-137">Тип</span><span class="sxs-lookup"><span data-stu-id="03cf2-137">Type</span></span>|<span data-ttu-id="03cf2-138">Описание</span><span class="sxs-lookup"><span data-stu-id="03cf2-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03cf2-139">id</span><span class="sxs-lookup"><span data-stu-id="03cf2-139">id</span></span>|<span data-ttu-id="03cf2-140">Строка</span><span class="sxs-lookup"><span data-stu-id="03cf2-140">String</span></span>|<span data-ttu-id="03cf2-141">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="03cf2-141">The GUID for the object</span></span>|
|<span data-ttu-id="03cf2-142">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="03cf2-142">**Troubleshooting**</span></span>|
|<span data-ttu-id="03cf2-143">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="03cf2-143">additionalInformation</span></span>|<span data-ttu-id="03cf2-144">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="03cf2-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="03cf2-145">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="03cf2-145">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="03cf2-146">applicationId</span><span class="sxs-lookup"><span data-stu-id="03cf2-146">applicationId</span></span>|<span data-ttu-id="03cf2-147">Строка</span><span class="sxs-lookup"><span data-stu-id="03cf2-147">String</span></span>|<span data-ttu-id="03cf2-148">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="03cf2-148">Intune application identifier.</span></span>|
|<span data-ttu-id="03cf2-149">correlationId</span><span class="sxs-lookup"><span data-stu-id="03cf2-149">correlationId</span></span>|<span data-ttu-id="03cf2-150">Строка</span><span class="sxs-lookup"><span data-stu-id="03cf2-150">String</span></span>|<span data-ttu-id="03cf2-151">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="03cf2-151">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="03cf2-152">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="03cf2-152">eventDateTime</span></span>|<span data-ttu-id="03cf2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03cf2-153">DateTimeOffset</span></span>|<span data-ttu-id="03cf2-154">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="03cf2-154">Time when the event occurred.</span></span> |
|<span data-ttu-id="03cf2-155">eventName</span><span class="sxs-lookup"><span data-stu-id="03cf2-155">eventName</span></span>|<span data-ttu-id="03cf2-156">Строка</span><span class="sxs-lookup"><span data-stu-id="03cf2-156">String</span></span>|<span data-ttu-id="03cf2-157">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="03cf2-157">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="03cf2-158">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="03cf2-158">Optional.</span></span>|
|<span data-ttu-id="03cf2-159">лист</span><span class="sxs-lookup"><span data-stu-id="03cf2-159">history</span></span>|<span data-ttu-id="03cf2-160">Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="03cf2-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="03cf2-161">Элемент журнала устранения неполадок мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="03cf2-161">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="03cf2-162">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="03cf2-162">managedDeviceIdentifier</span></span>|<span data-ttu-id="03cf2-163">String</span><span class="sxs-lookup"><span data-stu-id="03cf2-163">String</span></span>|<span data-ttu-id="03cf2-164">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="03cf2-164">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="03cf2-165">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="03cf2-165">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="03cf2-166">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="03cf2-166">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="03cf2-167">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="03cf2-167">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="03cf2-168">userId</span><span class="sxs-lookup"><span data-stu-id="03cf2-168">userId</span></span>|<span data-ttu-id="03cf2-169">String</span><span class="sxs-lookup"><span data-stu-id="03cf2-169">String</span></span>|<span data-ttu-id="03cf2-170">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="03cf2-170">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="03cf2-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="03cf2-171">Response</span></span>
<span data-ttu-id="03cf2-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03cf2-172">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03cf2-173">Пример</span><span class="sxs-lookup"><span data-stu-id="03cf2-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="03cf2-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="03cf2-174">Request</span></span>
<span data-ttu-id="03cf2-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03cf2-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="03cf2-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="03cf2-176">Response</span></span>
<span data-ttu-id="03cf2-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03cf2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```












