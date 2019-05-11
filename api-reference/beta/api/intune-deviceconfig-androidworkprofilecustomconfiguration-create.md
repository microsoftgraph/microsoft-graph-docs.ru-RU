---
title: Создание Андроидворкпрофилекустомконфигуратион
description: Создание нового объекта Андроидворкпрофилекустомконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73bca18f8a8d91f3dd0f78827deab25abae5c5c2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928640"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="14885-103">Создание Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="14885-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="14885-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14885-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14885-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14885-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14885-106">Создание нового объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="14885-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14885-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14885-107">Prerequisites</span></span>
<span data-ttu-id="14885-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14885-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14885-110">Permission type</span></span>|<span data-ttu-id="14885-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14885-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14885-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14885-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14885-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14885-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14885-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14885-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14885-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14885-115">Not supported.</span></span>|
|<span data-ttu-id="14885-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14885-116">Application</span></span>|<span data-ttu-id="14885-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14885-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14885-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14885-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="14885-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14885-119">Request headers</span></span>
|<span data-ttu-id="14885-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14885-120">Header</span></span>|<span data-ttu-id="14885-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14885-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14885-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14885-122">Authorization</span></span>|<span data-ttu-id="14885-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14885-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14885-124">Accept</span><span class="sxs-lookup"><span data-stu-id="14885-124">Accept</span></span>|<span data-ttu-id="14885-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14885-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14885-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14885-126">Request body</span></span>
<span data-ttu-id="14885-127">В тексте запроса добавьте представление объекта Андроидворкпрофилекустомконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14885-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="14885-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилекустомконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="14885-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="14885-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14885-129">Property</span></span>|<span data-ttu-id="14885-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14885-130">Type</span></span>|<span data-ttu-id="14885-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14885-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14885-132">id</span><span class="sxs-lookup"><span data-stu-id="14885-132">id</span></span>|<span data-ttu-id="14885-133">String</span><span class="sxs-lookup"><span data-stu-id="14885-133">String</span></span>|<span data-ttu-id="14885-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14885-134">Key of the entity.</span></span> <span data-ttu-id="14885-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14885-136">lastModifiedDateTime</span></span>|<span data-ttu-id="14885-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14885-137">DateTimeOffset</span></span>|<span data-ttu-id="14885-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="14885-138">DateTime the object was last modified.</span></span> <span data-ttu-id="14885-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14885-140">roleScopeTagIds</span></span>|<span data-ttu-id="14885-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="14885-141">String collection</span></span>|<span data-ttu-id="14885-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="14885-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="14885-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="14885-144">supportsScopeTags</span></span>|<span data-ttu-id="14885-145">Логический</span><span class="sxs-lookup"><span data-stu-id="14885-145">Boolean</span></span>|<span data-ttu-id="14885-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="14885-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="14885-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="14885-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="14885-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="14885-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="14885-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14885-149">This property is read-only.</span></span> <span data-ttu-id="14885-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14885-151">createdDateTime</span></span>|<span data-ttu-id="14885-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14885-152">DateTimeOffset</span></span>|<span data-ttu-id="14885-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="14885-153">DateTime the object was created.</span></span> <span data-ttu-id="14885-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-155">description</span><span class="sxs-lookup"><span data-stu-id="14885-155">description</span></span>|<span data-ttu-id="14885-156">String</span><span class="sxs-lookup"><span data-stu-id="14885-156">String</span></span>|<span data-ttu-id="14885-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14885-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14885-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-159">displayName</span><span class="sxs-lookup"><span data-stu-id="14885-159">displayName</span></span>|<span data-ttu-id="14885-160">Строка</span><span class="sxs-lookup"><span data-stu-id="14885-160">String</span></span>|<span data-ttu-id="14885-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14885-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14885-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14885-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-163">version</span><span class="sxs-lookup"><span data-stu-id="14885-163">version</span></span>|<span data-ttu-id="14885-164">Int32</span><span class="sxs-lookup"><span data-stu-id="14885-164">Int32</span></span>|<span data-ttu-id="14885-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14885-165">Version of the device configuration.</span></span> <span data-ttu-id="14885-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14885-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14885-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="14885-167">omaSettings</span></span>|<span data-ttu-id="14885-168">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="14885-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="14885-169">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="14885-169">OMA settings.</span></span> <span data-ttu-id="14885-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14885-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="14885-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="14885-171">Response</span></span>
<span data-ttu-id="14885-172">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14885-172">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14885-173">Пример</span><span class="sxs-lookup"><span data-stu-id="14885-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="14885-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="14885-174">Request</span></span>
<span data-ttu-id="14885-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14885-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="14885-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="14885-176">Response</span></span>
<span data-ttu-id="14885-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14885-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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




