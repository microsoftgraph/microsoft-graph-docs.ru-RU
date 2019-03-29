---
title: Обновление объекта macOSCustomConfiguration
description: Обновление свойств объекта macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22710e7e9087eed11065b9dd89a94ccf62a2bbdb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970501"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="f0964-103">Обновление объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0964-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="f0964-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0964-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0964-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0964-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0964-106">Обновление свойств объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-106">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0964-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0964-107">Prerequisites</span></span>
<span data-ttu-id="f0964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0964-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0964-110">Permission type</span></span>|<span data-ttu-id="f0964-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0964-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0964-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0964-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0964-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0964-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0964-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0964-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0964-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0964-115">Not supported.</span></span>|
|<span data-ttu-id="f0964-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0964-116">Application</span></span>|<span data-ttu-id="f0964-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0964-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0964-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0964-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f0964-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0964-119">Request headers</span></span>
|<span data-ttu-id="f0964-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0964-120">Header</span></span>|<span data-ttu-id="f0964-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f0964-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0964-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0964-122">Authorization</span></span>|<span data-ttu-id="f0964-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0964-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0964-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f0964-124">Accept</span></span>|<span data-ttu-id="f0964-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0964-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0964-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0964-126">Request body</span></span>
<span data-ttu-id="f0964-127">В теле запроса добавьте представление объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0964-127">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="f0964-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-128">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="f0964-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0964-129">Property</span></span>|<span data-ttu-id="f0964-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f0964-130">Type</span></span>|<span data-ttu-id="f0964-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f0964-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0964-132">id</span><span class="sxs-lookup"><span data-stu-id="f0964-132">id</span></span>|<span data-ttu-id="f0964-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f0964-133">String</span></span>|<span data-ttu-id="f0964-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0964-134">Key of the entity.</span></span> <span data-ttu-id="f0964-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0964-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f0964-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0964-137">DateTimeOffset</span></span>|<span data-ttu-id="f0964-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f0964-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f0964-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0964-140">roleScopeTagIds</span></span>|<span data-ttu-id="f0964-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f0964-141">String collection</span></span>|<span data-ttu-id="f0964-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f0964-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0964-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f0964-144">supportsScopeTags</span></span>|<span data-ttu-id="f0964-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0964-145">Boolean</span></span>|<span data-ttu-id="f0964-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f0964-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0964-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f0964-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0964-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f0964-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0964-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0964-149">This property is read-only.</span></span> <span data-ttu-id="f0964-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0964-151">createdDateTime</span></span>|<span data-ttu-id="f0964-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0964-152">DateTimeOffset</span></span>|<span data-ttu-id="f0964-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f0964-153">DateTime the object was created.</span></span> <span data-ttu-id="f0964-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-155">description</span><span class="sxs-lookup"><span data-stu-id="f0964-155">description</span></span>|<span data-ttu-id="f0964-156">String</span><span class="sxs-lookup"><span data-stu-id="f0964-156">String</span></span>|<span data-ttu-id="f0964-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0964-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0964-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f0964-159">displayName</span></span>|<span data-ttu-id="f0964-160">Строка</span><span class="sxs-lookup"><span data-stu-id="f0964-160">String</span></span>|<span data-ttu-id="f0964-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0964-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0964-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0964-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-163">version</span><span class="sxs-lookup"><span data-stu-id="f0964-163">version</span></span>|<span data-ttu-id="f0964-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f0964-164">Int32</span></span>|<span data-ttu-id="f0964-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0964-165">Version of the device configuration.</span></span> <span data-ttu-id="f0964-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0964-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0964-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="f0964-167">payloadName</span></span>|<span data-ttu-id="f0964-168">String</span><span class="sxs-lookup"><span data-stu-id="f0964-168">String</span></span>|<span data-ttu-id="f0964-169">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="f0964-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="f0964-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="f0964-170">payloadFileName</span></span>|<span data-ttu-id="f0964-171">String</span><span class="sxs-lookup"><span data-stu-id="f0964-171">String</span></span>|<span data-ttu-id="f0964-172">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="f0964-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="f0964-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="f0964-173">\*.xml).</span></span>|
|<span data-ttu-id="f0964-174">payload</span><span class="sxs-lookup"><span data-stu-id="f0964-174">payload</span></span>|<span data-ttu-id="f0964-175">Binary</span><span class="sxs-lookup"><span data-stu-id="f0964-175">Binary</span></span>|<span data-ttu-id="f0964-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="f0964-176">Payload.</span></span> <span data-ttu-id="f0964-177">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="f0964-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="f0964-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0964-178">Response</span></span>
<span data-ttu-id="f0964-179">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0964-179">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0964-180">Пример</span><span class="sxs-lookup"><span data-stu-id="f0964-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0964-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0964-181">Request</span></span>
<span data-ttu-id="f0964-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0964-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="f0964-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0964-183">Response</span></span>
<span data-ttu-id="f0964-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0964-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 545

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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




