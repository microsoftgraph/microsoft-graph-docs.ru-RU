---
title: Обновление Апплеусеринитиатеденроллментпрофиле
description: Обновление свойств объекта Апплеусеринитиатеденроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ec83d3d9f4e8ca06d9f0f92752e9655b9fb469c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309692"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="e1ed5-103">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="e1ed5-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="e1ed5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ed5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1ed5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1ed5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1ed5-107">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e1ed5-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1ed5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1ed5-108">Prerequisites</span></span>
<span data-ttu-id="e1ed5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ed5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ed5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1ed5-111">Permission type</span></span>|<span data-ttu-id="e1ed5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1ed5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1ed5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ed5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1ed5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1ed5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-116">Not supported.</span></span>|
|<span data-ttu-id="e1ed5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1ed5-117">Application</span></span>|<span data-ttu-id="e1ed5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ed5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1ed5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1ed5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="e1ed5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1ed5-120">Request headers</span></span>
|<span data-ttu-id="e1ed5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1ed5-121">Header</span></span>|<span data-ttu-id="e1ed5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1ed5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1ed5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1ed5-123">Authorization</span></span>|<span data-ttu-id="e1ed5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1ed5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1ed5-125">Accept</span></span>|<span data-ttu-id="e1ed5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ed5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ed5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1ed5-127">Request body</span></span>
<span data-ttu-id="e1ed5-128">В тексте запроса добавьте представление объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="e1ed5-129">В следующей таблице приведены свойства, необходимые при создании [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e1ed5-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="e1ed5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1ed5-130">Property</span></span>|<span data-ttu-id="e1ed5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1ed5-131">Type</span></span>|<span data-ttu-id="e1ed5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ed5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ed5-133">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="e1ed5-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="e1ed5-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e1ed5-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="e1ed5-135">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-135">The default profile enrollment type.</span></span> <span data-ttu-id="e1ed5-136">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="e1ed5-137">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="e1ed5-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="e1ed5-138">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="e1ed5-139">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="e1ed5-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="e1ed5-140">id</span><span class="sxs-lookup"><span data-stu-id="e1ed5-140">id</span></span>|<span data-ttu-id="e1ed5-141">String</span><span class="sxs-lookup"><span data-stu-id="e1ed5-141">String</span></span>|<span data-ttu-id="e1ed5-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="e1ed5-142">The GUID for the object</span></span>|
|<span data-ttu-id="e1ed5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e1ed5-143">displayName</span></span>|<span data-ttu-id="e1ed5-144">String</span><span class="sxs-lookup"><span data-stu-id="e1ed5-144">String</span></span>|<span data-ttu-id="e1ed5-145">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="e1ed5-145">Name of the profile</span></span>|
|<span data-ttu-id="e1ed5-146">description</span><span class="sxs-lookup"><span data-stu-id="e1ed5-146">description</span></span>|<span data-ttu-id="e1ed5-147">String</span><span class="sxs-lookup"><span data-stu-id="e1ed5-147">String</span></span>|<span data-ttu-id="e1ed5-148">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="e1ed5-148">Description of the profile</span></span>|
|<span data-ttu-id="e1ed5-149">priority</span><span class="sxs-lookup"><span data-stu-id="e1ed5-149">priority</span></span>|<span data-ttu-id="e1ed5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ed5-150">Int32</span></span>|<span data-ttu-id="e1ed5-151">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="e1ed5-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="e1ed5-152">платформа</span><span class="sxs-lookup"><span data-stu-id="e1ed5-152">platform</span></span>|[<span data-ttu-id="e1ed5-153">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="e1ed5-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="e1ed5-154">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-154">The platform of the Device.</span></span> <span data-ttu-id="e1ed5-155">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="e1ed5-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ed5-156">createdDateTime</span></span>|<span data-ttu-id="e1ed5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ed5-157">DateTimeOffset</span></span>|<span data-ttu-id="e1ed5-158">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="e1ed5-158">Profile creation time</span></span>|
|<span data-ttu-id="e1ed5-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ed5-159">lastModifiedDateTime</span></span>|<span data-ttu-id="e1ed5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ed5-160">DateTimeOffset</span></span>|<span data-ttu-id="e1ed5-161">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="e1ed5-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="e1ed5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1ed5-162">Response</span></span>
<span data-ttu-id="e1ed5-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ed5-164">Пример</span><span class="sxs-lookup"><span data-stu-id="e1ed5-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1ed5-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1ed5-165">Request</span></span>
<span data-ttu-id="e1ed5-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1ed5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1ed5-167">Response</span></span>
<span data-ttu-id="e1ed5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




