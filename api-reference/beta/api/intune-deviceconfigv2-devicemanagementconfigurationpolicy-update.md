---
title: Обновление deviceManagementConfigurationPolicy
description: Обновление свойств объекта deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 344b8c710a89be0cd187df995852ce03c2ee638b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868248"
---
# <a name="update-devicemanagementconfigurationpolicy"></a><span data-ttu-id="ff929-103">Обновление deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="ff929-103">Update deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="ff929-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff929-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff929-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff929-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff929-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff929-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff929-107">Обновление свойств объекта [deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ff929-107">Update the properties of a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff929-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff929-108">Prerequisites</span></span>
<span data-ttu-id="ff929-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff929-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff929-111">Permission type</span></span>|<span data-ttu-id="ff929-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff929-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff929-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff929-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff929-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff929-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff929-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff929-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff929-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff929-116">Not supported.</span></span>|
|<span data-ttu-id="ff929-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ff929-117">Application</span></span>|<span data-ttu-id="ff929-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff929-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff929-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff929-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
PATCH /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ff929-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff929-120">Request headers</span></span>
|<span data-ttu-id="ff929-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff929-121">Header</span></span>|<span data-ttu-id="ff929-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff929-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff929-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff929-123">Authorization</span></span>|<span data-ttu-id="ff929-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff929-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff929-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff929-125">Accept</span></span>|<span data-ttu-id="ff929-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff929-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff929-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff929-127">Request body</span></span>
<span data-ttu-id="ff929-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ff929-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

<span data-ttu-id="ff929-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ff929-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span></span>

|<span data-ttu-id="ff929-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff929-130">Property</span></span>|<span data-ttu-id="ff929-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff929-131">Type</span></span>|<span data-ttu-id="ff929-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff929-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff929-133">id</span><span class="sxs-lookup"><span data-stu-id="ff929-133">id</span></span>|<span data-ttu-id="ff929-134">String</span><span class="sxs-lookup"><span data-stu-id="ff929-134">String</span></span>|<span data-ttu-id="ff929-135">Ключ документа политики.</span><span class="sxs-lookup"><span data-stu-id="ff929-135">Key of the policy document.</span></span> <span data-ttu-id="ff929-136">Автоматически созданный.</span><span class="sxs-lookup"><span data-stu-id="ff929-136">Automatically generated.</span></span>|
|<span data-ttu-id="ff929-137">name</span><span class="sxs-lookup"><span data-stu-id="ff929-137">name</span></span>|<span data-ttu-id="ff929-138">String</span><span class="sxs-lookup"><span data-stu-id="ff929-138">String</span></span>|<span data-ttu-id="ff929-139">Имя политики</span><span class="sxs-lookup"><span data-stu-id="ff929-139">Policy name</span></span>|
|<span data-ttu-id="ff929-140">description</span><span class="sxs-lookup"><span data-stu-id="ff929-140">description</span></span>|<span data-ttu-id="ff929-141">String</span><span class="sxs-lookup"><span data-stu-id="ff929-141">String</span></span>|<span data-ttu-id="ff929-142">Описание политики</span><span class="sxs-lookup"><span data-stu-id="ff929-142">Policy description</span></span>|
|<span data-ttu-id="ff929-143">платформы</span><span class="sxs-lookup"><span data-stu-id="ff929-143">platforms</span></span>|[<span data-ttu-id="ff929-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="ff929-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="ff929-145">Платформы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ff929-145">Platforms for this policy.</span></span> <span data-ttu-id="ff929-146">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="ff929-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="ff929-147">технологии</span><span class="sxs-lookup"><span data-stu-id="ff929-147">technologies</span></span>|[<span data-ttu-id="ff929-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="ff929-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="ff929-149">Технологии для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ff929-149">Technologies for this policy.</span></span> <span data-ttu-id="ff929-150">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ff929-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="ff929-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff929-151">createdDateTime</span></span>|<span data-ttu-id="ff929-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff929-152">DateTimeOffset</span></span>|<span data-ttu-id="ff929-153">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="ff929-153">Policy creation date and time.</span></span> <span data-ttu-id="ff929-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff929-154">This property is read-only.</span></span>|
|<span data-ttu-id="ff929-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff929-155">lastModifiedDateTime</span></span>|<span data-ttu-id="ff929-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff929-156">DateTimeOffset</span></span>|<span data-ttu-id="ff929-157">Политика последней даты и времени изменения.</span><span class="sxs-lookup"><span data-stu-id="ff929-157">Policy last modification date and time.</span></span> <span data-ttu-id="ff929-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff929-158">This property is read-only.</span></span>|
|<span data-ttu-id="ff929-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="ff929-159">settingCount</span></span>|<span data-ttu-id="ff929-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ff929-160">Int32</span></span>|<span data-ttu-id="ff929-161">Количество параметров.</span><span class="sxs-lookup"><span data-stu-id="ff929-161">Number of settings.</span></span> <span data-ttu-id="ff929-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff929-162">This property is read-only.</span></span>|
|<span data-ttu-id="ff929-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="ff929-163">creationSource</span></span>|<span data-ttu-id="ff929-164">String</span><span class="sxs-lookup"><span data-stu-id="ff929-164">String</span></span>|<span data-ttu-id="ff929-165">Источник создания политики</span><span class="sxs-lookup"><span data-stu-id="ff929-165">Policy creation source</span></span>|
|<span data-ttu-id="ff929-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff929-166">roleScopeTagIds</span></span>|<span data-ttu-id="ff929-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff929-167">String collection</span></span>|<span data-ttu-id="ff929-168">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ff929-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="ff929-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ff929-169">isAssigned</span></span>|<span data-ttu-id="ff929-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff929-170">Boolean</span></span>|<span data-ttu-id="ff929-171">Состояние назначения политики.</span><span class="sxs-lookup"><span data-stu-id="ff929-171">Policy assignment status.</span></span> <span data-ttu-id="ff929-172">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff929-172">This property is read-only.</span></span>|
|<span data-ttu-id="ff929-173">templateReference</span><span class="sxs-lookup"><span data-stu-id="ff929-173">templateReference</span></span>|[<span data-ttu-id="ff929-174">deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="ff929-174">deviceManagementConfigurationPolicyTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplatereference.md)|<span data-ttu-id="ff929-175">Справочные сведения по шаблонам</span><span class="sxs-lookup"><span data-stu-id="ff929-175">Template reference information</span></span>|



## <a name="response"></a><span data-ttu-id="ff929-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff929-176">Response</span></span>
<span data-ttu-id="ff929-177">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ff929-177">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff929-178">Пример</span><span class="sxs-lookup"><span data-stu-id="ff929-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff929-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff929-179">Request</span></span>
<span data-ttu-id="ff929-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff929-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
Content-type: application/json
Content-length: 685

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
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "Template Id value",
    "templateFamily": "endpointSecurityAntivirus",
    "templateDisplayName": "Template Display Name value",
    "templateDisplayVersion": "Template Display Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ff929-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff929-181">Response</span></span>
<span data-ttu-id="ff929-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff929-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 857

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
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "Template Id value",
    "templateFamily": "endpointSecurityAntivirus",
    "templateDisplayName": "Template Display Name value",
    "templateDisplayVersion": "Template Display Version value"
  }
}
```




