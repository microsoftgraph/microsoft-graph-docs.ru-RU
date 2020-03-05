---
title: Создание Мобилеапптраублешутинжевент
description: Описывает метод Create Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d1c863fb470746afff287c0d3c6b3af9b89ad0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458261"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="08d15-103">Создание Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="08d15-103">Create mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="08d15-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08d15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08d15-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08d15-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08d15-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08d15-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08d15-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08d15-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08d15-108">Создание нового объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="08d15-108">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08d15-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08d15-109">Prerequisites</span></span>
<span data-ttu-id="08d15-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08d15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08d15-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08d15-112">Permission type</span></span>|<span data-ttu-id="08d15-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08d15-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08d15-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08d15-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="08d15-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="08d15-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="08d15-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d15-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08d15-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="08d15-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="08d15-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d15-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08d15-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08d15-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08d15-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08d15-120">Not supported.</span></span>|
|<span data-ttu-id="08d15-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08d15-121">Application</span></span>||
|<span data-ttu-id="08d15-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="08d15-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="08d15-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d15-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08d15-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="08d15-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="08d15-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d15-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08d15-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08d15-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="08d15-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08d15-127">Request headers</span></span>
|<span data-ttu-id="08d15-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08d15-128">Header</span></span>|<span data-ttu-id="08d15-129">Значение</span><span class="sxs-lookup"><span data-stu-id="08d15-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08d15-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="08d15-130">Authorization</span></span>|<span data-ttu-id="08d15-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08d15-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08d15-132">Accept</span><span class="sxs-lookup"><span data-stu-id="08d15-132">Accept</span></span>|<span data-ttu-id="08d15-133">application/json</span><span class="sxs-lookup"><span data-stu-id="08d15-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08d15-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08d15-134">Request body</span></span>
<span data-ttu-id="08d15-135">В тексте запроса добавьте представление объекта Мобилеапптраублешутинжевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08d15-135">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="08d15-136">В следующей таблице приведены свойства, необходимые при создании Мобилеапптраублешутинжевент.</span><span class="sxs-lookup"><span data-stu-id="08d15-136">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="08d15-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="08d15-137">Property</span></span>|<span data-ttu-id="08d15-138">Тип</span><span class="sxs-lookup"><span data-stu-id="08d15-138">Type</span></span>|<span data-ttu-id="08d15-139">Описание</span><span class="sxs-lookup"><span data-stu-id="08d15-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08d15-140">id</span><span class="sxs-lookup"><span data-stu-id="08d15-140">id</span></span>|<span data-ttu-id="08d15-141">Строка</span><span class="sxs-lookup"><span data-stu-id="08d15-141">String</span></span>|<span data-ttu-id="08d15-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="08d15-142">The GUID for the object</span></span>|
|<span data-ttu-id="08d15-143">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="08d15-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="08d15-144">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="08d15-144">additionalInformation</span></span>|<span data-ttu-id="08d15-145">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="08d15-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="08d15-146">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="08d15-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="08d15-147">applicationId</span><span class="sxs-lookup"><span data-stu-id="08d15-147">applicationId</span></span>|<span data-ttu-id="08d15-148">String</span><span class="sxs-lookup"><span data-stu-id="08d15-148">String</span></span>|<span data-ttu-id="08d15-149">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="08d15-149">Intune application identifier.</span></span>|
|<span data-ttu-id="08d15-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="08d15-150">correlationId</span></span>|<span data-ttu-id="08d15-151">String</span><span class="sxs-lookup"><span data-stu-id="08d15-151">String</span></span>|<span data-ttu-id="08d15-152">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="08d15-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="08d15-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="08d15-153">eventDateTime</span></span>|<span data-ttu-id="08d15-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d15-154">DateTimeOffset</span></span>|<span data-ttu-id="08d15-155">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="08d15-155">Time when the event occurred .</span></span> |
|<span data-ttu-id="08d15-156">eventName</span><span class="sxs-lookup"><span data-stu-id="08d15-156">eventName</span></span>|<span data-ttu-id="08d15-157">String</span><span class="sxs-lookup"><span data-stu-id="08d15-157">String</span></span>|<span data-ttu-id="08d15-158">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="08d15-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="08d15-159">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="08d15-159">Optional.</span></span>|
|<span data-ttu-id="08d15-160">лист</span><span class="sxs-lookup"><span data-stu-id="08d15-160">history</span></span>|<span data-ttu-id="08d15-161">Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="08d15-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="08d15-162">Элемент журнала устранения неполадок мобильных приложений Intune</span><span class="sxs-lookup"><span data-stu-id="08d15-162">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="08d15-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="08d15-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="08d15-164">String</span><span class="sxs-lookup"><span data-stu-id="08d15-164">String</span></span>|<span data-ttu-id="08d15-165">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="08d15-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="08d15-166">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="08d15-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="08d15-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="08d15-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="08d15-168">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="08d15-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="08d15-169">userId</span><span class="sxs-lookup"><span data-stu-id="08d15-169">userId</span></span>|<span data-ttu-id="08d15-170">String</span><span class="sxs-lookup"><span data-stu-id="08d15-170">String</span></span>|<span data-ttu-id="08d15-171">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="08d15-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="08d15-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="08d15-172">Response</span></span>
<span data-ttu-id="08d15-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08d15-173">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08d15-174">Пример</span><span class="sxs-lookup"><span data-stu-id="08d15-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="08d15-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="08d15-175">Request</span></span>
<span data-ttu-id="08d15-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08d15-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="08d15-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="08d15-177">Response</span></span>
<span data-ttu-id="08d15-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08d15-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```












