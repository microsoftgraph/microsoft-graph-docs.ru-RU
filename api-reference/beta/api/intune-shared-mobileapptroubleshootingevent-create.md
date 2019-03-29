---
title: Создание Мобилеапптраублешутинжевент
description: Описывает метод Create Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 89a191f94d68636226b6a8d41be0d9ba962da761
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979265"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="ee9f5-103">Создание Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="ee9f5-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="ee9f5-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee9f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee9f5-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee9f5-107">Создание нового объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="ee9f5-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee9f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee9f5-108">Prerequisites</span></span>
<span data-ttu-id="ee9f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee9f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee9f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee9f5-111">Permission type</span></span>|<span data-ttu-id="ee9f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee9f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee9f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee9f5-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ee9f5-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ee9f5-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ee9f5-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee9f5-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee9f5-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="ee9f5-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ee9f5-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee9f5-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee9f5-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee9f5-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee9f5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-119">Not supported.</span></span>|
|<span data-ttu-id="ee9f5-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee9f5-120">Application</span></span>|<span data-ttu-id="ee9f5-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee9f5-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee9f5-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ee9f5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee9f5-123">Request headers</span></span>
|<span data-ttu-id="ee9f5-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee9f5-124">Header</span></span>|<span data-ttu-id="ee9f5-125">Значение</span><span class="sxs-lookup"><span data-stu-id="ee9f5-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee9f5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee9f5-126">Authorization</span></span>|<span data-ttu-id="ee9f5-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee9f5-128">Accept</span><span class="sxs-lookup"><span data-stu-id="ee9f5-128">Accept</span></span>|<span data-ttu-id="ee9f5-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ee9f5-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee9f5-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee9f5-130">Request body</span></span>
<span data-ttu-id="ee9f5-131">В тексте запроса добавьте представление объекта Мобилеапптраублешутинжевент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="ee9f5-132">В следующей таблице приведены свойства, необходимые при создании Мобилеапптраублешутинжевент.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="ee9f5-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee9f5-133">Property</span></span>|<span data-ttu-id="ee9f5-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ee9f5-134">Type</span></span>|<span data-ttu-id="ee9f5-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ee9f5-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee9f5-136">id</span><span class="sxs-lookup"><span data-stu-id="ee9f5-136">id</span></span>|<span data-ttu-id="ee9f5-137">String</span><span class="sxs-lookup"><span data-stu-id="ee9f5-137">String</span></span>|<span data-ttu-id="ee9f5-138">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="ee9f5-138">The GUID for the object</span></span>|
|<span data-ttu-id="ee9f5-139">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="ee9f5-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="ee9f5-140">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="ee9f5-140">additionalInformation</span></span>|<span data-ttu-id="ee9f5-141">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ee9f5-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ee9f5-142">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="ee9f5-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="ee9f5-143">applicationId</span></span>|<span data-ttu-id="ee9f5-144">String</span><span class="sxs-lookup"><span data-stu-id="ee9f5-144">String</span></span>|<span data-ttu-id="ee9f5-145">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-145">Intune application identifier.</span></span>|
|<span data-ttu-id="ee9f5-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="ee9f5-146">correlationId</span></span>|<span data-ttu-id="ee9f5-147">String</span><span class="sxs-lookup"><span data-stu-id="ee9f5-147">String</span></span>|<span data-ttu-id="ee9f5-148">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="ee9f5-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ee9f5-149">eventDateTime</span></span>|<span data-ttu-id="ee9f5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee9f5-150">DateTimeOffset</span></span>|<span data-ttu-id="ee9f5-151">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="ee9f5-152">eventName</span><span class="sxs-lookup"><span data-stu-id="ee9f5-152">eventName</span></span>|<span data-ttu-id="ee9f5-153">String</span><span class="sxs-lookup"><span data-stu-id="ee9f5-153">String</span></span>|<span data-ttu-id="ee9f5-154">Имя события, соответствующее соБытию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="ee9f5-155">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-155">Optional.</span></span>|
|<span data-ttu-id="ee9f5-156">лист</span><span class="sxs-lookup"><span data-stu-id="ee9f5-156">history</span></span>|<span data-ttu-id="ee9f5-157">Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ee9f5-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="ee9f5-158">Элемент журнала устранения неполадок мобильных приложений Intune</span><span class="sxs-lookup"><span data-stu-id="ee9f5-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="ee9f5-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ee9f5-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="ee9f5-160">String</span><span class="sxs-lookup"><span data-stu-id="ee9f5-160">String</span></span>|<span data-ttu-id="ee9f5-161">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="ee9f5-162">Траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="ee9f5-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="ee9f5-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ee9f5-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="ee9f5-164">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="ee9f5-165">userId</span><span class="sxs-lookup"><span data-stu-id="ee9f5-165">userId</span></span>|<span data-ttu-id="ee9f5-166">String</span><span class="sxs-lookup"><span data-stu-id="ee9f5-166">String</span></span>|<span data-ttu-id="ee9f5-167">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="ee9f5-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee9f5-168">Response</span></span>
<span data-ttu-id="ee9f5-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee9f5-170">Пример</span><span class="sxs-lookup"><span data-stu-id="ee9f5-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee9f5-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee9f5-171">Request</span></span>
<span data-ttu-id="ee9f5-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="ee9f5-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee9f5-173">Response</span></span>
<span data-ttu-id="ee9f5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee9f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




