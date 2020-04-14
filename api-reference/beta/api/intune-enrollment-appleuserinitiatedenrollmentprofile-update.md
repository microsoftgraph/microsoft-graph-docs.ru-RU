---
title: Обновление Апплеусеринитиатеденроллментпрофиле
description: Обновление свойств объекта Апплеусеринитиатеденроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 961b4f863d2617b61b5f4276ccff80184979f42e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43320311"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="5ae09-103">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="5ae09-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="5ae09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ae09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ae09-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ae09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ae09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ae09-107">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5ae09-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ae09-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ae09-108">Prerequisites</span></span>
<span data-ttu-id="5ae09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ae09-111">Permission type</span></span>|<span data-ttu-id="5ae09-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ae09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ae09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae09-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae09-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ae09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae09-116">Not supported.</span></span>|
|<span data-ttu-id="5ae09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ae09-117">Application</span></span>|<span data-ttu-id="5ae09-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae09-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ae09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="5ae09-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ae09-120">Request headers</span></span>
|<span data-ttu-id="5ae09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ae09-121">Header</span></span>|<span data-ttu-id="5ae09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5ae09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ae09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ae09-123">Authorization</span></span>|<span data-ttu-id="5ae09-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ae09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ae09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ae09-125">Accept</span></span>|<span data-ttu-id="5ae09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ae09-127">Request body</span></span>
<span data-ttu-id="5ae09-128">В тексте запроса добавьте представление объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ae09-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="5ae09-129">В следующей таблице приведены свойства, необходимые при создании [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5ae09-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="5ae09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ae09-130">Property</span></span>|<span data-ttu-id="5ae09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ae09-131">Type</span></span>|<span data-ttu-id="5ae09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ae09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae09-133">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="5ae09-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="5ae09-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5ae09-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="5ae09-135">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5ae09-135">The default profile enrollment type.</span></span> <span data-ttu-id="5ae09-136">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="5ae09-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="5ae09-137">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="5ae09-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="5ae09-138">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="5ae09-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="5ae09-139">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="5ae09-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="5ae09-140">id</span><span class="sxs-lookup"><span data-stu-id="5ae09-140">id</span></span>|<span data-ttu-id="5ae09-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5ae09-141">String</span></span>|<span data-ttu-id="5ae09-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="5ae09-142">The GUID for the object</span></span>|
|<span data-ttu-id="5ae09-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5ae09-143">displayName</span></span>|<span data-ttu-id="5ae09-144">Строка</span><span class="sxs-lookup"><span data-stu-id="5ae09-144">String</span></span>|<span data-ttu-id="5ae09-145">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="5ae09-145">Name of the profile</span></span>|
|<span data-ttu-id="5ae09-146">description</span><span class="sxs-lookup"><span data-stu-id="5ae09-146">description</span></span>|<span data-ttu-id="5ae09-147">String</span><span class="sxs-lookup"><span data-stu-id="5ae09-147">String</span></span>|<span data-ttu-id="5ae09-148">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="5ae09-148">Description of the profile</span></span>|
|<span data-ttu-id="5ae09-149">priority</span><span class="sxs-lookup"><span data-stu-id="5ae09-149">priority</span></span>|<span data-ttu-id="5ae09-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae09-150">Int32</span></span>|<span data-ttu-id="5ae09-151">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="5ae09-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="5ae09-152">platform</span><span class="sxs-lookup"><span data-stu-id="5ae09-152">platform</span></span>|[<span data-ttu-id="5ae09-153">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="5ae09-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="5ae09-154">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="5ae09-154">The platform of the Device.</span></span> <span data-ttu-id="5ae09-155">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5ae09-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="5ae09-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae09-156">createdDateTime</span></span>|<span data-ttu-id="5ae09-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae09-157">DateTimeOffset</span></span>|<span data-ttu-id="5ae09-158">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="5ae09-158">Profile creation time</span></span>|
|<span data-ttu-id="5ae09-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae09-159">lastModifiedDateTime</span></span>|<span data-ttu-id="5ae09-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae09-160">DateTimeOffset</span></span>|<span data-ttu-id="5ae09-161">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="5ae09-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="5ae09-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae09-162">Response</span></span>
<span data-ttu-id="5ae09-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ae09-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ae09-164">Пример</span><span class="sxs-lookup"><span data-stu-id="5ae09-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ae09-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ae09-165">Request</span></span>
<span data-ttu-id="5ae09-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ae09-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ae09-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae09-167">Response</span></span>
<span data-ttu-id="5ae09-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ae09-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



