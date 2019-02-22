---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb162edf796b14969eb6ba6efda5c3ea28ec06ce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167237"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="5604b-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5604b-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="5604b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5604b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5604b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5604b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5604b-106">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5604b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5604b-107">Prerequisites</span></span>
<span data-ttu-id="5604b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5604b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5604b-110">Permission type</span></span>|<span data-ttu-id="5604b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5604b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5604b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5604b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5604b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5604b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5604b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5604b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5604b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5604b-115">Not supported.</span></span>|
|<span data-ttu-id="5604b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5604b-116">Application</span></span>|<span data-ttu-id="5604b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5604b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5604b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5604b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5604b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5604b-119">Request headers</span></span>
|<span data-ttu-id="5604b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5604b-120">Header</span></span>|<span data-ttu-id="5604b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5604b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5604b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5604b-122">Authorization</span></span>|<span data-ttu-id="5604b-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5604b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5604b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5604b-124">Accept</span></span>|<span data-ttu-id="5604b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5604b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5604b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5604b-126">Request body</span></span>
<span data-ttu-id="5604b-127">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5604b-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="5604b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5604b-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="5604b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5604b-129">Property</span></span>|<span data-ttu-id="5604b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5604b-130">Type</span></span>|<span data-ttu-id="5604b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5604b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5604b-132">id</span><span class="sxs-lookup"><span data-stu-id="5604b-132">id</span></span>|<span data-ttu-id="5604b-133">String</span><span class="sxs-lookup"><span data-stu-id="5604b-133">String</span></span>|<span data-ttu-id="5604b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5604b-134">Key of the entity.</span></span> <span data-ttu-id="5604b-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5604b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5604b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5604b-137">DateTimeOffset</span></span>|<span data-ttu-id="5604b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5604b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5604b-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5604b-140">roleScopeTagIds</span></span>|<span data-ttu-id="5604b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5604b-141">String collection</span></span>|<span data-ttu-id="5604b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5604b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5604b-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5604b-144">supportsScopeTags</span></span>|<span data-ttu-id="5604b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="5604b-145">Boolean</span></span>|<span data-ttu-id="5604b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5604b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5604b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5604b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5604b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5604b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5604b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5604b-149">This property is read-only.</span></span> <span data-ttu-id="5604b-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5604b-151">createdDateTime</span></span>|<span data-ttu-id="5604b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5604b-152">DateTimeOffset</span></span>|<span data-ttu-id="5604b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5604b-153">DateTime the object was created.</span></span> <span data-ttu-id="5604b-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-155">description</span><span class="sxs-lookup"><span data-stu-id="5604b-155">description</span></span>|<span data-ttu-id="5604b-156">Строка</span><span class="sxs-lookup"><span data-stu-id="5604b-156">String</span></span>|<span data-ttu-id="5604b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5604b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5604b-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5604b-159">displayName</span></span>|<span data-ttu-id="5604b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="5604b-160">String</span></span>|<span data-ttu-id="5604b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5604b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5604b-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5604b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-163">version</span><span class="sxs-lookup"><span data-stu-id="5604b-163">version</span></span>|<span data-ttu-id="5604b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5604b-164">Int32</span></span>|<span data-ttu-id="5604b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5604b-165">Version of the device configuration.</span></span> <span data-ttu-id="5604b-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5604b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5604b-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="5604b-167">payloadName</span></span>|<span data-ttu-id="5604b-168">String</span><span class="sxs-lookup"><span data-stu-id="5604b-168">String</span></span>|<span data-ttu-id="5604b-169">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="5604b-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="5604b-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="5604b-170">payloadFileName</span></span>|<span data-ttu-id="5604b-171">String</span><span class="sxs-lookup"><span data-stu-id="5604b-171">String</span></span>|<span data-ttu-id="5604b-172">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="5604b-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="5604b-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="5604b-173">\*.xml).</span></span>|
|<span data-ttu-id="5604b-174">payload</span><span class="sxs-lookup"><span data-stu-id="5604b-174">payload</span></span>|<span data-ttu-id="5604b-175">Binary</span><span class="sxs-lookup"><span data-stu-id="5604b-175">Binary</span></span>|<span data-ttu-id="5604b-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="5604b-176">Payload.</span></span> <span data-ttu-id="5604b-177">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="5604b-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="5604b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="5604b-178">Response</span></span>
<span data-ttu-id="5604b-179">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5604b-179">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5604b-180">Пример</span><span class="sxs-lookup"><span data-stu-id="5604b-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="5604b-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="5604b-181">Request</span></span>
<span data-ttu-id="5604b-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5604b-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="5604b-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="5604b-183">Response</span></span>
<span data-ttu-id="5604b-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5604b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




