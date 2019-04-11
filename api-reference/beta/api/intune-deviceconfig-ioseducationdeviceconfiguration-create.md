---
title: Создание iosEducationDeviceConfiguration
description: Создание нового объекта iosEducationDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b848eff476d0e085d4ed8c39c6023d88b789a8f7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795655"
---
# <a name="create-ioseducationdeviceconfiguration"></a><span data-ttu-id="804a0-103">Создание iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="804a0-103">Create iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="804a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="804a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="804a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="804a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="804a0-106">Создание нового объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="804a0-106">Create a new [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="804a0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="804a0-107">Prerequisites</span></span>
<span data-ttu-id="804a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="804a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="804a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="804a0-110">Permission type</span></span>|<span data-ttu-id="804a0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="804a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="804a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="804a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="804a0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="804a0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="804a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="804a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="804a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="804a0-115">Not supported.</span></span>|
|<span data-ttu-id="804a0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="804a0-116">Application</span></span>|<span data-ttu-id="804a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="804a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="804a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="804a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="804a0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="804a0-119">Request headers</span></span>
|<span data-ttu-id="804a0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="804a0-120">Header</span></span>|<span data-ttu-id="804a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="804a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="804a0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="804a0-122">Authorization</span></span>|<span data-ttu-id="804a0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="804a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="804a0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="804a0-124">Accept</span></span>|<span data-ttu-id="804a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="804a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="804a0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="804a0-126">Request body</span></span>
<span data-ttu-id="804a0-127">В тексте запроса добавьте представление объекта iosEducationDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="804a0-127">In the request body, supply a JSON representation for the iosEducationDeviceConfiguration object.</span></span>

<span data-ttu-id="804a0-128">В следующей таблице приведены свойства, необходимые при создании iosEducationDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="804a0-128">The following table shows the properties that are required when you create the iosEducationDeviceConfiguration.</span></span>

|<span data-ttu-id="804a0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="804a0-129">Property</span></span>|<span data-ttu-id="804a0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="804a0-130">Type</span></span>|<span data-ttu-id="804a0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="804a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="804a0-132">id</span><span class="sxs-lookup"><span data-stu-id="804a0-132">id</span></span>|<span data-ttu-id="804a0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="804a0-133">String</span></span>|<span data-ttu-id="804a0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="804a0-134">Key of the entity.</span></span> <span data-ttu-id="804a0-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="804a0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="804a0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804a0-137">DateTimeOffset</span></span>|<span data-ttu-id="804a0-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="804a0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="804a0-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="804a0-140">roleScopeTagIds</span></span>|<span data-ttu-id="804a0-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="804a0-141">String collection</span></span>|<span data-ttu-id="804a0-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="804a0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="804a0-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="804a0-144">supportsScopeTags</span></span>|<span data-ttu-id="804a0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="804a0-145">Boolean</span></span>|<span data-ttu-id="804a0-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="804a0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="804a0-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="804a0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="804a0-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="804a0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="804a0-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="804a0-149">This property is read-only.</span></span> <span data-ttu-id="804a0-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="804a0-151">createdDateTime</span></span>|<span data-ttu-id="804a0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804a0-152">DateTimeOffset</span></span>|<span data-ttu-id="804a0-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="804a0-153">DateTime the object was created.</span></span> <span data-ttu-id="804a0-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-155">description</span><span class="sxs-lookup"><span data-stu-id="804a0-155">description</span></span>|<span data-ttu-id="804a0-156">String</span><span class="sxs-lookup"><span data-stu-id="804a0-156">String</span></span>|<span data-ttu-id="804a0-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="804a0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="804a0-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="804a0-159">displayName</span></span>|<span data-ttu-id="804a0-160">String</span><span class="sxs-lookup"><span data-stu-id="804a0-160">String</span></span>|<span data-ttu-id="804a0-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="804a0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="804a0-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="804a0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="804a0-163">version</span><span class="sxs-lookup"><span data-stu-id="804a0-163">version</span></span>|<span data-ttu-id="804a0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="804a0-164">Int32</span></span>|<span data-ttu-id="804a0-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="804a0-165">Version of the device configuration.</span></span> <span data-ttu-id="804a0-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="804a0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="804a0-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="804a0-167">Response</span></span>
<span data-ttu-id="804a0-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="804a0-168">If successful, this method returns a `201 Created` response code and a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="804a0-169">Пример</span><span class="sxs-lookup"><span data-stu-id="804a0-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="804a0-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="804a0-170">Request</span></span>
<span data-ttu-id="804a0-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="804a0-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="804a0-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="804a0-172">Response</span></span>
<span data-ttu-id="804a0-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="804a0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```





