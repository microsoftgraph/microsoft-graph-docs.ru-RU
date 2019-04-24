---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b19affa1478c2b40526dea48bcf1050659beedb3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467591"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="bacbf-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="bacbf-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="bacbf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bacbf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bacbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bacbf-106">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bacbf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bacbf-107">Prerequisites</span></span>
<span data-ttu-id="bacbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bacbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bacbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bacbf-110">Permission type</span></span>|<span data-ttu-id="bacbf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bacbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bacbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bacbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bacbf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacbf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bacbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bacbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bacbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacbf-115">Not supported.</span></span>|
|<span data-ttu-id="bacbf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bacbf-116">Application</span></span>|<span data-ttu-id="bacbf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bacbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bacbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bacbf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bacbf-119">Request headers</span></span>
|<span data-ttu-id="bacbf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bacbf-120">Header</span></span>|<span data-ttu-id="bacbf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bacbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bacbf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bacbf-122">Authorization</span></span>|<span data-ttu-id="bacbf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bacbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bacbf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bacbf-124">Accept</span></span>|<span data-ttu-id="bacbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bacbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bacbf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bacbf-126">Request body</span></span>
<span data-ttu-id="bacbf-127">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bacbf-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="bacbf-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bacbf-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="bacbf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bacbf-129">Property</span></span>|<span data-ttu-id="bacbf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bacbf-130">Type</span></span>|<span data-ttu-id="bacbf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bacbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bacbf-132">id</span><span class="sxs-lookup"><span data-stu-id="bacbf-132">id</span></span>|<span data-ttu-id="bacbf-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bacbf-133">String</span></span>|<span data-ttu-id="bacbf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bacbf-134">Key of the entity.</span></span> <span data-ttu-id="bacbf-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bacbf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bacbf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacbf-137">DateTimeOffset</span></span>|<span data-ttu-id="bacbf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bacbf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bacbf-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bacbf-140">roleScopeTagIds</span></span>|<span data-ttu-id="bacbf-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bacbf-141">String collection</span></span>|<span data-ttu-id="bacbf-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bacbf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bacbf-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bacbf-144">supportsScopeTags</span></span>|<span data-ttu-id="bacbf-145">Логический</span><span class="sxs-lookup"><span data-stu-id="bacbf-145">Boolean</span></span>|<span data-ttu-id="bacbf-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bacbf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bacbf-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bacbf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bacbf-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bacbf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bacbf-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bacbf-149">This property is read-only.</span></span> <span data-ttu-id="bacbf-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bacbf-151">createdDateTime</span></span>|<span data-ttu-id="bacbf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacbf-152">DateTimeOffset</span></span>|<span data-ttu-id="bacbf-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bacbf-153">DateTime the object was created.</span></span> <span data-ttu-id="bacbf-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-155">description</span><span class="sxs-lookup"><span data-stu-id="bacbf-155">description</span></span>|<span data-ttu-id="bacbf-156">String</span><span class="sxs-lookup"><span data-stu-id="bacbf-156">String</span></span>|<span data-ttu-id="bacbf-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bacbf-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bacbf-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bacbf-159">displayName</span></span>|<span data-ttu-id="bacbf-160">Строка</span><span class="sxs-lookup"><span data-stu-id="bacbf-160">String</span></span>|<span data-ttu-id="bacbf-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bacbf-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bacbf-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bacbf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-163">version</span><span class="sxs-lookup"><span data-stu-id="bacbf-163">version</span></span>|<span data-ttu-id="bacbf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bacbf-164">Int32</span></span>|<span data-ttu-id="bacbf-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bacbf-165">Version of the device configuration.</span></span> <span data-ttu-id="bacbf-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bacbf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bacbf-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="bacbf-167">payloadName</span></span>|<span data-ttu-id="bacbf-168">String</span><span class="sxs-lookup"><span data-stu-id="bacbf-168">String</span></span>|<span data-ttu-id="bacbf-169">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="bacbf-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="bacbf-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="bacbf-170">payloadFileName</span></span>|<span data-ttu-id="bacbf-171">String</span><span class="sxs-lookup"><span data-stu-id="bacbf-171">String</span></span>|<span data-ttu-id="bacbf-172">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="bacbf-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="bacbf-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="bacbf-173">\*.xml).</span></span>|
|<span data-ttu-id="bacbf-174">payload</span><span class="sxs-lookup"><span data-stu-id="bacbf-174">payload</span></span>|<span data-ttu-id="bacbf-175">Binary</span><span class="sxs-lookup"><span data-stu-id="bacbf-175">Binary</span></span>|<span data-ttu-id="bacbf-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="bacbf-176">Payload.</span></span> <span data-ttu-id="bacbf-177">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="bacbf-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="bacbf-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="bacbf-178">Response</span></span>
<span data-ttu-id="bacbf-179">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bacbf-179">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bacbf-180">Пример</span><span class="sxs-lookup"><span data-stu-id="bacbf-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="bacbf-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="bacbf-181">Request</span></span>
<span data-ttu-id="bacbf-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bacbf-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bacbf-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="bacbf-183">Response</span></span>
<span data-ttu-id="bacbf-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bacbf-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





