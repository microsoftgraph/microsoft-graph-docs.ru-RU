---
title: Создание Импортеддевицеидентити
description: Создание нового объекта Импортеддевицеидентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76ed9d27936878501526d8dcbed24ac1abdca4a9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184967"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="a07d9-103">Создание Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="a07d9-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="a07d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a07d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a07d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a07d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a07d9-106">Создание нового объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a07d9-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a07d9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a07d9-107">Prerequisites</span></span>
<span data-ttu-id="a07d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a07d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a07d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a07d9-110">Permission type</span></span>|<span data-ttu-id="a07d9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a07d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a07d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a07d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a07d9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07d9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a07d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a07d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a07d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a07d9-115">Not supported.</span></span>|
|<span data-ttu-id="a07d9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a07d9-116">Application</span></span>|<span data-ttu-id="a07d9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07d9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a07d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a07d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a07d9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a07d9-119">Request headers</span></span>
|<span data-ttu-id="a07d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a07d9-120">Header</span></span>|<span data-ttu-id="a07d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a07d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a07d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a07d9-122">Authorization</span></span>|<span data-ttu-id="a07d9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a07d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a07d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a07d9-124">Accept</span></span>|<span data-ttu-id="a07d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a07d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a07d9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a07d9-126">Request body</span></span>
<span data-ttu-id="a07d9-127">В тексте запроса добавьте представление объекта Импортеддевицеидентити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a07d9-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="a07d9-128">В следующей таблице приведены свойства, необходимые при создании Импортеддевицеидентити.</span><span class="sxs-lookup"><span data-stu-id="a07d9-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="a07d9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a07d9-129">Property</span></span>|<span data-ttu-id="a07d9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a07d9-130">Type</span></span>|<span data-ttu-id="a07d9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a07d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a07d9-132">id</span><span class="sxs-lookup"><span data-stu-id="a07d9-132">id</span></span>|<span data-ttu-id="a07d9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a07d9-133">String</span></span>|<span data-ttu-id="a07d9-134">Идентификатор импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="a07d9-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="a07d9-135">импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="a07d9-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="a07d9-136">String.</span><span class="sxs-lookup"><span data-stu-id="a07d9-136">String</span></span>|<span data-ttu-id="a07d9-137">Импортированный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="a07d9-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="a07d9-138">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="a07d9-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="a07d9-139">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="a07d9-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="a07d9-140">Тип импортированного удостоверения устройства.</span><span class="sxs-lookup"><span data-stu-id="a07d9-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="a07d9-141">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="a07d9-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="a07d9-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a07d9-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a07d9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a07d9-143">DateTimeOffset</span></span>|<span data-ttu-id="a07d9-144">Дата и время последнего изменения описания</span><span class="sxs-lookup"><span data-stu-id="a07d9-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="a07d9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a07d9-145">createdDateTime</span></span>|<span data-ttu-id="a07d9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a07d9-146">DateTimeOffset</span></span>|<span data-ttu-id="a07d9-147">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="a07d9-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="a07d9-148">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a07d9-148">lastContactedDateTime</span></span>|<span data-ttu-id="a07d9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a07d9-149">DateTimeOffset</span></span>|<span data-ttu-id="a07d9-150">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="a07d9-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="a07d9-151">description</span><span class="sxs-lookup"><span data-stu-id="a07d9-151">description</span></span>|<span data-ttu-id="a07d9-152">String</span><span class="sxs-lookup"><span data-stu-id="a07d9-152">String</span></span>|<span data-ttu-id="a07d9-153">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="a07d9-153">The description of the device</span></span>|
|<span data-ttu-id="a07d9-154">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="a07d9-154">enrollmentState</span></span>|[<span data-ttu-id="a07d9-155">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="a07d9-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="a07d9-156">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="a07d9-156">The state of the device in Intune.</span></span> <span data-ttu-id="a07d9-157">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="a07d9-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a07d9-158">platform</span><span class="sxs-lookup"><span data-stu-id="a07d9-158">platform</span></span>|[<span data-ttu-id="a07d9-159">управляем</span><span class="sxs-lookup"><span data-stu-id="a07d9-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a07d9-160">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="a07d9-160">The platform of the Device.</span></span> <span data-ttu-id="a07d9-161">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="a07d9-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="a07d9-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07d9-162">Response</span></span>
<span data-ttu-id="a07d9-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a07d9-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07d9-164">Пример</span><span class="sxs-lookup"><span data-stu-id="a07d9-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="a07d9-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="a07d9-165">Request</span></span>
<span data-ttu-id="a07d9-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a07d9-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a07d9-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07d9-167">Response</span></span>
<span data-ttu-id="a07d9-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a07d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




