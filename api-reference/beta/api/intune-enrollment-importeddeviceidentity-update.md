---
title: Обновление importedDeviceIdentity
description: Обновление свойств объекта importedDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: decc169b9f1b404c03691323bb0686309cb603c4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142298"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="80b60-103">Обновление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="80b60-103">Update importedDeviceIdentity</span></span>

<span data-ttu-id="80b60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80b60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80b60-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80b60-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80b60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80b60-107">Обновление свойств объекта [importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="80b60-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80b60-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="80b60-108">Prerequisites</span></span>
<span data-ttu-id="80b60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80b60-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80b60-111">Permission type</span></span>|<span data-ttu-id="80b60-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80b60-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80b60-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80b60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80b60-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80b60-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80b60-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80b60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80b60-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b60-116">Not supported.</span></span>|
|<span data-ttu-id="80b60-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="80b60-117">Application</span></span>|<span data-ttu-id="80b60-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80b60-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80b60-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80b60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="80b60-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80b60-120">Request headers</span></span>
|<span data-ttu-id="80b60-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80b60-121">Header</span></span>|<span data-ttu-id="80b60-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80b60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80b60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80b60-123">Authorization</span></span>|<span data-ttu-id="80b60-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80b60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80b60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80b60-125">Accept</span></span>|<span data-ttu-id="80b60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80b60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80b60-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80b60-127">Request body</span></span>
<span data-ttu-id="80b60-128">В теле запроса поставляем представление JSON для [объекта importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="80b60-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="80b60-129">В следующей таблице показаны свойства, необходимые при создании [объекта importedDeviceId.](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="80b60-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="80b60-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="80b60-130">Property</span></span>|<span data-ttu-id="80b60-131">Тип</span><span class="sxs-lookup"><span data-stu-id="80b60-131">Type</span></span>|<span data-ttu-id="80b60-132">Описание</span><span class="sxs-lookup"><span data-stu-id="80b60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80b60-133">id</span><span class="sxs-lookup"><span data-stu-id="80b60-133">id</span></span>|<span data-ttu-id="80b60-134">Строка</span><span class="sxs-lookup"><span data-stu-id="80b60-134">String</span></span>|<span data-ttu-id="80b60-135">Идентификатор импортируемого удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="80b60-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="80b60-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="80b60-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="80b60-137">Строка</span><span class="sxs-lookup"><span data-stu-id="80b60-137">String</span></span>|<span data-ttu-id="80b60-138">Идентификатор импортируемого устройства</span><span class="sxs-lookup"><span data-stu-id="80b60-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="80b60-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="80b60-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="80b60-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="80b60-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="80b60-141">Тип импортируемого удостоверения устройства.</span><span class="sxs-lookup"><span data-stu-id="80b60-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="80b60-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="80b60-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="80b60-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80b60-143">lastModifiedDateTime</span></span>|<span data-ttu-id="80b60-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80b60-144">DateTimeOffset</span></span>|<span data-ttu-id="80b60-145">Последнее изменение dateTime описания</span><span class="sxs-lookup"><span data-stu-id="80b60-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="80b60-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80b60-146">createdDateTime</span></span>|<span data-ttu-id="80b60-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80b60-147">DateTimeOffset</span></span>|<span data-ttu-id="80b60-148">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="80b60-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="80b60-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="80b60-149">lastContactedDateTime</span></span>|<span data-ttu-id="80b60-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80b60-150">DateTimeOffset</span></span>|<span data-ttu-id="80b60-151">Время последней контактной даты устройства</span><span class="sxs-lookup"><span data-stu-id="80b60-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="80b60-152">description</span><span class="sxs-lookup"><span data-stu-id="80b60-152">description</span></span>|<span data-ttu-id="80b60-153">Строка</span><span class="sxs-lookup"><span data-stu-id="80b60-153">String</span></span>|<span data-ttu-id="80b60-154">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="80b60-154">The description of the device</span></span>|
|<span data-ttu-id="80b60-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="80b60-155">enrollmentState</span></span>|[<span data-ttu-id="80b60-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="80b60-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="80b60-157">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="80b60-157">The state of the device in Intune.</span></span> <span data-ttu-id="80b60-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="80b60-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="80b60-159">платформа</span><span class="sxs-lookup"><span data-stu-id="80b60-159">platform</span></span>|[<span data-ttu-id="80b60-160">платформа</span><span class="sxs-lookup"><span data-stu-id="80b60-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="80b60-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="80b60-161">The platform of the Device.</span></span> <span data-ttu-id="80b60-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="80b60-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="80b60-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="80b60-163">Response</span></span>
<span data-ttu-id="80b60-164">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="80b60-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80b60-165">Пример</span><span class="sxs-lookup"><span data-stu-id="80b60-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="80b60-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="80b60-166">Request</span></span>
<span data-ttu-id="80b60-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80b60-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80b60-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="80b60-168">Response</span></span>
<span data-ttu-id="80b60-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80b60-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




