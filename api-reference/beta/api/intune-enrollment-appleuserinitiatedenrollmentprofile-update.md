---
title: Обновление appleUserInitiatedEnrollmentProfile
description: Обновление свойств объекта appleUserInitiatedEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca6dda640ceaadb4420a41cf4bfd0e147f3d29f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146064"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="7d6a5-103">Обновление appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="7d6a5-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="7d6a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d6a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d6a5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d6a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d6a5-107">Обновление свойств объекта [appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d6a5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d6a5-108">Prerequisites</span></span>
<span data-ttu-id="7d6a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d6a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d6a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d6a5-111">Permission type</span></span>|<span data-ttu-id="7d6a5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d6a5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d6a5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d6a5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d6a5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d6a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-116">Not supported.</span></span>|
|<span data-ttu-id="7d6a5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d6a5-117">Application</span></span>|<span data-ttu-id="7d6a5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d6a5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d6a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d6a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="7d6a5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d6a5-120">Request headers</span></span>
|<span data-ttu-id="7d6a5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d6a5-121">Header</span></span>|<span data-ttu-id="7d6a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d6a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d6a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d6a5-123">Authorization</span></span>|<span data-ttu-id="7d6a5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d6a5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d6a5-125">Accept</span></span>|<span data-ttu-id="7d6a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d6a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d6a5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d6a5-127">Request body</span></span>
<span data-ttu-id="7d6a5-128">В теле запроса поставляем представление JSON для [объекта appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="7d6a5-129">В следующей таблице показаны свойства, необходимые при создании [appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="7d6a5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d6a5-130">Property</span></span>|<span data-ttu-id="7d6a5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7d6a5-131">Type</span></span>|<span data-ttu-id="7d6a5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7d6a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d6a5-133">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7d6a5-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="7d6a5-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7d6a5-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="7d6a5-135">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-135">The default profile enrollment type.</span></span> <span data-ttu-id="7d6a5-136">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="7d6a5-137">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="7d6a5-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="7d6a5-138">[коллекция appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="7d6a5-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="7d6a5-139">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="7d6a5-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="7d6a5-140">id</span><span class="sxs-lookup"><span data-stu-id="7d6a5-140">id</span></span>|<span data-ttu-id="7d6a5-141">Строка</span><span class="sxs-lookup"><span data-stu-id="7d6a5-141">String</span></span>|<span data-ttu-id="7d6a5-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="7d6a5-142">The GUID for the object</span></span>|
|<span data-ttu-id="7d6a5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7d6a5-143">displayName</span></span>|<span data-ttu-id="7d6a5-144">Строка</span><span class="sxs-lookup"><span data-stu-id="7d6a5-144">String</span></span>|<span data-ttu-id="7d6a5-145">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="7d6a5-145">Name of the profile</span></span>|
|<span data-ttu-id="7d6a5-146">description</span><span class="sxs-lookup"><span data-stu-id="7d6a5-146">description</span></span>|<span data-ttu-id="7d6a5-147">Строка</span><span class="sxs-lookup"><span data-stu-id="7d6a5-147">String</span></span>|<span data-ttu-id="7d6a5-148">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="7d6a5-148">Description of the profile</span></span>|
|<span data-ttu-id="7d6a5-149">priority</span><span class="sxs-lookup"><span data-stu-id="7d6a5-149">priority</span></span>|<span data-ttu-id="7d6a5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7d6a5-150">Int32</span></span>|<span data-ttu-id="7d6a5-151">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="7d6a5-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="7d6a5-152">платформа</span><span class="sxs-lookup"><span data-stu-id="7d6a5-152">platform</span></span>|[<span data-ttu-id="7d6a5-153">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="7d6a5-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="7d6a5-154">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-154">The platform of the Device.</span></span> <span data-ttu-id="7d6a5-155">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="7d6a5-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d6a5-156">createdDateTime</span></span>|<span data-ttu-id="7d6a5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d6a5-157">DateTimeOffset</span></span>|<span data-ttu-id="7d6a5-158">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="7d6a5-158">Profile creation time</span></span>|
|<span data-ttu-id="7d6a5-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d6a5-159">lastModifiedDateTime</span></span>|<span data-ttu-id="7d6a5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d6a5-160">DateTimeOffset</span></span>|<span data-ttu-id="7d6a5-161">Последнее изменение профиля</span><span class="sxs-lookup"><span data-stu-id="7d6a5-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="7d6a5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d6a5-162">Response</span></span>
<span data-ttu-id="7d6a5-163">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d6a5-164">Пример</span><span class="sxs-lookup"><span data-stu-id="7d6a5-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d6a5-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d6a5-165">Request</span></span>
<span data-ttu-id="7d6a5-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d6a5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d6a5-167">Response</span></span>
<span data-ttu-id="7d6a5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d6a5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




