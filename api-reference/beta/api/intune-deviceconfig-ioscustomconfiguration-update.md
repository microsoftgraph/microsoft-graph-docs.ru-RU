---
title: Обновление объекта iosCustomConfiguration
description: Обновление свойств объекта iosCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8262bee3e0b86d76f14054283471d7eaabc1322
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923730"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="69900-103">Обновление объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="69900-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="69900-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69900-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69900-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69900-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69900-106">Обновление свойств объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-106">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69900-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69900-107">Prerequisites</span></span>
<span data-ttu-id="69900-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69900-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69900-110">Permission type</span></span>|<span data-ttu-id="69900-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69900-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69900-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69900-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69900-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69900-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69900-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69900-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69900-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69900-115">Not supported.</span></span>|
|<span data-ttu-id="69900-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69900-116">Application</span></span>|<span data-ttu-id="69900-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69900-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69900-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69900-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="69900-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69900-119">Request headers</span></span>
|<span data-ttu-id="69900-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69900-120">Header</span></span>|<span data-ttu-id="69900-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69900-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69900-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69900-122">Authorization</span></span>|<span data-ttu-id="69900-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69900-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69900-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69900-124">Accept</span></span>|<span data-ttu-id="69900-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69900-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69900-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69900-126">Request body</span></span>
<span data-ttu-id="69900-127">В теле запроса добавьте представление объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69900-127">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="69900-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-128">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="69900-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69900-129">Property</span></span>|<span data-ttu-id="69900-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69900-130">Type</span></span>|<span data-ttu-id="69900-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69900-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69900-132">id</span><span class="sxs-lookup"><span data-stu-id="69900-132">id</span></span>|<span data-ttu-id="69900-133">Строка</span><span class="sxs-lookup"><span data-stu-id="69900-133">String</span></span>|<span data-ttu-id="69900-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="69900-134">Key of the entity.</span></span> <span data-ttu-id="69900-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69900-136">lastModifiedDateTime</span></span>|<span data-ttu-id="69900-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69900-137">DateTimeOffset</span></span>|<span data-ttu-id="69900-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="69900-138">DateTime the object was last modified.</span></span> <span data-ttu-id="69900-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="69900-140">roleScopeTagIds</span></span>|<span data-ttu-id="69900-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="69900-141">String collection</span></span>|<span data-ttu-id="69900-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="69900-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="69900-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="69900-144">supportsScopeTags</span></span>|<span data-ttu-id="69900-145">Логический</span><span class="sxs-lookup"><span data-stu-id="69900-145">Boolean</span></span>|<span data-ttu-id="69900-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="69900-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="69900-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="69900-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="69900-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="69900-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="69900-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69900-149">This property is read-only.</span></span> <span data-ttu-id="69900-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69900-151">createdDateTime</span></span>|<span data-ttu-id="69900-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69900-152">DateTimeOffset</span></span>|<span data-ttu-id="69900-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="69900-153">DateTime the object was created.</span></span> <span data-ttu-id="69900-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-155">description</span><span class="sxs-lookup"><span data-stu-id="69900-155">description</span></span>|<span data-ttu-id="69900-156">String</span><span class="sxs-lookup"><span data-stu-id="69900-156">String</span></span>|<span data-ttu-id="69900-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69900-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69900-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-159">displayName</span><span class="sxs-lookup"><span data-stu-id="69900-159">displayName</span></span>|<span data-ttu-id="69900-160">Строка</span><span class="sxs-lookup"><span data-stu-id="69900-160">String</span></span>|<span data-ttu-id="69900-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69900-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69900-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="69900-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-163">version</span><span class="sxs-lookup"><span data-stu-id="69900-163">version</span></span>|<span data-ttu-id="69900-164">Int32</span><span class="sxs-lookup"><span data-stu-id="69900-164">Int32</span></span>|<span data-ttu-id="69900-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69900-165">Version of the device configuration.</span></span> <span data-ttu-id="69900-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69900-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69900-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="69900-167">payloadName</span></span>|<span data-ttu-id="69900-168">Строка</span><span class="sxs-lookup"><span data-stu-id="69900-168">String</span></span>|<span data-ttu-id="69900-169">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="69900-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="69900-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="69900-170">payloadFileName</span></span>|<span data-ttu-id="69900-171">String</span><span class="sxs-lookup"><span data-stu-id="69900-171">String</span></span>|<span data-ttu-id="69900-172">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="69900-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="69900-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="69900-173">\*.xml).</span></span>|
|<span data-ttu-id="69900-174">payload</span><span class="sxs-lookup"><span data-stu-id="69900-174">payload</span></span>|<span data-ttu-id="69900-175">Binary</span><span class="sxs-lookup"><span data-stu-id="69900-175">Binary</span></span>|<span data-ttu-id="69900-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="69900-176">Payload.</span></span> <span data-ttu-id="69900-177">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="69900-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="69900-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="69900-178">Response</span></span>
<span data-ttu-id="69900-179">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="69900-179">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69900-180">Пример</span><span class="sxs-lookup"><span data-stu-id="69900-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="69900-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="69900-181">Request</span></span>
<span data-ttu-id="69900-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69900-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="69900-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="69900-183">Response</span></span>
<span data-ttu-id="69900-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69900-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




