---
title: Создание deviceManagementConfigurationPolicy
description: Создание нового объекта deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94410b8e7b3259a74893e93b450486398c5bef13
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129274"
---
# <a name="create-devicemanagementconfigurationpolicy"></a><span data-ttu-id="f0883-103">Создание deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f0883-103">Create deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="f0883-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0883-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0883-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0883-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0883-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0883-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0883-107">Создание нового [объекта deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f0883-107">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0883-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0883-108">Prerequisites</span></span>
<span data-ttu-id="f0883-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0883-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0883-111">Permission type</span></span>|<span data-ttu-id="f0883-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0883-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0883-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0883-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0883-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0883-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0883-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0883-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0883-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0883-116">Not supported.</span></span>|
|<span data-ttu-id="f0883-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0883-117">Application</span></span>|<span data-ttu-id="f0883-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0883-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0883-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0883-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f0883-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0883-120">Request headers</span></span>
|<span data-ttu-id="f0883-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0883-121">Header</span></span>|<span data-ttu-id="f0883-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0883-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0883-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0883-123">Authorization</span></span>|<span data-ttu-id="f0883-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0883-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0883-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0883-125">Accept</span></span>|<span data-ttu-id="f0883-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0883-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0883-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0883-127">Request body</span></span>
<span data-ttu-id="f0883-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="f0883-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicy object.</span></span>

<span data-ttu-id="f0883-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="f0883-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicy.</span></span>

|<span data-ttu-id="f0883-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0883-130">Property</span></span>|<span data-ttu-id="f0883-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0883-131">Type</span></span>|<span data-ttu-id="f0883-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0883-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0883-133">id</span><span class="sxs-lookup"><span data-stu-id="f0883-133">id</span></span>|<span data-ttu-id="f0883-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f0883-134">String</span></span>|<span data-ttu-id="f0883-135">Ключ документа политики.</span><span class="sxs-lookup"><span data-stu-id="f0883-135">Key of the policy document.</span></span> <span data-ttu-id="f0883-136">Автоматически созданный.</span><span class="sxs-lookup"><span data-stu-id="f0883-136">Automatically generated.</span></span>|
|<span data-ttu-id="f0883-137">name</span><span class="sxs-lookup"><span data-stu-id="f0883-137">name</span></span>|<span data-ttu-id="f0883-138">String</span><span class="sxs-lookup"><span data-stu-id="f0883-138">String</span></span>|<span data-ttu-id="f0883-139">Имя политики</span><span class="sxs-lookup"><span data-stu-id="f0883-139">Policy name</span></span>|
|<span data-ttu-id="f0883-140">description</span><span class="sxs-lookup"><span data-stu-id="f0883-140">description</span></span>|<span data-ttu-id="f0883-141">Строка</span><span class="sxs-lookup"><span data-stu-id="f0883-141">String</span></span>|<span data-ttu-id="f0883-142">Описание политики</span><span class="sxs-lookup"><span data-stu-id="f0883-142">Policy description</span></span>|
|<span data-ttu-id="f0883-143">платформы</span><span class="sxs-lookup"><span data-stu-id="f0883-143">platforms</span></span>|[<span data-ttu-id="f0883-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="f0883-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="f0883-145">Платформы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f0883-145">Platforms for this policy.</span></span> <span data-ttu-id="f0883-146">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="f0883-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="f0883-147">технологии</span><span class="sxs-lookup"><span data-stu-id="f0883-147">technologies</span></span>|[<span data-ttu-id="f0883-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="f0883-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="f0883-149">Технологии для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f0883-149">Technologies for this policy.</span></span> <span data-ttu-id="f0883-150">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f0883-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="f0883-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0883-151">createdDateTime</span></span>|<span data-ttu-id="f0883-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0883-152">DateTimeOffset</span></span>|<span data-ttu-id="f0883-153">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="f0883-153">Policy creation date and time.</span></span> <span data-ttu-id="f0883-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0883-154">This property is read-only.</span></span>|
|<span data-ttu-id="f0883-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0883-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f0883-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0883-156">DateTimeOffset</span></span>|<span data-ttu-id="f0883-157">Политика последней даты и времени изменения.</span><span class="sxs-lookup"><span data-stu-id="f0883-157">Policy last modification date and time.</span></span> <span data-ttu-id="f0883-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0883-158">This property is read-only.</span></span>|
|<span data-ttu-id="f0883-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="f0883-159">settingCount</span></span>|<span data-ttu-id="f0883-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f0883-160">Int32</span></span>|<span data-ttu-id="f0883-161">Количество параметров.</span><span class="sxs-lookup"><span data-stu-id="f0883-161">Number of settings.</span></span> <span data-ttu-id="f0883-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0883-162">This property is read-only.</span></span>|
|<span data-ttu-id="f0883-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="f0883-163">creationSource</span></span>|<span data-ttu-id="f0883-164">Строка</span><span class="sxs-lookup"><span data-stu-id="f0883-164">String</span></span>|<span data-ttu-id="f0883-165">Источник создания политики</span><span class="sxs-lookup"><span data-stu-id="f0883-165">Policy creation source</span></span>|
|<span data-ttu-id="f0883-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0883-166">roleScopeTagIds</span></span>|<span data-ttu-id="f0883-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0883-167">String collection</span></span>|<span data-ttu-id="f0883-168">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="f0883-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="f0883-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f0883-169">isAssigned</span></span>|<span data-ttu-id="f0883-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0883-170">Boolean</span></span>|<span data-ttu-id="f0883-171">Состояние назначения политики.</span><span class="sxs-lookup"><span data-stu-id="f0883-171">Policy assignment status.</span></span> <span data-ttu-id="f0883-172">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0883-172">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="f0883-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0883-173">Response</span></span>
<span data-ttu-id="f0883-174">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f0883-174">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0883-175">Пример</span><span class="sxs-lookup"><span data-stu-id="f0883-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0883-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0883-176">Request</span></span>
<span data-ttu-id="f0883-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0883-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="f0883-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0883-178">Response</span></span>
<span data-ttu-id="f0883-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0883-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 518

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```




