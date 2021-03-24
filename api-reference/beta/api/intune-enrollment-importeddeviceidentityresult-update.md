---
title: Обновление importedDeviceIdentityResult
description: Обновление свойств импортируемого объектаDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36f71f2d4d1494e459e2cf9f9867d354a931a2f1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142221"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="7a66a-103">Обновление importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="7a66a-103">Update importedDeviceIdentityResult</span></span>

<span data-ttu-id="7a66a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a66a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a66a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a66a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a66a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a66a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a66a-107">Обновление свойств импортируемого [объектаDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a66a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a66a-108">Prerequisites</span></span>
<span data-ttu-id="7a66a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a66a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a66a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a66a-111">Permission type</span></span>|<span data-ttu-id="7a66a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a66a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a66a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a66a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a66a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a66a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7a66a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a66a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a66a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a66a-116">Not supported.</span></span>|
|<span data-ttu-id="7a66a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7a66a-117">Application</span></span>|<span data-ttu-id="7a66a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a66a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a66a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a66a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="7a66a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a66a-120">Request headers</span></span>
|<span data-ttu-id="7a66a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a66a-121">Header</span></span>|<span data-ttu-id="7a66a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a66a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a66a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a66a-123">Authorization</span></span>|<span data-ttu-id="7a66a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a66a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a66a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a66a-125">Accept</span></span>|<span data-ttu-id="7a66a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a66a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a66a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a66a-127">Request body</span></span>
<span data-ttu-id="7a66a-128">В теле запроса поставляем представление JSON для [объекта importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="7a66a-129">В следующей таблице показаны свойства, необходимые при создании [импортируемогоDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="7a66a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a66a-130">Property</span></span>|<span data-ttu-id="7a66a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a66a-131">Type</span></span>|<span data-ttu-id="7a66a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a66a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a66a-133">id</span><span class="sxs-lookup"><span data-stu-id="7a66a-133">id</span></span>|<span data-ttu-id="7a66a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7a66a-134">String</span></span>|<span data-ttu-id="7a66a-135">Идентификатор импортируемого удостоверения устройства, унаследованный от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7a66a-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7a66a-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="7a66a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7a66a-137">String</span></span>|<span data-ttu-id="7a66a-138">Импортируемый идентификатор устройства, унаследованный от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7a66a-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7a66a-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="7a66a-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7a66a-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="7a66a-141">Тип импортируемого удостоверения устройства, унаследованный от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="7a66a-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7a66a-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="7a66a-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="7a66a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a66a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7a66a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a66a-144">DateTimeOffset</span></span>|<span data-ttu-id="7a66a-145">Последнее изменение dateTime описания, унаследованной от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7a66a-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a66a-146">createdDateTime</span></span>|<span data-ttu-id="7a66a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a66a-147">DateTimeOffset</span></span>|<span data-ttu-id="7a66a-148">Время создания даты устройства, унаследованной от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7a66a-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a66a-149">lastContactedDateTime</span></span>|<span data-ttu-id="7a66a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a66a-150">DateTimeOffset</span></span>|<span data-ttu-id="7a66a-151">Время последней контактируемой даты устройства, унаследованной от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7a66a-152">description</span><span class="sxs-lookup"><span data-stu-id="7a66a-152">description</span></span>|<span data-ttu-id="7a66a-153">Строка</span><span class="sxs-lookup"><span data-stu-id="7a66a-153">String</span></span>|<span data-ttu-id="7a66a-154">Описание устройства, унаследованной от [импортируемогоDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7a66a-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7a66a-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7a66a-155">enrollmentState</span></span>|[<span data-ttu-id="7a66a-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7a66a-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="7a66a-157">Состояние устройства в Intune Наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="7a66a-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7a66a-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="7a66a-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7a66a-159">платформа</span><span class="sxs-lookup"><span data-stu-id="7a66a-159">platform</span></span>|[<span data-ttu-id="7a66a-160">платформа</span><span class="sxs-lookup"><span data-stu-id="7a66a-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7a66a-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="7a66a-161">The platform of the Device.</span></span> <span data-ttu-id="7a66a-162">Наследуется [от importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="7a66a-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7a66a-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="7a66a-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="7a66a-164">status</span><span class="sxs-lookup"><span data-stu-id="7a66a-164">status</span></span>|<span data-ttu-id="7a66a-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a66a-165">Boolean</span></span>|<span data-ttu-id="7a66a-166">Состояние удостоверения импортируемого устройства</span><span class="sxs-lookup"><span data-stu-id="7a66a-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="7a66a-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a66a-167">Response</span></span>
<span data-ttu-id="7a66a-168">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [импортируемый объектDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7a66a-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a66a-169">Пример</span><span class="sxs-lookup"><span data-stu-id="7a66a-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a66a-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a66a-170">Request</span></span>
<span data-ttu-id="7a66a-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a66a-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7a66a-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a66a-172">Response</span></span>
<span data-ttu-id="7a66a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a66a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




