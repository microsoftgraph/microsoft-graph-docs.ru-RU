---
title: Создание Импортеддевицеидентити
description: Создание нового объекта Импортеддевицеидентити.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47556de0dad4de9fee7fa1406d862ca39363b214
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228255"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="d4e50-103">Создание Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="d4e50-103">Create importedDeviceIdentity</span></span>

<span data-ttu-id="d4e50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4e50-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4e50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e50-107">Создание нового объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d4e50-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e50-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4e50-108">Prerequisites</span></span>
<span data-ttu-id="d4e50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4e50-111">Permission type</span></span>|<span data-ttu-id="d4e50-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4e50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4e50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e50-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e50-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4e50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e50-116">Not supported.</span></span>|
|<span data-ttu-id="d4e50-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4e50-117">Application</span></span>|<span data-ttu-id="d4e50-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e50-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4e50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d4e50-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4e50-120">Request headers</span></span>
|<span data-ttu-id="d4e50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4e50-121">Header</span></span>|<span data-ttu-id="d4e50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4e50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e50-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4e50-123">Authorization</span></span>|<span data-ttu-id="d4e50-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4e50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4e50-125">Accept</span></span>|<span data-ttu-id="d4e50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4e50-127">Request body</span></span>
<span data-ttu-id="d4e50-128">В тексте запроса добавьте представление объекта Импортеддевицеидентити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e50-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="d4e50-129">В следующей таблице приведены свойства, необходимые при создании Импортеддевицеидентити.</span><span class="sxs-lookup"><span data-stu-id="d4e50-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="d4e50-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4e50-130">Property</span></span>|<span data-ttu-id="d4e50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4e50-131">Type</span></span>|<span data-ttu-id="d4e50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4e50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e50-133">id</span><span class="sxs-lookup"><span data-stu-id="d4e50-133">id</span></span>|<span data-ttu-id="d4e50-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e50-134">String</span></span>|<span data-ttu-id="d4e50-135">Идентификатор импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="d4e50-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="d4e50-136">импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="d4e50-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="d4e50-137">String</span><span class="sxs-lookup"><span data-stu-id="d4e50-137">String</span></span>|<span data-ttu-id="d4e50-138">Импортированный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="d4e50-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="d4e50-139">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="d4e50-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="d4e50-140">импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="d4e50-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="d4e50-141">Тип импортированного удостоверения устройства.</span><span class="sxs-lookup"><span data-stu-id="d4e50-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="d4e50-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="d4e50-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="d4e50-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e50-143">lastModifiedDateTime</span></span>|<span data-ttu-id="d4e50-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e50-144">DateTimeOffset</span></span>|<span data-ttu-id="d4e50-145">Дата и время последнего изменения описания</span><span class="sxs-lookup"><span data-stu-id="d4e50-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="d4e50-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e50-146">createdDateTime</span></span>|<span data-ttu-id="d4e50-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e50-147">DateTimeOffset</span></span>|<span data-ttu-id="d4e50-148">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="d4e50-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="d4e50-149">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="d4e50-149">lastContactedDateTime</span></span>|<span data-ttu-id="d4e50-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e50-150">DateTimeOffset</span></span>|<span data-ttu-id="d4e50-151">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="d4e50-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="d4e50-152">description</span><span class="sxs-lookup"><span data-stu-id="d4e50-152">description</span></span>|<span data-ttu-id="d4e50-153">String</span><span class="sxs-lookup"><span data-stu-id="d4e50-153">String</span></span>|<span data-ttu-id="d4e50-154">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="d4e50-154">The description of the device</span></span>|
|<span data-ttu-id="d4e50-155">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="d4e50-155">enrollmentState</span></span>|[<span data-ttu-id="d4e50-156">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="d4e50-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="d4e50-157">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="d4e50-157">The state of the device in Intune.</span></span> <span data-ttu-id="d4e50-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d4e50-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d4e50-159">платформа</span><span class="sxs-lookup"><span data-stu-id="d4e50-159">platform</span></span>|[<span data-ttu-id="d4e50-160">платформа</span><span class="sxs-lookup"><span data-stu-id="d4e50-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d4e50-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="d4e50-161">The platform of the Device.</span></span> <span data-ttu-id="d4e50-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="d4e50-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="d4e50-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e50-163">Response</span></span>
<span data-ttu-id="d4e50-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4e50-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e50-165">Пример</span><span class="sxs-lookup"><span data-stu-id="d4e50-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e50-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4e50-166">Request</span></span>
<span data-ttu-id="d4e50-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4e50-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4e50-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e50-168">Response</span></span>
<span data-ttu-id="d4e50-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4e50-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




