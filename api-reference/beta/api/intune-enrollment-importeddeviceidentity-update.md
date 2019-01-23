---
title: Обновление importedDeviceIdentity
description: Обновление свойства объекта importedDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: abc82d0f5305c2cefcc76283e8836d8dacf6e626
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420390"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="90ebc-103">Обновление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="90ebc-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="90ebc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90ebc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90ebc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ebc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90ebc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90ebc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ebc-107">Обновление свойства объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="90ebc-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90ebc-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="90ebc-108">Prerequisites</span></span>
<span data-ttu-id="90ebc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="90ebc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90ebc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90ebc-111">Permission type</span></span>|<span data-ttu-id="90ebc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90ebc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ebc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90ebc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90ebc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ebc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90ebc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90ebc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ebc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ebc-116">Not supported.</span></span>|
|<span data-ttu-id="90ebc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90ebc-117">Application</span></span>|<span data-ttu-id="90ebc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ebc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ebc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90ebc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="90ebc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90ebc-120">Request headers</span></span>
|<span data-ttu-id="90ebc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90ebc-121">Header</span></span>|<span data-ttu-id="90ebc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90ebc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ebc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90ebc-123">Authorization</span></span>|<span data-ttu-id="90ebc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="90ebc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ebc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90ebc-125">Accept</span></span>|<span data-ttu-id="90ebc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90ebc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ebc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90ebc-127">Request body</span></span>
<span data-ttu-id="90ebc-128">В тексте запроса укажите представление JSON для объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="90ebc-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="90ebc-129">В следующей таблице показаны свойства, которые необходимы для создания [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="90ebc-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="90ebc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ebc-130">Property</span></span>|<span data-ttu-id="90ebc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="90ebc-131">Type</span></span>|<span data-ttu-id="90ebc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="90ebc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ebc-133">id</span><span class="sxs-lookup"><span data-stu-id="90ebc-133">id</span></span>|<span data-ttu-id="90ebc-134">String</span><span class="sxs-lookup"><span data-stu-id="90ebc-134">String</span></span>|<span data-ttu-id="90ebc-135">Идентификатор идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="90ebc-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="90ebc-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="90ebc-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="90ebc-137">String</span><span class="sxs-lookup"><span data-stu-id="90ebc-137">String</span></span>|<span data-ttu-id="90ebc-138">Идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="90ebc-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="90ebc-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="90ebc-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="90ebc-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="90ebc-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="90ebc-141">Тип удостоверения импортированных устройства.</span><span class="sxs-lookup"><span data-stu-id="90ebc-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="90ebc-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="90ebc-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="90ebc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90ebc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="90ebc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ebc-144">DateTimeOffset</span></span>|<span data-ttu-id="90ebc-145">Последние изменения даты и времени описания</span><span class="sxs-lookup"><span data-stu-id="90ebc-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="90ebc-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90ebc-146">createdDateTime</span></span>|<span data-ttu-id="90ebc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ebc-147">DateTimeOffset</span></span>|<span data-ttu-id="90ebc-148">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="90ebc-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="90ebc-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="90ebc-149">lastContactedDateTime</span></span>|<span data-ttu-id="90ebc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ebc-150">DateTimeOffset</span></span>|<span data-ttu-id="90ebc-151">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="90ebc-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="90ebc-152">description</span><span class="sxs-lookup"><span data-stu-id="90ebc-152">description</span></span>|<span data-ttu-id="90ebc-153">String</span><span class="sxs-lookup"><span data-stu-id="90ebc-153">String</span></span>|<span data-ttu-id="90ebc-154">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="90ebc-154">The description of the device</span></span>|
|<span data-ttu-id="90ebc-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="90ebc-155">enrollmentState</span></span>|[<span data-ttu-id="90ebc-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="90ebc-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="90ebc-157">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="90ebc-157">The state of the device in Intune.</span></span> <span data-ttu-id="90ebc-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="90ebc-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="90ebc-159">platform</span><span class="sxs-lookup"><span data-stu-id="90ebc-159">platform</span></span>|[<span data-ttu-id="90ebc-160">Платформа</span><span class="sxs-lookup"><span data-stu-id="90ebc-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="90ebc-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="90ebc-161">The platform of the Device.</span></span> <span data-ttu-id="90ebc-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="90ebc-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="90ebc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ebc-163">Response</span></span>
<span data-ttu-id="90ebc-164">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="90ebc-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ebc-165">Пример</span><span class="sxs-lookup"><span data-stu-id="90ebc-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="90ebc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="90ebc-166">Request</span></span>
<span data-ttu-id="90ebc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90ebc-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="90ebc-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ebc-168">Response</span></span>
<span data-ttu-id="90ebc-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="90ebc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```




