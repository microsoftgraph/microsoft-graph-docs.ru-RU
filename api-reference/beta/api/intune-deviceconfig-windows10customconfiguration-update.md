---
title: Обновление объекта windows10CustomConfiguration
description: Обновление свойств объекта windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4feaac0afa6b079eeea6a6509d20a0d21b471e6d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777118"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="42f1b-103">Обновление объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="42f1b-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="42f1b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42f1b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42f1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42f1b-106">Обновление свойств объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-106">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42f1b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="42f1b-107">Prerequisites</span></span>
<span data-ttu-id="42f1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42f1b-110">Permission type</span></span>|<span data-ttu-id="42f1b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42f1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42f1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42f1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42f1b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f1b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42f1b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42f1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42f1b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f1b-115">Not supported.</span></span>|
|<span data-ttu-id="42f1b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42f1b-116">Application</span></span>|<span data-ttu-id="42f1b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42f1b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42f1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42f1b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42f1b-119">Request headers</span></span>
|<span data-ttu-id="42f1b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42f1b-120">Header</span></span>|<span data-ttu-id="42f1b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42f1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42f1b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42f1b-122">Authorization</span></span>|<span data-ttu-id="42f1b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42f1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42f1b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42f1b-124">Accept</span></span>|<span data-ttu-id="42f1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42f1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42f1b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42f1b-126">Request body</span></span>
<span data-ttu-id="42f1b-127">В теле запроса добавьте представление объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42f1b-127">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="42f1b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-128">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="42f1b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="42f1b-129">Property</span></span>|<span data-ttu-id="42f1b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42f1b-130">Type</span></span>|<span data-ttu-id="42f1b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42f1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42f1b-132">id</span><span class="sxs-lookup"><span data-stu-id="42f1b-132">id</span></span>|<span data-ttu-id="42f1b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="42f1b-133">String</span></span>|<span data-ttu-id="42f1b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42f1b-134">Key of the entity.</span></span> <span data-ttu-id="42f1b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42f1b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="42f1b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42f1b-137">DateTimeOffset</span></span>|<span data-ttu-id="42f1b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="42f1b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="42f1b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42f1b-140">roleScopeTagIds</span></span>|<span data-ttu-id="42f1b-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="42f1b-141">String collection</span></span>|<span data-ttu-id="42f1b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="42f1b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42f1b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="42f1b-144">supportsScopeTags</span></span>|<span data-ttu-id="42f1b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="42f1b-145">Boolean</span></span>|<span data-ttu-id="42f1b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="42f1b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42f1b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="42f1b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42f1b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="42f1b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42f1b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42f1b-149">This property is read-only.</span></span> <span data-ttu-id="42f1b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42f1b-151">createdDateTime</span></span>|<span data-ttu-id="42f1b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42f1b-152">DateTimeOffset</span></span>|<span data-ttu-id="42f1b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="42f1b-153">DateTime the object was created.</span></span> <span data-ttu-id="42f1b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-155">description</span><span class="sxs-lookup"><span data-stu-id="42f1b-155">description</span></span>|<span data-ttu-id="42f1b-156">String</span><span class="sxs-lookup"><span data-stu-id="42f1b-156">String</span></span>|<span data-ttu-id="42f1b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42f1b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42f1b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="42f1b-159">displayName</span></span>|<span data-ttu-id="42f1b-160">String</span><span class="sxs-lookup"><span data-stu-id="42f1b-160">String</span></span>|<span data-ttu-id="42f1b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42f1b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42f1b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42f1b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-163">version</span><span class="sxs-lookup"><span data-stu-id="42f1b-163">version</span></span>|<span data-ttu-id="42f1b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="42f1b-164">Int32</span></span>|<span data-ttu-id="42f1b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42f1b-165">Version of the device configuration.</span></span> <span data-ttu-id="42f1b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f1b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f1b-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="42f1b-167">omaSettings</span></span>|<span data-ttu-id="42f1b-168">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42f1b-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="42f1b-169">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="42f1b-169">OMA settings.</span></span> <span data-ttu-id="42f1b-170">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="42f1b-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="42f1b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="42f1b-171">Response</span></span>
<span data-ttu-id="42f1b-172">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42f1b-172">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42f1b-173">Пример</span><span class="sxs-lookup"><span data-stu-id="42f1b-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="42f1b-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="42f1b-174">Request</span></span>
<span data-ttu-id="42f1b-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42f1b-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="42f1b-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="42f1b-176">Response</span></span>
<span data-ttu-id="42f1b-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42f1b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```





