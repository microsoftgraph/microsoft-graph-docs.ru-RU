---
title: Создание Девицеманажементконфигуратионполици
description: Создание нового объекта Девицеманажементконфигуратионполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 044059bddb9893fb4c7f2520a56d1774f6b47792
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242312"
---
# <a name="create-devicemanagementconfigurationpolicy"></a><span data-ttu-id="84eae-103">Создание Девицеманажементконфигуратионполици</span><span class="sxs-lookup"><span data-stu-id="84eae-103">Create deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="84eae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84eae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84eae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84eae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84eae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84eae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84eae-107">Создание нового объекта [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="84eae-107">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84eae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84eae-108">Prerequisites</span></span>
<span data-ttu-id="84eae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84eae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84eae-111">Permission type</span></span>|<span data-ttu-id="84eae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84eae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84eae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84eae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84eae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84eae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84eae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84eae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84eae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84eae-116">Not supported.</span></span>|
|<span data-ttu-id="84eae-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="84eae-117">Application</span></span>|<span data-ttu-id="84eae-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84eae-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84eae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84eae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="84eae-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84eae-120">Request headers</span></span>
|<span data-ttu-id="84eae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84eae-121">Header</span></span>|<span data-ttu-id="84eae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84eae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84eae-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84eae-123">Authorization</span></span>|<span data-ttu-id="84eae-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84eae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84eae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84eae-125">Accept</span></span>|<span data-ttu-id="84eae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84eae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84eae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84eae-127">Request body</span></span>
<span data-ttu-id="84eae-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратионполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84eae-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicy object.</span></span>

<span data-ttu-id="84eae-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратионполици.</span><span class="sxs-lookup"><span data-stu-id="84eae-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicy.</span></span>

|<span data-ttu-id="84eae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84eae-130">Property</span></span>|<span data-ttu-id="84eae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84eae-131">Type</span></span>|<span data-ttu-id="84eae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84eae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84eae-133">id</span><span class="sxs-lookup"><span data-stu-id="84eae-133">id</span></span>|<span data-ttu-id="84eae-134">String</span><span class="sxs-lookup"><span data-stu-id="84eae-134">String</span></span>|<span data-ttu-id="84eae-135">Ключ документа политики.</span><span class="sxs-lookup"><span data-stu-id="84eae-135">Key of the policy document.</span></span> <span data-ttu-id="84eae-136">Создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="84eae-136">Automatically generated.</span></span>|
|<span data-ttu-id="84eae-137">name</span><span class="sxs-lookup"><span data-stu-id="84eae-137">name</span></span>|<span data-ttu-id="84eae-138">String</span><span class="sxs-lookup"><span data-stu-id="84eae-138">String</span></span>|<span data-ttu-id="84eae-139">Имя политики</span><span class="sxs-lookup"><span data-stu-id="84eae-139">Policy name</span></span>|
|<span data-ttu-id="84eae-140">description</span><span class="sxs-lookup"><span data-stu-id="84eae-140">description</span></span>|<span data-ttu-id="84eae-141">String</span><span class="sxs-lookup"><span data-stu-id="84eae-141">String</span></span>|<span data-ttu-id="84eae-142">Описание политики</span><span class="sxs-lookup"><span data-stu-id="84eae-142">Policy description</span></span>|
|<span data-ttu-id="84eae-143">Embedded</span><span class="sxs-lookup"><span data-stu-id="84eae-143">platforms</span></span>|[<span data-ttu-id="84eae-144">девицеманажементконфигуратионплатформс</span><span class="sxs-lookup"><span data-stu-id="84eae-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="84eae-145">Платформы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="84eae-145">Platforms for this policy.</span></span> <span data-ttu-id="84eae-146">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="84eae-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="84eae-147">технологически</span><span class="sxs-lookup"><span data-stu-id="84eae-147">technologies</span></span>|[<span data-ttu-id="84eae-148">девицеманажементконфигуратионтечнологиес</span><span class="sxs-lookup"><span data-stu-id="84eae-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="84eae-149">Технологии для этой политики.</span><span class="sxs-lookup"><span data-stu-id="84eae-149">Technologies for this policy.</span></span> <span data-ttu-id="84eae-150">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="84eae-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="84eae-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84eae-151">createdDateTime</span></span>|<span data-ttu-id="84eae-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84eae-152">DateTimeOffset</span></span>|<span data-ttu-id="84eae-153">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="84eae-153">Policy creation date and time.</span></span> <span data-ttu-id="84eae-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84eae-154">This property is read-only.</span></span>|
|<span data-ttu-id="84eae-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84eae-155">lastModifiedDateTime</span></span>|<span data-ttu-id="84eae-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84eae-156">DateTimeOffset</span></span>|<span data-ttu-id="84eae-157">Дата и время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="84eae-157">Policy last modification date and time.</span></span> <span data-ttu-id="84eae-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84eae-158">This property is read-only.</span></span>|
|<span data-ttu-id="84eae-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="84eae-159">settingCount</span></span>|<span data-ttu-id="84eae-160">Int32</span><span class="sxs-lookup"><span data-stu-id="84eae-160">Int32</span></span>|<span data-ttu-id="84eae-161">Количество параметров.</span><span class="sxs-lookup"><span data-stu-id="84eae-161">Number of settings.</span></span> <span data-ttu-id="84eae-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84eae-162">This property is read-only.</span></span>|
|<span data-ttu-id="84eae-163">креатионсаурце</span><span class="sxs-lookup"><span data-stu-id="84eae-163">creationSource</span></span>|<span data-ttu-id="84eae-164">String</span><span class="sxs-lookup"><span data-stu-id="84eae-164">String</span></span>|<span data-ttu-id="84eae-165">Источник создания политики</span><span class="sxs-lookup"><span data-stu-id="84eae-165">Policy creation source</span></span>|
|<span data-ttu-id="84eae-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84eae-166">roleScopeTagIds</span></span>|<span data-ttu-id="84eae-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="84eae-167">String collection</span></span>|<span data-ttu-id="84eae-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="84eae-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="84eae-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="84eae-169">isAssigned</span></span>|<span data-ttu-id="84eae-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="84eae-170">Boolean</span></span>|<span data-ttu-id="84eae-171">Состояние назначения политики.</span><span class="sxs-lookup"><span data-stu-id="84eae-171">Policy assignment status.</span></span> <span data-ttu-id="84eae-172">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84eae-172">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="84eae-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="84eae-173">Response</span></span>
<span data-ttu-id="84eae-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84eae-174">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84eae-175">Пример</span><span class="sxs-lookup"><span data-stu-id="84eae-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="84eae-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="84eae-176">Request</span></span>
<span data-ttu-id="84eae-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84eae-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84eae-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="84eae-178">Response</span></span>
<span data-ttu-id="84eae-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84eae-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




