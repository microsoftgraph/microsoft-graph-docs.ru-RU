---
title: Создание Импортеддевицеидентити
description: Создание нового объекта Импортеддевицеидентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2976dea7a10cdaa35cde4500480fd0200370bbca
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943882"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="f6ab5-103">Создание Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="f6ab5-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="f6ab5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6ab5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6ab5-106">Создание нового объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f6ab5-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6ab5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6ab5-107">Prerequisites</span></span>
<span data-ttu-id="f6ab5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ab5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ab5-110">Permission type</span></span>|<span data-ttu-id="f6ab5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6ab5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6ab5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6ab5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6ab5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ab5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6ab5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6ab5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6ab5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-115">Not supported.</span></span>|
|<span data-ttu-id="f6ab5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6ab5-116">Application</span></span>|<span data-ttu-id="f6ab5-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ab5-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6ab5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6ab5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="f6ab5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6ab5-119">Request headers</span></span>
|<span data-ttu-id="f6ab5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6ab5-120">Header</span></span>|<span data-ttu-id="f6ab5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f6ab5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6ab5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6ab5-122">Authorization</span></span>|<span data-ttu-id="f6ab5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6ab5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f6ab5-124">Accept</span></span>|<span data-ttu-id="f6ab5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6ab5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6ab5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6ab5-126">Request body</span></span>
<span data-ttu-id="f6ab5-127">В тексте запроса добавьте представление объекта Импортеддевицеидентити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="f6ab5-128">В следующей таблице приведены свойства, необходимые при создании Импортеддевицеидентити.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="f6ab5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6ab5-129">Property</span></span>|<span data-ttu-id="f6ab5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f6ab5-130">Type</span></span>|<span data-ttu-id="f6ab5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ab5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6ab5-132">id</span><span class="sxs-lookup"><span data-stu-id="f6ab5-132">id</span></span>|<span data-ttu-id="f6ab5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f6ab5-133">String</span></span>|<span data-ttu-id="f6ab5-134">Идентификатор импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="f6ab5-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="f6ab5-135">импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="f6ab5-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="f6ab5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f6ab5-136">String</span></span>|<span data-ttu-id="f6ab5-137">Импортированный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="f6ab5-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="f6ab5-138">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="f6ab5-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="f6ab5-139">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="f6ab5-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="f6ab5-140">Тип импортированного удостоверения устройства.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="f6ab5-141">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="f6ab5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ab5-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f6ab5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ab5-143">DateTimeOffset</span></span>|<span data-ttu-id="f6ab5-144">Дата и время последнего изменения описания</span><span class="sxs-lookup"><span data-stu-id="f6ab5-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="f6ab5-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ab5-145">createdDateTime</span></span>|<span data-ttu-id="f6ab5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ab5-146">DateTimeOffset</span></span>|<span data-ttu-id="f6ab5-147">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="f6ab5-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="f6ab5-148">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="f6ab5-148">lastContactedDateTime</span></span>|<span data-ttu-id="f6ab5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ab5-149">DateTimeOffset</span></span>|<span data-ttu-id="f6ab5-150">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="f6ab5-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="f6ab5-151">description</span><span class="sxs-lookup"><span data-stu-id="f6ab5-151">description</span></span>|<span data-ttu-id="f6ab5-152">String</span><span class="sxs-lookup"><span data-stu-id="f6ab5-152">String</span></span>|<span data-ttu-id="f6ab5-153">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="f6ab5-153">The description of the device</span></span>|
|<span data-ttu-id="f6ab5-154">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="f6ab5-154">enrollmentState</span></span>|[<span data-ttu-id="f6ab5-155">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="f6ab5-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="f6ab5-156">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-156">The state of the device in Intune.</span></span> <span data-ttu-id="f6ab5-157">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f6ab5-158">platform</span><span class="sxs-lookup"><span data-stu-id="f6ab5-158">platform</span></span>|[<span data-ttu-id="f6ab5-159">управляем</span><span class="sxs-lookup"><span data-stu-id="f6ab5-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f6ab5-160">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-160">The platform of the Device.</span></span> <span data-ttu-id="f6ab5-161">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="f6ab5-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6ab5-162">Response</span></span>
<span data-ttu-id="f6ab5-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6ab5-164">Пример</span><span class="sxs-lookup"><span data-stu-id="f6ab5-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6ab5-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6ab5-165">Request</span></span>
<span data-ttu-id="f6ab5-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="f6ab5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ab5-167">Response</span></span>
<span data-ttu-id="f6ab5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6ab5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





