---
title: Создание объекта windows10EnterpriseModernAppManagementConfiguration
description: Создание объекта windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44bfa095bf9178866c25dcab2d285968226a8bbb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793842"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="346c8-103">Создание объекта windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="346c8-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="346c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="346c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="346c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="346c8-106">Создание объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="346c8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="346c8-107">Prerequisites</span></span>
<span data-ttu-id="346c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="346c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="346c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="346c8-110">Permission type</span></span>|<span data-ttu-id="346c8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="346c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="346c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="346c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="346c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="346c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="346c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="346c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346c8-115">Not supported.</span></span>|
|<span data-ttu-id="346c8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="346c8-116">Application</span></span>|<span data-ttu-id="346c8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="346c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="346c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="346c8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="346c8-119">Request headers</span></span>
|<span data-ttu-id="346c8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="346c8-120">Header</span></span>|<span data-ttu-id="346c8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="346c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="346c8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="346c8-122">Authorization</span></span>|<span data-ttu-id="346c8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="346c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="346c8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="346c8-124">Accept</span></span>|<span data-ttu-id="346c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="346c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="346c8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="346c8-126">Request body</span></span>
<span data-ttu-id="346c8-127">В теле запроса добавьте представление объекта windows10EnterpriseModernAppManagementConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="346c8-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="346c8-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="346c8-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="346c8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="346c8-129">Property</span></span>|<span data-ttu-id="346c8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="346c8-130">Type</span></span>|<span data-ttu-id="346c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="346c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346c8-132">id</span><span class="sxs-lookup"><span data-stu-id="346c8-132">id</span></span>|<span data-ttu-id="346c8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="346c8-133">String</span></span>|<span data-ttu-id="346c8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="346c8-134">Key of the entity.</span></span> <span data-ttu-id="346c8-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="346c8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="346c8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346c8-137">DateTimeOffset</span></span>|<span data-ttu-id="346c8-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="346c8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="346c8-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="346c8-140">roleScopeTagIds</span></span>|<span data-ttu-id="346c8-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="346c8-141">String collection</span></span>|<span data-ttu-id="346c8-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="346c8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="346c8-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="346c8-144">supportsScopeTags</span></span>|<span data-ttu-id="346c8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="346c8-145">Boolean</span></span>|<span data-ttu-id="346c8-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="346c8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="346c8-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="346c8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="346c8-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="346c8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="346c8-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346c8-149">This property is read-only.</span></span> <span data-ttu-id="346c8-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="346c8-151">createdDateTime</span></span>|<span data-ttu-id="346c8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346c8-152">DateTimeOffset</span></span>|<span data-ttu-id="346c8-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="346c8-153">DateTime the object was created.</span></span> <span data-ttu-id="346c8-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-155">description</span><span class="sxs-lookup"><span data-stu-id="346c8-155">description</span></span>|<span data-ttu-id="346c8-156">String</span><span class="sxs-lookup"><span data-stu-id="346c8-156">String</span></span>|<span data-ttu-id="346c8-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="346c8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="346c8-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="346c8-159">displayName</span></span>|<span data-ttu-id="346c8-160">String</span><span class="sxs-lookup"><span data-stu-id="346c8-160">String</span></span>|<span data-ttu-id="346c8-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="346c8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="346c8-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="346c8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-163">version</span><span class="sxs-lookup"><span data-stu-id="346c8-163">version</span></span>|<span data-ttu-id="346c8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="346c8-164">Int32</span></span>|<span data-ttu-id="346c8-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="346c8-165">Version of the device configuration.</span></span> <span data-ttu-id="346c8-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="346c8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="346c8-167">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="346c8-167">uninstallBuiltInApps</span></span>|<span data-ttu-id="346c8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="346c8-168">Boolean</span></span>|<span data-ttu-id="346c8-169">Указывает, следует ли удалить фиксированный список встроенных приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="346c8-169">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="346c8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="346c8-170">Response</span></span>
<span data-ttu-id="346c8-171">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="346c8-171">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="346c8-172">Пример</span><span class="sxs-lookup"><span data-stu-id="346c8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="346c8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="346c8-173">Request</span></span>
<span data-ttu-id="346c8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="346c8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="346c8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="346c8-175">Response</span></span>
<span data-ttu-id="346c8-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="346c8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```





