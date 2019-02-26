---
title: Обновление Андроидфорворккустомконфигуратион
description: Обновление свойств объекта Андроидфорворккустомконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e0c28db69f4418bf2984cd3fd11f08022e080ba
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157577"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="fd1b6-103">Обновление Андроидфорворккустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="fd1b6-103">Update androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="fd1b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd1b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd1b6-106">Обновление свойств объекта [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fd1b6-106">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd1b6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fd1b6-107">Prerequisites</span></span>
<span data-ttu-id="fd1b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd1b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd1b6-110">Permission type</span></span>|<span data-ttu-id="fd1b6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd1b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd1b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd1b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd1b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd1b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd1b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd1b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd1b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-115">Not supported.</span></span>|
|<span data-ttu-id="fd1b6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd1b6-116">Application</span></span>|<span data-ttu-id="fd1b6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd1b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd1b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fd1b6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd1b6-119">Request headers</span></span>
|<span data-ttu-id="fd1b6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd1b6-120">Header</span></span>|<span data-ttu-id="fd1b6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fd1b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd1b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd1b6-122">Authorization</span></span>|<span data-ttu-id="fd1b6-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd1b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd1b6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fd1b6-124">Accept</span></span>|<span data-ttu-id="fd1b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd1b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd1b6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd1b6-126">Request body</span></span>
<span data-ttu-id="fd1b6-127">В тексте запроса добавьте представление объекта [Андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-127">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="fd1b6-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-128">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="fd1b6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd1b6-129">Property</span></span>|<span data-ttu-id="fd1b6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fd1b6-130">Type</span></span>|<span data-ttu-id="fd1b6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fd1b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd1b6-132">id</span><span class="sxs-lookup"><span data-stu-id="fd1b6-132">id</span></span>|<span data-ttu-id="fd1b6-133">String</span><span class="sxs-lookup"><span data-stu-id="fd1b6-133">String</span></span>|<span data-ttu-id="fd1b6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-134">Key of the entity.</span></span> <span data-ttu-id="fd1b6-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd1b6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fd1b6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd1b6-137">DateTimeOffset</span></span>|<span data-ttu-id="fd1b6-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fd1b6-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd1b6-140">roleScopeTagIds</span></span>|<span data-ttu-id="fd1b6-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fd1b6-141">String collection</span></span>|<span data-ttu-id="fd1b6-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fd1b6-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fd1b6-144">supportsScopeTags</span></span>|<span data-ttu-id="fd1b6-145">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1b6-145">Boolean</span></span>|<span data-ttu-id="fd1b6-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fd1b6-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fd1b6-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fd1b6-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-149">This property is read-only.</span></span> <span data-ttu-id="fd1b6-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd1b6-151">createdDateTime</span></span>|<span data-ttu-id="fd1b6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd1b6-152">DateTimeOffset</span></span>|<span data-ttu-id="fd1b6-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-153">DateTime the object was created.</span></span> <span data-ttu-id="fd1b6-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-155">description</span><span class="sxs-lookup"><span data-stu-id="fd1b6-155">description</span></span>|<span data-ttu-id="fd1b6-156">String</span><span class="sxs-lookup"><span data-stu-id="fd1b6-156">String</span></span>|<span data-ttu-id="fd1b6-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fd1b6-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fd1b6-159">displayName</span></span>|<span data-ttu-id="fd1b6-160">String</span><span class="sxs-lookup"><span data-stu-id="fd1b6-160">String</span></span>|<span data-ttu-id="fd1b6-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fd1b6-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd1b6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-163">version</span><span class="sxs-lookup"><span data-stu-id="fd1b6-163">version</span></span>|<span data-ttu-id="fd1b6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1b6-164">Int32</span></span>|<span data-ttu-id="fd1b6-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-165">Version of the device configuration.</span></span> <span data-ttu-id="fd1b6-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd1b6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd1b6-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="fd1b6-167">omaSettings</span></span>|<span data-ttu-id="fd1b6-168">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd1b6-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="fd1b6-169">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-169">OMA settings.</span></span> <span data-ttu-id="fd1b6-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fd1b6-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd1b6-171">Response</span></span>
<span data-ttu-id="fd1b6-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-172">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd1b6-173">Пример</span><span class="sxs-lookup"><span data-stu-id="fd1b6-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd1b6-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd1b6-174">Request</span></span>
<span data-ttu-id="fd1b6-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="fd1b6-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd1b6-176">Response</span></span>
<span data-ttu-id="fd1b6-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd1b6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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




