---
title: Создание Апплеусеринитиатеденроллментпрофиле
description: Создание нового объекта Апплеусеринитиатеденроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2532b226d01158c2b1ea6b70478a7f3527cd879d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525793"
---
# <a name="create-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="67fe6-103">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="67fe6-103">Create appleUserInitiatedEnrollmentProfile</span></span>

> <span data-ttu-id="67fe6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67fe6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67fe6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67fe6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fe6-106">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="67fe6-106">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67fe6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67fe6-107">Prerequisites</span></span>
<span data-ttu-id="67fe6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67fe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67fe6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67fe6-110">Permission type</span></span>|<span data-ttu-id="67fe6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67fe6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67fe6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67fe6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67fe6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67fe6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67fe6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67fe6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67fe6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67fe6-115">Not supported.</span></span>|
|<span data-ttu-id="67fe6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="67fe6-116">Application</span></span>|<span data-ttu-id="67fe6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67fe6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67fe6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67fe6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="67fe6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67fe6-119">Request headers</span></span>
|<span data-ttu-id="67fe6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67fe6-120">Header</span></span>|<span data-ttu-id="67fe6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="67fe6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67fe6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67fe6-122">Authorization</span></span>|<span data-ttu-id="67fe6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67fe6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67fe6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="67fe6-124">Accept</span></span>|<span data-ttu-id="67fe6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67fe6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67fe6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67fe6-126">Request body</span></span>
<span data-ttu-id="67fe6-127">В тексте запроса добавьте представление объекта Апплеусеринитиатеденроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67fe6-127">In the request body, supply a JSON representation for the appleUserInitiatedEnrollmentProfile object.</span></span>

<span data-ttu-id="67fe6-128">В следующей таблице приведены свойства, необходимые при создании Апплеусеринитиатеденроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="67fe6-128">The following table shows the properties that are required when you create the appleUserInitiatedEnrollmentProfile.</span></span>

|<span data-ttu-id="67fe6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="67fe6-129">Property</span></span>|<span data-ttu-id="67fe6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="67fe6-130">Type</span></span>|<span data-ttu-id="67fe6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="67fe6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67fe6-132">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="67fe6-132">defaultEnrollmentType</span></span>|[<span data-ttu-id="67fe6-133">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="67fe6-133">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="67fe6-134">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="67fe6-134">The default profile enrollment type.</span></span> <span data-ttu-id="67fe6-135">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="67fe6-135">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="67fe6-136">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="67fe6-136">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="67fe6-137">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="67fe6-137">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="67fe6-138">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="67fe6-138">List of available enrollment type options</span></span>|
|<span data-ttu-id="67fe6-139">id</span><span class="sxs-lookup"><span data-stu-id="67fe6-139">id</span></span>|<span data-ttu-id="67fe6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="67fe6-140">String</span></span>|<span data-ttu-id="67fe6-141">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="67fe6-141">The GUID for the object</span></span>|
|<span data-ttu-id="67fe6-142">displayName</span><span class="sxs-lookup"><span data-stu-id="67fe6-142">displayName</span></span>|<span data-ttu-id="67fe6-143">Строка</span><span class="sxs-lookup"><span data-stu-id="67fe6-143">String</span></span>|<span data-ttu-id="67fe6-144">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="67fe6-144">Name of the profile</span></span>|
|<span data-ttu-id="67fe6-145">description</span><span class="sxs-lookup"><span data-stu-id="67fe6-145">description</span></span>|<span data-ttu-id="67fe6-146">String</span><span class="sxs-lookup"><span data-stu-id="67fe6-146">String</span></span>|<span data-ttu-id="67fe6-147">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="67fe6-147">Description of the profile</span></span>|
|<span data-ttu-id="67fe6-148">priority</span><span class="sxs-lookup"><span data-stu-id="67fe6-148">priority</span></span>|<span data-ttu-id="67fe6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="67fe6-149">Int32</span></span>|<span data-ttu-id="67fe6-150">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="67fe6-150">Priority, 0 is highest</span></span>|
|<span data-ttu-id="67fe6-151">platform</span><span class="sxs-lookup"><span data-stu-id="67fe6-151">platform</span></span>|[<span data-ttu-id="67fe6-152">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="67fe6-152">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="67fe6-153">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="67fe6-153">The platform of the Device.</span></span> <span data-ttu-id="67fe6-154">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="67fe6-154">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="67fe6-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67fe6-155">createdDateTime</span></span>|<span data-ttu-id="67fe6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67fe6-156">DateTimeOffset</span></span>|<span data-ttu-id="67fe6-157">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="67fe6-157">Profile creation time</span></span>|
|<span data-ttu-id="67fe6-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67fe6-158">lastModifiedDateTime</span></span>|<span data-ttu-id="67fe6-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67fe6-159">DateTimeOffset</span></span>|<span data-ttu-id="67fe6-160">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="67fe6-160">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="67fe6-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="67fe6-161">Response</span></span>
<span data-ttu-id="67fe6-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67fe6-162">If successful, this method returns a `201 Created` response code and a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67fe6-163">Пример</span><span class="sxs-lookup"><span data-stu-id="67fe6-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="67fe6-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="67fe6-164">Request</span></span>
<span data-ttu-id="67fe6-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67fe6-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="67fe6-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="67fe6-166">Response</span></span>
<span data-ttu-id="67fe6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67fe6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






