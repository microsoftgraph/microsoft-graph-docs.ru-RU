---
title: Обновление Макосекстенсионсконфигуратион
description: Обновление свойств объекта Макосекстенсионсконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d8e53b83aefee8debcbe0e06f20dd4233a74171
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518606"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="82336-103">Обновление Макосекстенсионсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="82336-103">Update macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="82336-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82336-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82336-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82336-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82336-106">Обновление свойств объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82336-106">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82336-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82336-107">Prerequisites</span></span>
<span data-ttu-id="82336-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82336-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82336-110">Permission type</span></span>|<span data-ttu-id="82336-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82336-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82336-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82336-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82336-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82336-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82336-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82336-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82336-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82336-115">Not supported.</span></span>|
|<span data-ttu-id="82336-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82336-116">Application</span></span>|<span data-ttu-id="82336-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82336-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82336-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82336-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82336-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82336-119">Request headers</span></span>
|<span data-ttu-id="82336-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82336-120">Header</span></span>|<span data-ttu-id="82336-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82336-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82336-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82336-122">Authorization</span></span>|<span data-ttu-id="82336-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82336-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82336-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82336-124">Accept</span></span>|<span data-ttu-id="82336-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82336-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82336-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82336-126">Request body</span></span>
<span data-ttu-id="82336-127">В тексте запроса добавьте представление объекта [Макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82336-127">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="82336-128">В следующей таблице приведены свойства, необходимые при создании [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-128">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="82336-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82336-129">Property</span></span>|<span data-ttu-id="82336-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82336-130">Type</span></span>|<span data-ttu-id="82336-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82336-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82336-132">id</span><span class="sxs-lookup"><span data-stu-id="82336-132">id</span></span>|<span data-ttu-id="82336-133">Строка</span><span class="sxs-lookup"><span data-stu-id="82336-133">String</span></span>|<span data-ttu-id="82336-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82336-134">Key of the entity.</span></span> <span data-ttu-id="82336-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82336-136">lastModifiedDateTime</span></span>|<span data-ttu-id="82336-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82336-137">DateTimeOffset</span></span>|<span data-ttu-id="82336-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82336-138">DateTime the object was last modified.</span></span> <span data-ttu-id="82336-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82336-140">roleScopeTagIds</span></span>|<span data-ttu-id="82336-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="82336-141">String collection</span></span>|<span data-ttu-id="82336-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="82336-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82336-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="82336-144">supportsScopeTags</span></span>|<span data-ttu-id="82336-145">Логический</span><span class="sxs-lookup"><span data-stu-id="82336-145">Boolean</span></span>|<span data-ttu-id="82336-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="82336-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82336-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="82336-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82336-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="82336-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82336-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82336-149">This property is read-only.</span></span> <span data-ttu-id="82336-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82336-151">createdDateTime</span></span>|<span data-ttu-id="82336-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82336-152">DateTimeOffset</span></span>|<span data-ttu-id="82336-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="82336-153">DateTime the object was created.</span></span> <span data-ttu-id="82336-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-155">description</span><span class="sxs-lookup"><span data-stu-id="82336-155">description</span></span>|<span data-ttu-id="82336-156">String</span><span class="sxs-lookup"><span data-stu-id="82336-156">String</span></span>|<span data-ttu-id="82336-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82336-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82336-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-159">displayName</span><span class="sxs-lookup"><span data-stu-id="82336-159">displayName</span></span>|<span data-ttu-id="82336-160">String</span><span class="sxs-lookup"><span data-stu-id="82336-160">String</span></span>|<span data-ttu-id="82336-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82336-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82336-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-163">version</span><span class="sxs-lookup"><span data-stu-id="82336-163">version</span></span>|<span data-ttu-id="82336-164">Int32</span><span class="sxs-lookup"><span data-stu-id="82336-164">Int32</span></span>|<span data-ttu-id="82336-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82336-165">Version of the device configuration.</span></span> <span data-ttu-id="82336-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82336-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82336-167">Кернелекстенсионоверридесалловед</span><span class="sxs-lookup"><span data-stu-id="82336-167">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="82336-168">Логический</span><span class="sxs-lookup"><span data-stu-id="82336-168">Boolean</span></span>|<span data-ttu-id="82336-169">Если задано значение true, пользователи могут утверждать дополнительные расширения ядра, не разрешенные профилями конфигураций.</span><span class="sxs-lookup"><span data-stu-id="82336-169">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="82336-170">Кернелекстенсионалловедтеамидентифиерс</span><span class="sxs-lookup"><span data-stu-id="82336-170">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="82336-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="82336-171">String collection</span></span>|<span data-ttu-id="82336-172">Все расширения ядра, подписанные с помощью идентификаторов команд в этом списке, могут быть загружены.</span><span class="sxs-lookup"><span data-stu-id="82336-172">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="82336-173">Кернелекстенсионсалловед</span><span class="sxs-lookup"><span data-stu-id="82336-173">kernelExtensionsAllowed</span></span>|<span data-ttu-id="82336-174">Коллекция [макоскернелекстенсион](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="82336-174">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="82336-175">Список расширений ядра, которые будут разрешены для загрузки.</span><span class="sxs-lookup"><span data-stu-id="82336-175">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="82336-176">.</span><span class="sxs-lookup"><span data-stu-id="82336-176"></span></span> <span data-ttu-id="82336-177">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="82336-177">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="82336-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="82336-178">Response</span></span>
<span data-ttu-id="82336-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82336-179">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82336-180">Пример</span><span class="sxs-lookup"><span data-stu-id="82336-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="82336-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="82336-181">Request</span></span>
<span data-ttu-id="82336-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82336-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 610

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="82336-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="82336-183">Response</span></span>
<span data-ttu-id="82336-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82336-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 782

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```





