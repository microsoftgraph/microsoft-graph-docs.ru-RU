---
title: Создание Апплеусеринитиатеденроллментпрофиле
description: Создание нового объекта Апплеусеринитиатеденроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f39e754c57a9401e6fcb17e76411900a83256571
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090496"
---
# <a name="create-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="aec07-103">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="aec07-103">Create appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="aec07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aec07-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aec07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aec07-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aec07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec07-107">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="aec07-107">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aec07-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aec07-108">Prerequisites</span></span>
<span data-ttu-id="aec07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aec07-111">Permission type</span></span>|<span data-ttu-id="aec07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aec07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aec07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aec07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aec07-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec07-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aec07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aec07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aec07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aec07-116">Not supported.</span></span>|
|<span data-ttu-id="aec07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aec07-117">Application</span></span>|<span data-ttu-id="aec07-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec07-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aec07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aec07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="aec07-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aec07-120">Request headers</span></span>
|<span data-ttu-id="aec07-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aec07-121">Header</span></span>|<span data-ttu-id="aec07-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aec07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aec07-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aec07-123">Authorization</span></span>|<span data-ttu-id="aec07-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aec07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aec07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aec07-125">Accept</span></span>|<span data-ttu-id="aec07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aec07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aec07-127">Request body</span></span>
<span data-ttu-id="aec07-128">В тексте запроса добавьте представление объекта Апплеусеринитиатеденроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aec07-128">In the request body, supply a JSON representation for the appleUserInitiatedEnrollmentProfile object.</span></span>

<span data-ttu-id="aec07-129">В следующей таблице приведены свойства, необходимые при создании Апплеусеринитиатеденроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="aec07-129">The following table shows the properties that are required when you create the appleUserInitiatedEnrollmentProfile.</span></span>

|<span data-ttu-id="aec07-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aec07-130">Property</span></span>|<span data-ttu-id="aec07-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aec07-131">Type</span></span>|<span data-ttu-id="aec07-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aec07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec07-133">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="aec07-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="aec07-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="aec07-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="aec07-135">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="aec07-135">The default profile enrollment type.</span></span> <span data-ttu-id="aec07-136">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="aec07-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="aec07-137">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="aec07-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="aec07-138">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="aec07-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="aec07-139">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="aec07-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="aec07-140">id</span><span class="sxs-lookup"><span data-stu-id="aec07-140">id</span></span>|<span data-ttu-id="aec07-141">Строка</span><span class="sxs-lookup"><span data-stu-id="aec07-141">String</span></span>|<span data-ttu-id="aec07-142">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="aec07-142">The GUID for the object</span></span>|
|<span data-ttu-id="aec07-143">displayName</span><span class="sxs-lookup"><span data-stu-id="aec07-143">displayName</span></span>|<span data-ttu-id="aec07-144">Строка</span><span class="sxs-lookup"><span data-stu-id="aec07-144">String</span></span>|<span data-ttu-id="aec07-145">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="aec07-145">Name of the profile</span></span>|
|<span data-ttu-id="aec07-146">description</span><span class="sxs-lookup"><span data-stu-id="aec07-146">description</span></span>|<span data-ttu-id="aec07-147">Строка</span><span class="sxs-lookup"><span data-stu-id="aec07-147">String</span></span>|<span data-ttu-id="aec07-148">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="aec07-148">Description of the profile</span></span>|
|<span data-ttu-id="aec07-149">priority</span><span class="sxs-lookup"><span data-stu-id="aec07-149">priority</span></span>|<span data-ttu-id="aec07-150">Int32</span><span class="sxs-lookup"><span data-stu-id="aec07-150">Int32</span></span>|<span data-ttu-id="aec07-151">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="aec07-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="aec07-152">платформа</span><span class="sxs-lookup"><span data-stu-id="aec07-152">platform</span></span>|[<span data-ttu-id="aec07-153">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="aec07-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="aec07-154">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="aec07-154">The platform of the Device.</span></span> <span data-ttu-id="aec07-155">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="aec07-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="aec07-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aec07-156">createdDateTime</span></span>|<span data-ttu-id="aec07-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec07-157">DateTimeOffset</span></span>|<span data-ttu-id="aec07-158">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="aec07-158">Profile creation time</span></span>|
|<span data-ttu-id="aec07-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aec07-159">lastModifiedDateTime</span></span>|<span data-ttu-id="aec07-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec07-160">DateTimeOffset</span></span>|<span data-ttu-id="aec07-161">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="aec07-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="aec07-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="aec07-162">Response</span></span>
<span data-ttu-id="aec07-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aec07-163">If successful, this method returns a `201 Created` response code and a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aec07-164">Пример</span><span class="sxs-lookup"><span data-stu-id="aec07-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="aec07-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="aec07-165">Request</span></span>
<span data-ttu-id="aec07-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aec07-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aec07-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="aec07-167">Response</span></span>
<span data-ttu-id="aec07-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aec07-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






