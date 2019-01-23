---
title: Создание mobileAppTroubleshootingEvent
description: Описание метода Create mobileAppTroubleshootingEvent Microsoft Graph API для Intune, которая поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e409aa663ff2471222a7e36a9e381505792f37eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431726"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="57423-103">Создание mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="57423-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="57423-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57423-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57423-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57423-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57423-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57423-107">Создание нового объекта [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="57423-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57423-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="57423-108">Prerequisites</span></span>
<span data-ttu-id="57423-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="57423-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="57423-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57423-111">Permission type</span></span>|<span data-ttu-id="57423-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57423-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57423-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57423-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="57423-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="57423-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="57423-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57423-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57423-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="57423-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="57423-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57423-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57423-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57423-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57423-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57423-119">Not supported.</span></span>|
|<span data-ttu-id="57423-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57423-120">Application</span></span>|<span data-ttu-id="57423-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57423-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57423-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57423-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="57423-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57423-123">Request headers</span></span>
|<span data-ttu-id="57423-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57423-124">Header</span></span>|<span data-ttu-id="57423-125">Значение</span><span class="sxs-lookup"><span data-stu-id="57423-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57423-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57423-126">Authorization</span></span>|<span data-ttu-id="57423-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="57423-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57423-128">Accept</span><span class="sxs-lookup"><span data-stu-id="57423-128">Accept</span></span>|<span data-ttu-id="57423-129">application/json</span><span class="sxs-lookup"><span data-stu-id="57423-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57423-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57423-130">Request body</span></span>
<span data-ttu-id="57423-131">В тексте запроса укажите представление JSON для объекта mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="57423-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="57423-132">В следующей таблице показаны свойства, которые необходимы для создания mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="57423-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="57423-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="57423-133">Property</span></span>|<span data-ttu-id="57423-134">Тип</span><span class="sxs-lookup"><span data-stu-id="57423-134">Type</span></span>|<span data-ttu-id="57423-135">Описание</span><span class="sxs-lookup"><span data-stu-id="57423-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57423-136">id</span><span class="sxs-lookup"><span data-stu-id="57423-136">id</span></span>|<span data-ttu-id="57423-137">Строка</span><span class="sxs-lookup"><span data-stu-id="57423-137">String</span></span>|<span data-ttu-id="57423-138">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="57423-138">The GUID for the object</span></span>|
|<span data-ttu-id="57423-139">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="57423-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="57423-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="57423-140">additionalInformation</span></span>|<span data-ttu-id="57423-141">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="57423-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="57423-142">Набор ключ строки и пар строковое значение которой содержатся дополнительные сведения на события устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="57423-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="57423-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="57423-143">applicationId</span></span>|<span data-ttu-id="57423-144">String</span><span class="sxs-lookup"><span data-stu-id="57423-144">String</span></span>|<span data-ttu-id="57423-145">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="57423-145">Intune application identifier.</span></span>|
|<span data-ttu-id="57423-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="57423-146">correlationId</span></span>|<span data-ttu-id="57423-147">String</span><span class="sxs-lookup"><span data-stu-id="57423-147">String</span></span>|<span data-ttu-id="57423-148">Идентификатор, используемый для отслеживания сбоев в службе.</span><span class="sxs-lookup"><span data-stu-id="57423-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="57423-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="57423-149">eventDateTime</span></span>|<span data-ttu-id="57423-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57423-150">DateTimeOffset</span></span>|<span data-ttu-id="57423-151">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="57423-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="57423-152">элемент eventName</span><span class="sxs-lookup"><span data-stu-id="57423-152">eventName</span></span>|<span data-ttu-id="57423-153">String</span><span class="sxs-lookup"><span data-stu-id="57423-153">String</span></span>|<span data-ttu-id="57423-154">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="57423-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="57423-155">Не обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="57423-155">Optional.</span></span>|
|<span data-ttu-id="57423-156">журнал</span><span class="sxs-lookup"><span data-stu-id="57423-156">history</span></span>|<span data-ttu-id="57423-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="57423-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="57423-158">Устранение неполадок в элемент журнала Intune мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="57423-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="57423-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="57423-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="57423-160">String</span><span class="sxs-lookup"><span data-stu-id="57423-160">String</span></span>|<span data-ttu-id="57423-161">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="57423-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="57423-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="57423-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="57423-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="57423-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="57423-164">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="57423-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="57423-165">userId</span><span class="sxs-lookup"><span data-stu-id="57423-165">userId</span></span>|<span data-ttu-id="57423-166">String</span><span class="sxs-lookup"><span data-stu-id="57423-166">String</span></span>|<span data-ttu-id="57423-167">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="57423-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="57423-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="57423-168">Response</span></span>
<span data-ttu-id="57423-169">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="57423-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57423-170">Пример</span><span class="sxs-lookup"><span data-stu-id="57423-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="57423-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="57423-171">Request</span></span>
<span data-ttu-id="57423-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57423-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="57423-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="57423-173">Response</span></span>
<span data-ttu-id="57423-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="57423-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




