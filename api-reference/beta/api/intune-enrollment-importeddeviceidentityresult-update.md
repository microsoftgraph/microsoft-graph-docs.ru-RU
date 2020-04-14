---
title: Обновление Импортеддевицеидентитиресулт
description: Обновление свойств объекта Импортеддевицеидентитиресулт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10975a400d201ef33698393068c8477fd0df559d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450955"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="fad18-103">Обновление Импортеддевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="fad18-103">Update importedDeviceIdentityResult</span></span>

<span data-ttu-id="fad18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fad18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fad18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fad18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fad18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fad18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fad18-107">Обновление свойств объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="fad18-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fad18-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fad18-108">Prerequisites</span></span>
<span data-ttu-id="fad18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad18-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fad18-111">Permission type</span></span>|<span data-ttu-id="fad18-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fad18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fad18-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fad18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fad18-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad18-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fad18-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fad18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fad18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fad18-116">Not supported.</span></span>|
|<span data-ttu-id="fad18-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fad18-117">Application</span></span>|<span data-ttu-id="fad18-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad18-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fad18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fad18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="fad18-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fad18-120">Request headers</span></span>
|<span data-ttu-id="fad18-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fad18-121">Header</span></span>|<span data-ttu-id="fad18-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fad18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fad18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fad18-123">Authorization</span></span>|<span data-ttu-id="fad18-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fad18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fad18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fad18-125">Accept</span></span>|<span data-ttu-id="fad18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fad18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fad18-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fad18-127">Request body</span></span>
<span data-ttu-id="fad18-128">В тексте запроса добавьте представление объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fad18-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="fad18-129">В следующей таблице приведены свойства, необходимые при создании [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="fad18-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="fad18-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fad18-130">Property</span></span>|<span data-ttu-id="fad18-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fad18-131">Type</span></span>|<span data-ttu-id="fad18-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fad18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fad18-133">id</span><span class="sxs-lookup"><span data-stu-id="fad18-133">id</span></span>|<span data-ttu-id="fad18-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fad18-134">String</span></span>|<span data-ttu-id="fad18-135">Идентификатор импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fad18-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fad18-136">импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="fad18-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="fad18-137">String</span><span class="sxs-lookup"><span data-stu-id="fad18-137">String</span></span>|<span data-ttu-id="fad18-138">Импортированный идентификатор устройства, наследуемый от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fad18-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fad18-139">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="fad18-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="fad18-140">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="fad18-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="fad18-141">Тип импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="fad18-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="fad18-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="fad18-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="fad18-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fad18-143">lastModifiedDateTime</span></span>|<span data-ttu-id="fad18-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad18-144">DateTimeOffset</span></span>|<span data-ttu-id="fad18-145">Дата и время последнего изменения описания, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fad18-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fad18-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fad18-146">createdDateTime</span></span>|<span data-ttu-id="fad18-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad18-147">DateTimeOffset</span></span>|<span data-ttu-id="fad18-148">Дата и время создания устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fad18-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fad18-149">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="fad18-149">lastContactedDateTime</span></span>|<span data-ttu-id="fad18-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad18-150">DateTimeOffset</span></span>|<span data-ttu-id="fad18-151">Дата и время последнего обращения к устройству, унаследованному от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fad18-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fad18-152">description</span><span class="sxs-lookup"><span data-stu-id="fad18-152">description</span></span>|<span data-ttu-id="fad18-153">String</span><span class="sxs-lookup"><span data-stu-id="fad18-153">String</span></span>|<span data-ttu-id="fad18-154">Описание устройства, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fad18-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="fad18-155">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="fad18-155">enrollmentState</span></span>|[<span data-ttu-id="fad18-156">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="fad18-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="fad18-157">Состояние устройства в Intune, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="fad18-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="fad18-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="fad18-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="fad18-159">platform</span><span class="sxs-lookup"><span data-stu-id="fad18-159">platform</span></span>|[<span data-ttu-id="fad18-160">управляем</span><span class="sxs-lookup"><span data-stu-id="fad18-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="fad18-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="fad18-161">The platform of the Device.</span></span> <span data-ttu-id="fad18-162">Наследуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="fad18-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="fad18-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="fad18-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="fad18-164">status</span><span class="sxs-lookup"><span data-stu-id="fad18-164">status</span></span>|<span data-ttu-id="fad18-165">Логическое</span><span class="sxs-lookup"><span data-stu-id="fad18-165">Boolean</span></span>|<span data-ttu-id="fad18-166">Состояние импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="fad18-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="fad18-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="fad18-167">Response</span></span>
<span data-ttu-id="fad18-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fad18-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fad18-169">Пример</span><span class="sxs-lookup"><span data-stu-id="fad18-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="fad18-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="fad18-170">Request</span></span>
<span data-ttu-id="fad18-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fad18-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="fad18-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="fad18-172">Response</span></span>
<span data-ttu-id="fad18-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fad18-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```



