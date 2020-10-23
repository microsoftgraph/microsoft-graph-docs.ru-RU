---
title: Обновление Апплеусеринитиатеденроллментпрофиле
description: Обновление свойств объекта Апплеусеринитиатеденроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bcd6ed9ee78ec96c189ae06d071f465da4659c3d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709455"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="c4a4d-103">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="c4a4d-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="c4a4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4a4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4a4d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4a4d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4a4d-107">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c4a4d-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4a4d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4a4d-108">Prerequisites</span></span>
<span data-ttu-id="c4a4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a4d-111">Permission type</span></span>|<span data-ttu-id="c4a4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4a4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4a4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a4d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a4d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4a4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4a4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-116">Not supported.</span></span>|
|<span data-ttu-id="c4a4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4a4d-117">Application</span></span>|<span data-ttu-id="c4a4d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a4d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4a4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4a4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="c4a4d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c4a4d-120">Request headers</span></span>
|<span data-ttu-id="c4a4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4a4d-121">Header</span></span>|<span data-ttu-id="c4a4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4a4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4a4d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4a4d-123">Authorization</span></span>|<span data-ttu-id="c4a4d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4a4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4a4d-125">Accept</span></span>|<span data-ttu-id="c4a4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4a4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a4d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4a4d-127">Request body</span></span>
<span data-ttu-id="c4a4d-128">В тексте запроса добавьте представление объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="c4a4d-129">В следующей таблице приведены свойства, необходимые при создании [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c4a4d-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="c4a4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4a4d-130">Property</span></span>|<span data-ttu-id="c4a4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4a4d-131">Type</span></span>|<span data-ttu-id="c4a4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4a4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4a4d-133">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="c4a4d-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="c4a4d-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c4a4d-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="c4a4d-135">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-135">The default profile enrollment type.</span></span> <span data-ttu-id="c4a4d-136">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="c4a4d-137">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="c4a4d-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="c4a4d-138">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="c4a4d-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="c4a4d-139">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="c4a4d-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="c4a4d-140">id</span><span class="sxs-lookup"><span data-stu-id="c4a4d-140">id</span></span>|<span data-ttu-id="c4a4d-141">Строка</span><span class="sxs-lookup"><span data-stu-id="c4a4d-141">String</span></span>|<span data-ttu-id="c4a4d-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="c4a4d-142">The GUID for the object</span></span>|
|<span data-ttu-id="c4a4d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c4a4d-143">displayName</span></span>|<span data-ttu-id="c4a4d-144">Строка</span><span class="sxs-lookup"><span data-stu-id="c4a4d-144">String</span></span>|<span data-ttu-id="c4a4d-145">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="c4a4d-145">Name of the profile</span></span>|
|<span data-ttu-id="c4a4d-146">description</span><span class="sxs-lookup"><span data-stu-id="c4a4d-146">description</span></span>|<span data-ttu-id="c4a4d-147">Строка</span><span class="sxs-lookup"><span data-stu-id="c4a4d-147">String</span></span>|<span data-ttu-id="c4a4d-148">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="c4a4d-148">Description of the profile</span></span>|
|<span data-ttu-id="c4a4d-149">priority</span><span class="sxs-lookup"><span data-stu-id="c4a4d-149">priority</span></span>|<span data-ttu-id="c4a4d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c4a4d-150">Int32</span></span>|<span data-ttu-id="c4a4d-151">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="c4a4d-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="c4a4d-152">платформа</span><span class="sxs-lookup"><span data-stu-id="c4a4d-152">platform</span></span>|[<span data-ttu-id="c4a4d-153">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="c4a4d-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="c4a4d-154">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-154">The platform of the Device.</span></span> <span data-ttu-id="c4a4d-155">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="c4a4d-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4a4d-156">createdDateTime</span></span>|<span data-ttu-id="c4a4d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4a4d-157">DateTimeOffset</span></span>|<span data-ttu-id="c4a4d-158">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="c4a4d-158">Profile creation time</span></span>|
|<span data-ttu-id="c4a4d-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4a4d-159">lastModifiedDateTime</span></span>|<span data-ttu-id="c4a4d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4a4d-160">DateTimeOffset</span></span>|<span data-ttu-id="c4a4d-161">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="c4a4d-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="c4a4d-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4a4d-162">Response</span></span>
<span data-ttu-id="c4a4d-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a4d-164">Пример</span><span class="sxs-lookup"><span data-stu-id="c4a4d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4a4d-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4a4d-165">Request</span></span>
<span data-ttu-id="c4a4d-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="c4a4d-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4a4d-167">Response</span></span>
<span data-ttu-id="c4a4d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4a4d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





