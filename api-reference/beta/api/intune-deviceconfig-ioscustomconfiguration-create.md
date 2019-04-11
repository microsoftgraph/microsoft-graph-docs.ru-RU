---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b19affa1478c2b40526dea48bcf1050659beedb3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805602"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="a3287-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3287-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="a3287-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3287-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3287-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3287-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3287-106">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3287-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3287-107">Prerequisites</span></span>
<span data-ttu-id="a3287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3287-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3287-110">Permission type</span></span>|<span data-ttu-id="a3287-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3287-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3287-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3287-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3287-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3287-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3287-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3287-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3287-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3287-115">Not supported.</span></span>|
|<span data-ttu-id="a3287-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3287-116">Application</span></span>|<span data-ttu-id="a3287-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3287-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3287-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3287-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3287-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3287-119">Request headers</span></span>
|<span data-ttu-id="a3287-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3287-120">Header</span></span>|<span data-ttu-id="a3287-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3287-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3287-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3287-122">Authorization</span></span>|<span data-ttu-id="a3287-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3287-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3287-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3287-124">Accept</span></span>|<span data-ttu-id="a3287-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3287-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3287-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3287-126">Request body</span></span>
<span data-ttu-id="a3287-127">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3287-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="a3287-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a3287-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="a3287-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3287-129">Property</span></span>|<span data-ttu-id="a3287-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a3287-130">Type</span></span>|<span data-ttu-id="a3287-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a3287-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3287-132">id</span><span class="sxs-lookup"><span data-stu-id="a3287-132">id</span></span>|<span data-ttu-id="a3287-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a3287-133">String</span></span>|<span data-ttu-id="a3287-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3287-134">Key of the entity.</span></span> <span data-ttu-id="a3287-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3287-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a3287-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3287-137">DateTimeOffset</span></span>|<span data-ttu-id="a3287-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a3287-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a3287-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3287-140">roleScopeTagIds</span></span>|<span data-ttu-id="a3287-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3287-141">String collection</span></span>|<span data-ttu-id="a3287-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a3287-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a3287-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a3287-144">supportsScopeTags</span></span>|<span data-ttu-id="a3287-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3287-145">Boolean</span></span>|<span data-ttu-id="a3287-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a3287-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a3287-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a3287-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a3287-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a3287-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a3287-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3287-149">This property is read-only.</span></span> <span data-ttu-id="a3287-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3287-151">createdDateTime</span></span>|<span data-ttu-id="a3287-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3287-152">DateTimeOffset</span></span>|<span data-ttu-id="a3287-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a3287-153">DateTime the object was created.</span></span> <span data-ttu-id="a3287-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-155">description</span><span class="sxs-lookup"><span data-stu-id="a3287-155">description</span></span>|<span data-ttu-id="a3287-156">String</span><span class="sxs-lookup"><span data-stu-id="a3287-156">String</span></span>|<span data-ttu-id="a3287-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3287-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3287-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a3287-159">displayName</span></span>|<span data-ttu-id="a3287-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a3287-160">String</span></span>|<span data-ttu-id="a3287-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3287-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3287-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3287-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-163">version</span><span class="sxs-lookup"><span data-stu-id="a3287-163">version</span></span>|<span data-ttu-id="a3287-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a3287-164">Int32</span></span>|<span data-ttu-id="a3287-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3287-165">Version of the device configuration.</span></span> <span data-ttu-id="a3287-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3287-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3287-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="a3287-167">payloadName</span></span>|<span data-ttu-id="a3287-168">String</span><span class="sxs-lookup"><span data-stu-id="a3287-168">String</span></span>|<span data-ttu-id="a3287-169">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="a3287-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a3287-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a3287-170">payloadFileName</span></span>|<span data-ttu-id="a3287-171">String</span><span class="sxs-lookup"><span data-stu-id="a3287-171">String</span></span>|<span data-ttu-id="a3287-172">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a3287-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a3287-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="a3287-173">\*.xml).</span></span>|
|<span data-ttu-id="a3287-174">payload</span><span class="sxs-lookup"><span data-stu-id="a3287-174">payload</span></span>|<span data-ttu-id="a3287-175">Binary</span><span class="sxs-lookup"><span data-stu-id="a3287-175">Binary</span></span>|<span data-ttu-id="a3287-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="a3287-176">Payload.</span></span> <span data-ttu-id="a3287-177">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="a3287-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a3287-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3287-178">Response</span></span>
<span data-ttu-id="a3287-179">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a3287-179">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3287-180">Пример</span><span class="sxs-lookup"><span data-stu-id="a3287-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3287-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3287-181">Request</span></span>
<span data-ttu-id="a3287-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3287-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a3287-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3287-183">Response</span></span>
<span data-ttu-id="a3287-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3287-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





