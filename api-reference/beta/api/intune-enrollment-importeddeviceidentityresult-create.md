---
title: Создание Импортеддевицеидентитиресулт
description: Создание нового объекта Импортеддевицеидентитиресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00355c647339dbb4f9e5f6e5965b0b3fe6faf577
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535872"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="bbd63-103">Создание Импортеддевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="bbd63-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="bbd63-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbd63-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbd63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbd63-106">Создание нового объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="bbd63-106">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbd63-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bbd63-107">Prerequisites</span></span>
<span data-ttu-id="bbd63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbd63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbd63-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd63-110">Permission type</span></span>|<span data-ttu-id="bbd63-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbd63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbd63-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbd63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bbd63-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbd63-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bbd63-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbd63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbd63-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd63-115">Not supported.</span></span>|
|<span data-ttu-id="bbd63-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bbd63-116">Application</span></span>|<span data-ttu-id="bbd63-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbd63-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbd63-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbd63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="bbd63-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbd63-119">Request headers</span></span>
|<span data-ttu-id="bbd63-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbd63-120">Header</span></span>|<span data-ttu-id="bbd63-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bbd63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbd63-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbd63-122">Authorization</span></span>|<span data-ttu-id="bbd63-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbd63-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bbd63-124">Accept</span></span>|<span data-ttu-id="bbd63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bbd63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbd63-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbd63-126">Request body</span></span>
<span data-ttu-id="bbd63-127">В тексте запроса добавьте представление объекта Импортеддевицеидентитиресулт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd63-127">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="bbd63-128">В следующей таблице приведены свойства, необходимые при создании Импортеддевицеидентитиресулт.</span><span class="sxs-lookup"><span data-stu-id="bbd63-128">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="bbd63-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbd63-129">Property</span></span>|<span data-ttu-id="bbd63-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd63-130">Type</span></span>|<span data-ttu-id="bbd63-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbd63-132">id</span><span class="sxs-lookup"><span data-stu-id="bbd63-132">id</span></span>|<span data-ttu-id="bbd63-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bbd63-133">String</span></span>|<span data-ttu-id="bbd63-134">Идентификатор импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbd63-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bbd63-135">импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="bbd63-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="bbd63-136">String</span><span class="sxs-lookup"><span data-stu-id="bbd63-136">String</span></span>|<span data-ttu-id="bbd63-137">Импортированный идентификатор устройства, наследуемый от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbd63-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bbd63-138">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="bbd63-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="bbd63-139">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="bbd63-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="bbd63-140">Тип импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="bbd63-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="bbd63-141">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="bbd63-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="bbd63-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbd63-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bbd63-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbd63-143">DateTimeOffset</span></span>|<span data-ttu-id="bbd63-144">Дата и время последнего изменения описания, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbd63-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bbd63-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbd63-145">createdDateTime</span></span>|<span data-ttu-id="bbd63-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbd63-146">DateTimeOffset</span></span>|<span data-ttu-id="bbd63-147">Дата и время создания устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbd63-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bbd63-148">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="bbd63-148">lastContactedDateTime</span></span>|<span data-ttu-id="bbd63-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbd63-149">DateTimeOffset</span></span>|<span data-ttu-id="bbd63-150">Дата и время последнего обращения к устройству, унаследованному от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbd63-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bbd63-151">description</span><span class="sxs-lookup"><span data-stu-id="bbd63-151">description</span></span>|<span data-ttu-id="bbd63-152">String</span><span class="sxs-lookup"><span data-stu-id="bbd63-152">String</span></span>|<span data-ttu-id="bbd63-153">Описание устройства, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbd63-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bbd63-154">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="bbd63-154">enrollmentState</span></span>|[<span data-ttu-id="bbd63-155">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="bbd63-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="bbd63-156">Состояние устройства в Intune, наследуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="bbd63-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="bbd63-157">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="bbd63-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="bbd63-158">platform</span><span class="sxs-lookup"><span data-stu-id="bbd63-158">platform</span></span>|[<span data-ttu-id="bbd63-159">управляем</span><span class="sxs-lookup"><span data-stu-id="bbd63-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="bbd63-160">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="bbd63-160">The platform of the Device.</span></span> <span data-ttu-id="bbd63-161">Наследуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="bbd63-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="bbd63-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="bbd63-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="bbd63-163">status</span><span class="sxs-lookup"><span data-stu-id="bbd63-163">status</span></span>|<span data-ttu-id="bbd63-164">Логический</span><span class="sxs-lookup"><span data-stu-id="bbd63-164">Boolean</span></span>|<span data-ttu-id="bbd63-165">Состояние импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="bbd63-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="bbd63-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd63-166">Response</span></span>
<span data-ttu-id="bbd63-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbd63-167">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbd63-168">Пример</span><span class="sxs-lookup"><span data-stu-id="bbd63-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbd63-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbd63-169">Request</span></span>
<span data-ttu-id="bbd63-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbd63-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="bbd63-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd63-171">Response</span></span>
<span data-ttu-id="bbd63-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbd63-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






