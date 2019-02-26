---
title: Создание объекта androidCustomConfiguration
description: Создание объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1941e67c2f632cd02af7fcc29062c1f102977345
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152978"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="00665-103">Создание объекта androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="00665-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="00665-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00665-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00665-106">Создание объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-106">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00665-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00665-107">Prerequisites</span></span>
<span data-ttu-id="00665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00665-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00665-110">Permission type</span></span>|<span data-ttu-id="00665-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00665-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00665-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00665-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00665-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00665-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00665-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00665-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00665-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00665-115">Not supported.</span></span>|
|<span data-ttu-id="00665-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00665-116">Application</span></span>|<span data-ttu-id="00665-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00665-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00665-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00665-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="00665-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00665-119">Request headers</span></span>
|<span data-ttu-id="00665-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00665-120">Header</span></span>|<span data-ttu-id="00665-121">Значение</span><span class="sxs-lookup"><span data-stu-id="00665-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00665-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00665-122">Authorization</span></span>|<span data-ttu-id="00665-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00665-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00665-124">Accept</span><span class="sxs-lookup"><span data-stu-id="00665-124">Accept</span></span>|<span data-ttu-id="00665-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00665-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00665-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00665-126">Request body</span></span>
<span data-ttu-id="00665-127">В тексте запроса добавьте представление объекта androidCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00665-127">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="00665-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="00665-128">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="00665-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="00665-129">Property</span></span>|<span data-ttu-id="00665-130">Тип</span><span class="sxs-lookup"><span data-stu-id="00665-130">Type</span></span>|<span data-ttu-id="00665-131">Описание</span><span class="sxs-lookup"><span data-stu-id="00665-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00665-132">id</span><span class="sxs-lookup"><span data-stu-id="00665-132">id</span></span>|<span data-ttu-id="00665-133">String</span><span class="sxs-lookup"><span data-stu-id="00665-133">String</span></span>|<span data-ttu-id="00665-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00665-134">Key of the entity.</span></span> <span data-ttu-id="00665-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00665-136">lastModifiedDateTime</span></span>|<span data-ttu-id="00665-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00665-137">DateTimeOffset</span></span>|<span data-ttu-id="00665-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="00665-138">DateTime the object was last modified.</span></span> <span data-ttu-id="00665-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00665-140">roleScopeTagIds</span></span>|<span data-ttu-id="00665-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="00665-141">String collection</span></span>|<span data-ttu-id="00665-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="00665-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00665-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="00665-144">supportsScopeTags</span></span>|<span data-ttu-id="00665-145">Логический</span><span class="sxs-lookup"><span data-stu-id="00665-145">Boolean</span></span>|<span data-ttu-id="00665-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="00665-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00665-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="00665-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00665-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="00665-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00665-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00665-149">This property is read-only.</span></span> <span data-ttu-id="00665-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00665-151">createdDateTime</span></span>|<span data-ttu-id="00665-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00665-152">DateTimeOffset</span></span>|<span data-ttu-id="00665-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="00665-153">DateTime the object was created.</span></span> <span data-ttu-id="00665-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-155">description</span><span class="sxs-lookup"><span data-stu-id="00665-155">description</span></span>|<span data-ttu-id="00665-156">String</span><span class="sxs-lookup"><span data-stu-id="00665-156">String</span></span>|<span data-ttu-id="00665-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00665-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00665-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-159">displayName</span><span class="sxs-lookup"><span data-stu-id="00665-159">displayName</span></span>|<span data-ttu-id="00665-160">String</span><span class="sxs-lookup"><span data-stu-id="00665-160">String</span></span>|<span data-ttu-id="00665-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00665-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00665-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00665-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-163">version</span><span class="sxs-lookup"><span data-stu-id="00665-163">version</span></span>|<span data-ttu-id="00665-164">Int32</span><span class="sxs-lookup"><span data-stu-id="00665-164">Int32</span></span>|<span data-ttu-id="00665-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00665-165">Version of the device configuration.</span></span> <span data-ttu-id="00665-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00665-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00665-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="00665-167">omaSettings</span></span>|<span data-ttu-id="00665-168">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="00665-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="00665-169">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="00665-169">OMA settings.</span></span> <span data-ttu-id="00665-170">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="00665-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="00665-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="00665-171">Response</span></span>
<span data-ttu-id="00665-172">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00665-172">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00665-173">Пример</span><span class="sxs-lookup"><span data-stu-id="00665-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="00665-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="00665-174">Request</span></span>
<span data-ttu-id="00665-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00665-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="00665-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="00665-176">Response</span></span>
<span data-ttu-id="00665-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00665-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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




