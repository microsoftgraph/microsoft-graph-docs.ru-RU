---
title: Обновление Мобилеапптраублешутинжевент
description: Описывает метод обновления Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58e41160bac079b131b1afe462ddb1309e9137b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979647"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="b5fa6-103">Обновление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="b5fa6-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="b5fa6-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5fa6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5fa6-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5fa6-107">Обновление свойств объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="b5fa6-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5fa6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5fa6-108">Prerequisites</span></span>
<span data-ttu-id="b5fa6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5fa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5fa6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5fa6-111">Permission type</span></span>|<span data-ttu-id="b5fa6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5fa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5fa6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5fa6-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="b5fa6-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="b5fa6-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="b5fa6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5fa6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5fa6-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b5fa6-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="b5fa6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5fa6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5fa6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5fa6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5fa6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-119">Not supported.</span></span>|
|<span data-ttu-id="b5fa6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5fa6-120">Application</span></span>|<span data-ttu-id="b5fa6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5fa6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5fa6-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="b5fa6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5fa6-123">Request headers</span></span>
|<span data-ttu-id="b5fa6-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5fa6-124">Header</span></span>|<span data-ttu-id="b5fa6-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b5fa6-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5fa6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5fa6-126">Authorization</span></span>|<span data-ttu-id="b5fa6-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5fa6-128">Accept</span><span class="sxs-lookup"><span data-stu-id="b5fa6-128">Accept</span></span>|<span data-ttu-id="b5fa6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b5fa6-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5fa6-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5fa6-130">Request body</span></span>
<span data-ttu-id="b5fa6-131">В тексте запроса добавьте представление объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="b5fa6-132">В следующей таблице приведены свойства, необходимые при создании [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b5fa6-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="b5fa6-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5fa6-133">Property</span></span>|<span data-ttu-id="b5fa6-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b5fa6-134">Type</span></span>|<span data-ttu-id="b5fa6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b5fa6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5fa6-136">id</span><span class="sxs-lookup"><span data-stu-id="b5fa6-136">id</span></span>|<span data-ttu-id="b5fa6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b5fa6-137">String</span></span>|<span data-ttu-id="b5fa6-138">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b5fa6-138">The GUID for the object</span></span>|
|<span data-ttu-id="b5fa6-139">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b5fa6-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="b5fa6-140">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="b5fa6-140">additionalInformation</span></span>|<span data-ttu-id="b5fa6-141">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5fa6-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b5fa6-142">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="b5fa6-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="b5fa6-143">applicationId</span></span>|<span data-ttu-id="b5fa6-144">String</span><span class="sxs-lookup"><span data-stu-id="b5fa6-144">String</span></span>|<span data-ttu-id="b5fa6-145">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-145">Intune application identifier.</span></span>|
|<span data-ttu-id="b5fa6-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="b5fa6-146">correlationId</span></span>|<span data-ttu-id="b5fa6-147">String</span><span class="sxs-lookup"><span data-stu-id="b5fa6-147">String</span></span>|<span data-ttu-id="b5fa6-148">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="b5fa6-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b5fa6-149">eventDateTime</span></span>|<span data-ttu-id="b5fa6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5fa6-150">DateTimeOffset</span></span>|<span data-ttu-id="b5fa6-151">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="b5fa6-152">eventName</span><span class="sxs-lookup"><span data-stu-id="b5fa6-152">eventName</span></span>|<span data-ttu-id="b5fa6-153">String</span><span class="sxs-lookup"><span data-stu-id="b5fa6-153">String</span></span>|<span data-ttu-id="b5fa6-154">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="b5fa6-155">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-155">Optional.</span></span>|
|<span data-ttu-id="b5fa6-156">лист</span><span class="sxs-lookup"><span data-stu-id="b5fa6-156">history</span></span>|<span data-ttu-id="b5fa6-157">Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5fa6-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="b5fa6-158">Элемент журнала устранения неполадок мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="b5fa6-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5fa6-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="b5fa6-160">String</span><span class="sxs-lookup"><span data-stu-id="b5fa6-160">String</span></span>|<span data-ttu-id="b5fa6-161">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b5fa6-162">Траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="b5fa6-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="b5fa6-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b5fa6-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="b5fa6-164">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="b5fa6-165">userId</span><span class="sxs-lookup"><span data-stu-id="b5fa6-165">userId</span></span>|<span data-ttu-id="b5fa6-166">String</span><span class="sxs-lookup"><span data-stu-id="b5fa6-166">String</span></span>|<span data-ttu-id="b5fa6-167">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="b5fa6-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5fa6-168">Response</span></span>
<span data-ttu-id="b5fa6-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5fa6-170">Пример</span><span class="sxs-lookup"><span data-stu-id="b5fa6-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5fa6-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5fa6-171">Request</span></span>
<span data-ttu-id="b5fa6-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="b5fa6-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5fa6-173">Response</span></span>
<span data-ttu-id="b5fa6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




