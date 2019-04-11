---
title: Обновление Андроидомакпконфигуратион
description: Обновление свойств объекта Андроидомакпконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f8b7bba614056e97081b8a7997a9fbae4e83e74
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772568"
---
# <a name="update-androidomacpconfiguration"></a><span data-ttu-id="1b426-103">Обновление Андроидомакпконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1b426-103">Update androidOmaCpConfiguration</span></span>

> <span data-ttu-id="1b426-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b426-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b426-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b426-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b426-106">Обновление свойств объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1b426-106">Update the properties of a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b426-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b426-107">Prerequisites</span></span>
<span data-ttu-id="1b426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b426-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b426-110">Permission type</span></span>|<span data-ttu-id="1b426-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b426-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b426-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b426-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b426-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b426-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b426-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b426-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b426-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b426-115">Not supported.</span></span>|
|<span data-ttu-id="1b426-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b426-116">Application</span></span>|<span data-ttu-id="1b426-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b426-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b426-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b426-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1b426-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b426-119">Request headers</span></span>
|<span data-ttu-id="1b426-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b426-120">Header</span></span>|<span data-ttu-id="1b426-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b426-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b426-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b426-122">Authorization</span></span>|<span data-ttu-id="1b426-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b426-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b426-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b426-124">Accept</span></span>|<span data-ttu-id="1b426-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b426-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b426-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b426-126">Request body</span></span>
<span data-ttu-id="1b426-127">В тексте запроса добавьте представление объекта [Андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b426-127">In the request body, supply a JSON representation for the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

<span data-ttu-id="1b426-128">В следующей таблице приведены свойства, необходимые при создании [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-128">The following table shows the properties that are required when you create the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span></span>

|<span data-ttu-id="1b426-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b426-129">Property</span></span>|<span data-ttu-id="1b426-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b426-130">Type</span></span>|<span data-ttu-id="1b426-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b426-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b426-132">id</span><span class="sxs-lookup"><span data-stu-id="1b426-132">id</span></span>|<span data-ttu-id="1b426-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1b426-133">String</span></span>|<span data-ttu-id="1b426-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b426-134">Key of the entity.</span></span> <span data-ttu-id="1b426-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b426-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1b426-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b426-137">DateTimeOffset</span></span>|<span data-ttu-id="1b426-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1b426-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1b426-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b426-140">roleScopeTagIds</span></span>|<span data-ttu-id="1b426-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1b426-141">String collection</span></span>|<span data-ttu-id="1b426-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1b426-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1b426-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1b426-144">supportsScopeTags</span></span>|<span data-ttu-id="1b426-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b426-145">Boolean</span></span>|<span data-ttu-id="1b426-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1b426-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1b426-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1b426-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1b426-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1b426-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1b426-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b426-149">This property is read-only.</span></span> <span data-ttu-id="1b426-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b426-151">createdDateTime</span></span>|<span data-ttu-id="1b426-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b426-152">DateTimeOffset</span></span>|<span data-ttu-id="1b426-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1b426-153">DateTime the object was created.</span></span> <span data-ttu-id="1b426-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-155">description</span><span class="sxs-lookup"><span data-stu-id="1b426-155">description</span></span>|<span data-ttu-id="1b426-156">String</span><span class="sxs-lookup"><span data-stu-id="1b426-156">String</span></span>|<span data-ttu-id="1b426-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b426-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b426-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1b426-159">displayName</span></span>|<span data-ttu-id="1b426-160">String</span><span class="sxs-lookup"><span data-stu-id="1b426-160">String</span></span>|<span data-ttu-id="1b426-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b426-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b426-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-163">version</span><span class="sxs-lookup"><span data-stu-id="1b426-163">version</span></span>|<span data-ttu-id="1b426-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1b426-164">Int32</span></span>|<span data-ttu-id="1b426-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b426-165">Version of the device configuration.</span></span> <span data-ttu-id="1b426-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b426-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b426-167">Конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="1b426-167">configurationXml</span></span>|<span data-ttu-id="1b426-168">Binary</span><span class="sxs-lookup"><span data-stu-id="1b426-168">Binary</span></span>|<span data-ttu-id="1b426-169">XML-файл конфигурации, который будет применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="1b426-169">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="1b426-170">При чтении она предоставляет только строку заполнителя, так как исходные данные шифруются и хранятся.</span><span class="sxs-lookup"><span data-stu-id="1b426-170">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="1b426-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b426-171">Response</span></span>
<span data-ttu-id="1b426-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b426-172">If successful, this method returns a `200 OK` response code and an updated [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b426-173">Пример</span><span class="sxs-lookup"><span data-stu-id="1b426-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b426-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b426-174">Request</span></span>
<span data-ttu-id="1b426-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b426-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="1b426-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b426-176">Response</span></span>
<span data-ttu-id="1b426-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b426-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```





