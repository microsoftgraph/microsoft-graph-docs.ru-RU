---
title: Создание Импортеддевицеидентитиресулт
description: Создание нового объекта Импортеддевицеидентитиресулт.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa030a98f59c587ff42033794cac31ee78b030b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167188"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="75618-103">Создание Импортеддевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="75618-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="75618-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75618-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75618-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75618-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75618-106">Создание нового объекта [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="75618-106">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75618-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75618-107">Prerequisites</span></span>
<span data-ttu-id="75618-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="75618-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="75618-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75618-110">Permission type</span></span>|<span data-ttu-id="75618-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75618-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75618-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75618-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75618-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75618-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="75618-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75618-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75618-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75618-115">Not supported.</span></span>|
|<span data-ttu-id="75618-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75618-116">Application</span></span>|<span data-ttu-id="75618-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75618-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75618-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75618-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="75618-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75618-119">Request headers</span></span>
|<span data-ttu-id="75618-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75618-120">Header</span></span>|<span data-ttu-id="75618-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75618-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75618-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75618-122">Authorization</span></span>|<span data-ttu-id="75618-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="75618-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75618-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75618-124">Accept</span></span>|<span data-ttu-id="75618-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75618-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75618-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75618-126">Request body</span></span>
<span data-ttu-id="75618-127">В тексте запроса добавьте представление объекта Импортеддевицеидентитиресулт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75618-127">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="75618-128">В следующей таблице приведены свойства, необходимые при создании Импортеддевицеидентитиресулт.</span><span class="sxs-lookup"><span data-stu-id="75618-128">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="75618-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75618-129">Property</span></span>|<span data-ttu-id="75618-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75618-130">Type</span></span>|<span data-ttu-id="75618-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75618-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75618-132">id</span><span class="sxs-lookup"><span data-stu-id="75618-132">id</span></span>|<span data-ttu-id="75618-133">String</span><span class="sxs-lookup"><span data-stu-id="75618-133">String</span></span>|<span data-ttu-id="75618-134">Идентификатор импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75618-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75618-135">Импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="75618-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="75618-136">String</span><span class="sxs-lookup"><span data-stu-id="75618-136">String</span></span>|<span data-ttu-id="75618-137">Импортированный идентификатор устройства, наСледуемый от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75618-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75618-138">Импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="75618-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="75618-139">Импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="75618-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="75618-140">Тип импортированного удостоверения устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="75618-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="75618-141">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="75618-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="75618-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75618-142">lastModifiedDateTime</span></span>|<span data-ttu-id="75618-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75618-143">DateTimeOffset</span></span>|<span data-ttu-id="75618-144">Дата и время последнего изменения описания, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75618-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75618-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75618-145">createdDateTime</span></span>|<span data-ttu-id="75618-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75618-146">DateTimeOffset</span></span>|<span data-ttu-id="75618-147">Дата и время создания устройства, унаследованного от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75618-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75618-148">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="75618-148">lastContactedDateTime</span></span>|<span data-ttu-id="75618-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75618-149">DateTimeOffset</span></span>|<span data-ttu-id="75618-150">Дата и время последнего обращения к устройству, унаследованному от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75618-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75618-151">description</span><span class="sxs-lookup"><span data-stu-id="75618-151">description</span></span>|<span data-ttu-id="75618-152">String</span><span class="sxs-lookup"><span data-stu-id="75618-152">String</span></span>|<span data-ttu-id="75618-153">Описание устройства, наСледуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75618-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75618-154">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="75618-154">enrollmentState</span></span>|[<span data-ttu-id="75618-155">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="75618-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="75618-156">Состояние устройства в Intune, наСледуемого из [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="75618-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="75618-157">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="75618-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="75618-158">platform</span><span class="sxs-lookup"><span data-stu-id="75618-158">platform</span></span>|[<span data-ttu-id="75618-159">управляем</span><span class="sxs-lookup"><span data-stu-id="75618-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="75618-160">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="75618-160">The platform of the Device.</span></span> <span data-ttu-id="75618-161">НаСледуется от [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="75618-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="75618-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="75618-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="75618-163">status</span><span class="sxs-lookup"><span data-stu-id="75618-163">status</span></span>|<span data-ttu-id="75618-164">Логический</span><span class="sxs-lookup"><span data-stu-id="75618-164">Boolean</span></span>|<span data-ttu-id="75618-165">Состояние импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="75618-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="75618-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="75618-166">Response</span></span>
<span data-ttu-id="75618-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75618-167">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75618-168">Пример</span><span class="sxs-lookup"><span data-stu-id="75618-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="75618-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="75618-169">Request</span></span>
<span data-ttu-id="75618-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75618-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75618-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="75618-171">Response</span></span>
<span data-ttu-id="75618-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75618-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




