---
title: Обновление mobileAppTroubleshootingEvent
description: Описывает метод Update mobileAppTroubleshootingEvent Microsoft Graph API для Intune, которая поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10bf103a3e796cb5a9e84f1c87ff0571c0bbf551
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430747"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="74262-103">Обновление mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="74262-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="74262-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74262-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="74262-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74262-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74262-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74262-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74262-107">Обновление свойства объекта [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="74262-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74262-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="74262-108">Prerequisites</span></span>
<span data-ttu-id="74262-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="74262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="74262-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74262-111">Permission type</span></span>|<span data-ttu-id="74262-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74262-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74262-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74262-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="74262-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="74262-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="74262-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74262-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="74262-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="74262-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="74262-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74262-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="74262-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74262-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74262-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74262-119">Not supported.</span></span>|
|<span data-ttu-id="74262-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74262-120">Application</span></span>|<span data-ttu-id="74262-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74262-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74262-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74262-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="74262-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74262-123">Request headers</span></span>
|<span data-ttu-id="74262-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74262-124">Header</span></span>|<span data-ttu-id="74262-125">Значение</span><span class="sxs-lookup"><span data-stu-id="74262-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74262-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74262-126">Authorization</span></span>|<span data-ttu-id="74262-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="74262-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74262-128">Accept</span><span class="sxs-lookup"><span data-stu-id="74262-128">Accept</span></span>|<span data-ttu-id="74262-129">application/json</span><span class="sxs-lookup"><span data-stu-id="74262-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74262-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74262-130">Request body</span></span>
<span data-ttu-id="74262-131">В тексте запроса укажите представление JSON для объекта [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="74262-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="74262-132">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="74262-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="74262-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="74262-133">Property</span></span>|<span data-ttu-id="74262-134">Тип</span><span class="sxs-lookup"><span data-stu-id="74262-134">Type</span></span>|<span data-ttu-id="74262-135">Описание</span><span class="sxs-lookup"><span data-stu-id="74262-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74262-136">id</span><span class="sxs-lookup"><span data-stu-id="74262-136">id</span></span>|<span data-ttu-id="74262-137">Строка</span><span class="sxs-lookup"><span data-stu-id="74262-137">String</span></span>|<span data-ttu-id="74262-138">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="74262-138">The GUID for the object</span></span>|
|<span data-ttu-id="74262-139">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="74262-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="74262-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="74262-140">additionalInformation</span></span>|<span data-ttu-id="74262-141">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="74262-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="74262-142">Набор ключ строки и пар строковое значение которой содержатся дополнительные сведения на события устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="74262-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="74262-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="74262-143">applicationId</span></span>|<span data-ttu-id="74262-144">String</span><span class="sxs-lookup"><span data-stu-id="74262-144">String</span></span>|<span data-ttu-id="74262-145">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="74262-145">Intune application identifier.</span></span>|
|<span data-ttu-id="74262-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="74262-146">correlationId</span></span>|<span data-ttu-id="74262-147">String</span><span class="sxs-lookup"><span data-stu-id="74262-147">String</span></span>|<span data-ttu-id="74262-148">Идентификатор, используемый для отслеживания сбоев в службе.</span><span class="sxs-lookup"><span data-stu-id="74262-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="74262-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="74262-149">eventDateTime</span></span>|<span data-ttu-id="74262-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74262-150">DateTimeOffset</span></span>|<span data-ttu-id="74262-151">Время, когда произошло событие.</span><span class="sxs-lookup"><span data-stu-id="74262-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="74262-152">элемент eventName</span><span class="sxs-lookup"><span data-stu-id="74262-152">eventName</span></span>|<span data-ttu-id="74262-153">String</span><span class="sxs-lookup"><span data-stu-id="74262-153">String</span></span>|<span data-ttu-id="74262-154">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="74262-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="74262-155">Не обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="74262-155">Optional.</span></span>|
|<span data-ttu-id="74262-156">журнал</span><span class="sxs-lookup"><span data-stu-id="74262-156">history</span></span>|<span data-ttu-id="74262-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="74262-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="74262-158">Устранение неполадок в элемент журнала приложения Intune Mobile.</span><span class="sxs-lookup"><span data-stu-id="74262-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="74262-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="74262-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="74262-160">String</span><span class="sxs-lookup"><span data-stu-id="74262-160">String</span></span>|<span data-ttu-id="74262-161">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="74262-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="74262-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="74262-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="74262-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="74262-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="74262-164">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="74262-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="74262-165">userId</span><span class="sxs-lookup"><span data-stu-id="74262-165">userId</span></span>|<span data-ttu-id="74262-166">String</span><span class="sxs-lookup"><span data-stu-id="74262-166">String</span></span>|<span data-ttu-id="74262-167">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="74262-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="74262-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="74262-168">Response</span></span>
<span data-ttu-id="74262-169">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74262-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74262-170">Пример</span><span class="sxs-lookup"><span data-stu-id="74262-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="74262-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="74262-171">Request</span></span>
<span data-ttu-id="74262-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74262-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="74262-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="74262-173">Response</span></span>
<span data-ttu-id="74262-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74262-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




