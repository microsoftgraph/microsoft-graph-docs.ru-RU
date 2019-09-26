---
title: Обновление Импортеддевицеидентити
description: Обновление свойств объекта Импортеддевицеидентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60a2230ae85a5937752a5d96347b3b9b3c32229a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187865"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="addbb-103">Обновление Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="addbb-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="addbb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="addbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="addbb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="addbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="addbb-106">Обновление свойств объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="addbb-106">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="addbb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="addbb-107">Prerequisites</span></span>
<span data-ttu-id="addbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="addbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="addbb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="addbb-110">Permission type</span></span>|<span data-ttu-id="addbb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="addbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="addbb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="addbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="addbb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="addbb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="addbb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="addbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="addbb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="addbb-115">Not supported.</span></span>|
|<span data-ttu-id="addbb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="addbb-116">Application</span></span>|<span data-ttu-id="addbb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="addbb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="addbb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="addbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="addbb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="addbb-119">Request headers</span></span>
|<span data-ttu-id="addbb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="addbb-120">Header</span></span>|<span data-ttu-id="addbb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="addbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="addbb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="addbb-122">Authorization</span></span>|<span data-ttu-id="addbb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="addbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="addbb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="addbb-124">Accept</span></span>|<span data-ttu-id="addbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="addbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="addbb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="addbb-126">Request body</span></span>
<span data-ttu-id="addbb-127">В тексте запроса добавьте представление объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="addbb-127">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="addbb-128">В следующей таблице приведены свойства, необходимые при создании [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="addbb-128">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="addbb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="addbb-129">Property</span></span>|<span data-ttu-id="addbb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="addbb-130">Type</span></span>|<span data-ttu-id="addbb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="addbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="addbb-132">id</span><span class="sxs-lookup"><span data-stu-id="addbb-132">id</span></span>|<span data-ttu-id="addbb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="addbb-133">String</span></span>|<span data-ttu-id="addbb-134">Идентификатор импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="addbb-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="addbb-135">импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="addbb-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="addbb-136">String.</span><span class="sxs-lookup"><span data-stu-id="addbb-136">String</span></span>|<span data-ttu-id="addbb-137">Импортированный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="addbb-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="addbb-138">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="addbb-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="addbb-139">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="addbb-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="addbb-140">Тип импортированного удостоверения устройства.</span><span class="sxs-lookup"><span data-stu-id="addbb-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="addbb-141">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="addbb-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="addbb-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="addbb-142">lastModifiedDateTime</span></span>|<span data-ttu-id="addbb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="addbb-143">DateTimeOffset</span></span>|<span data-ttu-id="addbb-144">Дата и время последнего изменения описания</span><span class="sxs-lookup"><span data-stu-id="addbb-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="addbb-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="addbb-145">createdDateTime</span></span>|<span data-ttu-id="addbb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="addbb-146">DateTimeOffset</span></span>|<span data-ttu-id="addbb-147">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="addbb-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="addbb-148">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="addbb-148">lastContactedDateTime</span></span>|<span data-ttu-id="addbb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="addbb-149">DateTimeOffset</span></span>|<span data-ttu-id="addbb-150">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="addbb-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="addbb-151">description</span><span class="sxs-lookup"><span data-stu-id="addbb-151">description</span></span>|<span data-ttu-id="addbb-152">String</span><span class="sxs-lookup"><span data-stu-id="addbb-152">String</span></span>|<span data-ttu-id="addbb-153">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="addbb-153">The description of the device</span></span>|
|<span data-ttu-id="addbb-154">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="addbb-154">enrollmentState</span></span>|[<span data-ttu-id="addbb-155">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="addbb-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="addbb-156">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="addbb-156">The state of the device in Intune.</span></span> <span data-ttu-id="addbb-157">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="addbb-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="addbb-158">platform</span><span class="sxs-lookup"><span data-stu-id="addbb-158">platform</span></span>|[<span data-ttu-id="addbb-159">управляем</span><span class="sxs-lookup"><span data-stu-id="addbb-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="addbb-160">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="addbb-160">The platform of the Device.</span></span> <span data-ttu-id="addbb-161">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="addbb-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="addbb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="addbb-162">Response</span></span>
<span data-ttu-id="addbb-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="addbb-163">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="addbb-164">Пример</span><span class="sxs-lookup"><span data-stu-id="addbb-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="addbb-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="addbb-165">Request</span></span>
<span data-ttu-id="addbb-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="addbb-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="addbb-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="addbb-167">Response</span></span>
<span data-ttu-id="addbb-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="addbb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




