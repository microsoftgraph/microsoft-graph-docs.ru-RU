---
title: Создание Унсуппортеддевицеконфигуратион
description: Создание нового объекта Унсуппортеддевицеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db43b8dd74d354d87885b8acc5bdfb746a16978e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921963"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="e5ce5-103">Создание Унсуппортеддевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e5ce5-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="e5ce5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5ce5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5ce5-106">Создание нового объекта [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e5ce5-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5ce5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5ce5-107">Prerequisites</span></span>
<span data-ttu-id="e5ce5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5ce5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ce5-110">Permission type</span></span>|<span data-ttu-id="e5ce5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5ce5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5ce5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ce5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5ce5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5ce5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-115">Not supported.</span></span>|
|<span data-ttu-id="e5ce5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5ce5-116">Application</span></span>|<span data-ttu-id="e5ce5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5ce5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5ce5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e5ce5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5ce5-119">Request headers</span></span>
|<span data-ttu-id="e5ce5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5ce5-120">Header</span></span>|<span data-ttu-id="e5ce5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5ce5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5ce5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5ce5-122">Authorization</span></span>|<span data-ttu-id="e5ce5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5ce5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5ce5-124">Accept</span></span>|<span data-ttu-id="e5ce5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5ce5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5ce5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5ce5-126">Request body</span></span>
<span data-ttu-id="e5ce5-127">В тексте запроса добавьте представление объекта Унсуппортеддевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="e5ce5-128">В следующей таблице приведены свойства, необходимые при создании Унсуппортеддевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="e5ce5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5ce5-129">Property</span></span>|<span data-ttu-id="e5ce5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5ce5-130">Type</span></span>|<span data-ttu-id="e5ce5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5ce5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5ce5-132">id</span><span class="sxs-lookup"><span data-stu-id="e5ce5-132">id</span></span>|<span data-ttu-id="e5ce5-133">String</span><span class="sxs-lookup"><span data-stu-id="e5ce5-133">String</span></span>|<span data-ttu-id="e5ce5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-134">Key of the entity.</span></span> <span data-ttu-id="e5ce5-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5ce5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e5ce5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5ce5-137">DateTimeOffset</span></span>|<span data-ttu-id="e5ce5-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e5ce5-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5ce5-140">roleScopeTagIds</span></span>|<span data-ttu-id="e5ce5-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e5ce5-141">String collection</span></span>|<span data-ttu-id="e5ce5-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5ce5-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e5ce5-144">supportsScopeTags</span></span>|<span data-ttu-id="e5ce5-145">Логический</span><span class="sxs-lookup"><span data-stu-id="e5ce5-145">Boolean</span></span>|<span data-ttu-id="e5ce5-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e5ce5-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e5ce5-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e5ce5-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-149">This property is read-only.</span></span> <span data-ttu-id="e5ce5-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5ce5-151">createdDateTime</span></span>|<span data-ttu-id="e5ce5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5ce5-152">DateTimeOffset</span></span>|<span data-ttu-id="e5ce5-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-153">DateTime the object was created.</span></span> <span data-ttu-id="e5ce5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-155">description</span><span class="sxs-lookup"><span data-stu-id="e5ce5-155">description</span></span>|<span data-ttu-id="e5ce5-156">String</span><span class="sxs-lookup"><span data-stu-id="e5ce5-156">String</span></span>|<span data-ttu-id="e5ce5-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5ce5-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e5ce5-159">displayName</span></span>|<span data-ttu-id="e5ce5-160">Строка</span><span class="sxs-lookup"><span data-stu-id="e5ce5-160">String</span></span>|<span data-ttu-id="e5ce5-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5ce5-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-163">version</span><span class="sxs-lookup"><span data-stu-id="e5ce5-163">version</span></span>|<span data-ttu-id="e5ce5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ce5-164">Int32</span></span>|<span data-ttu-id="e5ce5-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-165">Version of the device configuration.</span></span> <span data-ttu-id="e5ce5-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5ce5-167">Оригиналентититипенаме</span><span class="sxs-lookup"><span data-stu-id="e5ce5-167">originalEntityTypeName</span></span>|<span data-ttu-id="e5ce5-168">Строка</span><span class="sxs-lookup"><span data-stu-id="e5ce5-168">String</span></span>|<span data-ttu-id="e5ce5-169">Тип сущности, возвращаемой в противном случае.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="e5ce5-170">details</span><span class="sxs-lookup"><span data-stu-id="e5ce5-170">details</span></span>|<span data-ttu-id="e5ce5-171">Коллекция [унсуппортеддевицеконфигуратиондетаил](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="e5ce5-172">Сведения о том, почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="e5ce5-173">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e5ce5-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5ce5-174">Response</span></span>
<span data-ttu-id="e5ce5-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-175">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5ce5-176">Пример</span><span class="sxs-lookup"><span data-stu-id="e5ce5-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5ce5-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5ce5-177">Request</span></span>
<span data-ttu-id="e5ce5-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e5ce5-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5ce5-179">Response</span></span>
<span data-ttu-id="e5ce5-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 690

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```




