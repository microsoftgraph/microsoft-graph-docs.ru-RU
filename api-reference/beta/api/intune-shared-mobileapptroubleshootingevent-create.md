---
title: Создание Мобилеапптраублешутинжевент
description: Описывает метод Create Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33336696744e8878ec5324026c88671b4b71fe17
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537967"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="51c4e-103">Создание Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="51c4e-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="51c4e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51c4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51c4e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51c4e-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51c4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51c4e-107">Создание нового объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="51c4e-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51c4e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51c4e-108">Prerequisites</span></span>
<span data-ttu-id="51c4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51c4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51c4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51c4e-111">Permission type</span></span>|<span data-ttu-id="51c4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51c4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51c4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51c4e-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="51c4e-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="51c4e-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="51c4e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c4e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="51c4e-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="51c4e-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="51c4e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c4e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="51c4e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51c4e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51c4e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c4e-119">Not supported.</span></span>|
|<span data-ttu-id="51c4e-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="51c4e-120">Application</span></span>||
|<span data-ttu-id="51c4e-121">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="51c4e-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="51c4e-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c4e-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="51c4e-123">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="51c4e-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="51c4e-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c4e-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51c4e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51c4e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="51c4e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51c4e-126">Request headers</span></span>
|<span data-ttu-id="51c4e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51c4e-127">Header</span></span>|<span data-ttu-id="51c4e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="51c4e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51c4e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51c4e-129">Authorization</span></span>|<span data-ttu-id="51c4e-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51c4e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51c4e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="51c4e-131">Accept</span></span>|<span data-ttu-id="51c4e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="51c4e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51c4e-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51c4e-133">Request body</span></span>
<span data-ttu-id="51c4e-134">В тексте запроса добавьте представление объекта Мобилеапптраублешутинжевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51c4e-134">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="51c4e-135">В следующей таблице приведены свойства, необходимые при создании Мобилеапптраублешутинжевент.</span><span class="sxs-lookup"><span data-stu-id="51c4e-135">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="51c4e-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="51c4e-136">Property</span></span>|<span data-ttu-id="51c4e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="51c4e-137">Type</span></span>|<span data-ttu-id="51c4e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="51c4e-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51c4e-139">id</span><span class="sxs-lookup"><span data-stu-id="51c4e-139">id</span></span>|<span data-ttu-id="51c4e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="51c4e-140">String</span></span>|<span data-ttu-id="51c4e-141">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="51c4e-141">The GUID for the object</span></span>|
|<span data-ttu-id="51c4e-142">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="51c4e-142">**Troubleshooting**</span></span>|
|<span data-ttu-id="51c4e-143">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="51c4e-143">additionalInformation</span></span>|<span data-ttu-id="51c4e-144">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="51c4e-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="51c4e-145">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="51c4e-145">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="51c4e-146">applicationId</span><span class="sxs-lookup"><span data-stu-id="51c4e-146">applicationId</span></span>|<span data-ttu-id="51c4e-147">String</span><span class="sxs-lookup"><span data-stu-id="51c4e-147">String</span></span>|<span data-ttu-id="51c4e-148">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="51c4e-148">Intune application identifier.</span></span>|
|<span data-ttu-id="51c4e-149">correlationId</span><span class="sxs-lookup"><span data-stu-id="51c4e-149">correlationId</span></span>|<span data-ttu-id="51c4e-150">String</span><span class="sxs-lookup"><span data-stu-id="51c4e-150">String</span></span>|<span data-ttu-id="51c4e-151">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="51c4e-151">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="51c4e-152">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="51c4e-152">eventDateTime</span></span>|<span data-ttu-id="51c4e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51c4e-153">DateTimeOffset</span></span>|<span data-ttu-id="51c4e-154">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="51c4e-154">Time when the event occurred .</span></span> |
|<span data-ttu-id="51c4e-155">eventName</span><span class="sxs-lookup"><span data-stu-id="51c4e-155">eventName</span></span>|<span data-ttu-id="51c4e-156">String</span><span class="sxs-lookup"><span data-stu-id="51c4e-156">String</span></span>|<span data-ttu-id="51c4e-157">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="51c4e-157">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="51c4e-158">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="51c4e-158">Optional.</span></span>|
|<span data-ttu-id="51c4e-159">лист</span><span class="sxs-lookup"><span data-stu-id="51c4e-159">history</span></span>|<span data-ttu-id="51c4e-160">Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="51c4e-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="51c4e-161">Элемент журнала устранения неполадок мобильных приложений Intune</span><span class="sxs-lookup"><span data-stu-id="51c4e-161">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="51c4e-162">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="51c4e-162">managedDeviceIdentifier</span></span>|<span data-ttu-id="51c4e-163">String</span><span class="sxs-lookup"><span data-stu-id="51c4e-163">String</span></span>|<span data-ttu-id="51c4e-164">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="51c4e-164">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="51c4e-165">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="51c4e-165">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="51c4e-166">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="51c4e-166">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="51c4e-167">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="51c4e-167">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="51c4e-168">userId</span><span class="sxs-lookup"><span data-stu-id="51c4e-168">userId</span></span>|<span data-ttu-id="51c4e-169">String</span><span class="sxs-lookup"><span data-stu-id="51c4e-169">String</span></span>|<span data-ttu-id="51c4e-170">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="51c4e-170">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="51c4e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="51c4e-171">Response</span></span>
<span data-ttu-id="51c4e-172">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51c4e-172">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51c4e-173">Пример</span><span class="sxs-lookup"><span data-stu-id="51c4e-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="51c4e-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="51c4e-174">Request</span></span>
<span data-ttu-id="51c4e-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51c4e-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="51c4e-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="51c4e-176">Response</span></span>
<span data-ttu-id="51c4e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51c4e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```










