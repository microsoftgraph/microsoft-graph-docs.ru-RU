---
title: Обновление windowsPhone81GeneralConfiguration
description: Обновление свойств объекта windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12095661877145412be24cf0b3c73b61d7852500
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979482"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="b7f6e-103">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7f6e-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="b7f6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f6e-106">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7f6e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7f6e-107">Prerequisites</span></span>
<span data-ttu-id="b7f6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7f6e-110">Permission type</span></span>|<span data-ttu-id="b7f6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f6e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f6e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-115">Not supported.</span></span>|
|<span data-ttu-id="b7f6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7f6e-116">Application</span></span>|<span data-ttu-id="b7f6e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7f6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b7f6e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7f6e-119">Request headers</span></span>
|<span data-ttu-id="b7f6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7f6e-120">Header</span></span>|<span data-ttu-id="b7f6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7f6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f6e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7f6e-122">Authorization</span></span>|<span data-ttu-id="b7f6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7f6e-124">Accept</span></span>|<span data-ttu-id="b7f6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f6e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7f6e-126">Request body</span></span>
<span data-ttu-id="b7f6e-127">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="b7f6e-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="b7f6e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7f6e-129">Property</span></span>|<span data-ttu-id="b7f6e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7f6e-130">Type</span></span>|<span data-ttu-id="b7f6e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7f6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f6e-132">id</span><span class="sxs-lookup"><span data-stu-id="b7f6e-132">id</span></span>|<span data-ttu-id="b7f6e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b7f6e-133">String</span></span>|<span data-ttu-id="b7f6e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-134">Key of the entity.</span></span> <span data-ttu-id="b7f6e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7f6e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b7f6e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7f6e-137">DateTimeOffset</span></span>|<span data-ttu-id="b7f6e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b7f6e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b7f6e-140">roleScopeTagIds</span></span>|<span data-ttu-id="b7f6e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b7f6e-141">String collection</span></span>|<span data-ttu-id="b7f6e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b7f6e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b7f6e-144">supportsScopeTags</span></span>|<span data-ttu-id="b7f6e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-145">Boolean</span></span>|<span data-ttu-id="b7f6e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b7f6e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b7f6e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b7f6e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-149">This property is read-only.</span></span> <span data-ttu-id="b7f6e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7f6e-151">createdDateTime</span></span>|<span data-ttu-id="b7f6e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7f6e-152">DateTimeOffset</span></span>|<span data-ttu-id="b7f6e-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-153">DateTime the object was created.</span></span> <span data-ttu-id="b7f6e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-155">description</span><span class="sxs-lookup"><span data-stu-id="b7f6e-155">description</span></span>|<span data-ttu-id="b7f6e-156">String</span><span class="sxs-lookup"><span data-stu-id="b7f6e-156">String</span></span>|<span data-ttu-id="b7f6e-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b7f6e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b7f6e-159">displayName</span></span>|<span data-ttu-id="b7f6e-160">String</span><span class="sxs-lookup"><span data-stu-id="b7f6e-160">String</span></span>|<span data-ttu-id="b7f6e-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b7f6e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-163">version</span><span class="sxs-lookup"><span data-stu-id="b7f6e-163">version</span></span>|<span data-ttu-id="b7f6e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-164">Int32</span></span>|<span data-ttu-id="b7f6e-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-165">Version of the device configuration.</span></span> <span data-ttu-id="b7f6e-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7f6e-167">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="b7f6e-167">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="b7f6e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-168">Boolean</span></span>|<span data-ttu-id="b7f6e-169">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-169">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="b7f6e-170">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-170">This property is read-only.</span></span>|
|<span data-ttu-id="b7f6e-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="b7f6e-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="b7f6e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-172">Boolean</span></span>|<span data-ttu-id="b7f6e-173">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-173">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="b7f6e-174">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-174">bluetoothBlocked</span></span>|<span data-ttu-id="b7f6e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-175">Boolean</span></span>|<span data-ttu-id="b7f6e-176">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-176">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="b7f6e-177">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-177">cameraBlocked</span></span>|<span data-ttu-id="b7f6e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-178">Boolean</span></span>|<span data-ttu-id="b7f6e-179">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-179">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="b7f6e-180">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="b7f6e-180">cellularBlockWifiTethering</span></span>|<span data-ttu-id="b7f6e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-181">Boolean</span></span>|<span data-ttu-id="b7f6e-182">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-182">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="b7f6e-183">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-183">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b7f6e-184">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b7f6e-184">compliantAppsList</span></span>|<span data-ttu-id="b7f6e-185">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b7f6e-186">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-186">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b7f6e-187">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-187">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b7f6e-188">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b7f6e-188">compliantAppListType</span></span>|[<span data-ttu-id="b7f6e-189">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="b7f6e-189">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b7f6e-190">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-190">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b7f6e-191">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-191">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b7f6e-192">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b7f6e-192">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b7f6e-193">Логический</span><span class="sxs-lookup"><span data-stu-id="b7f6e-193">Boolean</span></span>|<span data-ttu-id="b7f6e-194">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-194">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b7f6e-195">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="b7f6e-195">emailBlockAddingAccounts</span></span>|<span data-ttu-id="b7f6e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-196">Boolean</span></span>|<span data-ttu-id="b7f6e-197">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-197">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="b7f6e-198">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-198">locationServicesBlocked</span></span>|<span data-ttu-id="b7f6e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-199">Boolean</span></span>|<span data-ttu-id="b7f6e-200">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-200">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="b7f6e-201">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-201">microsoftAccountBlocked</span></span>|<span data-ttu-id="b7f6e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-202">Boolean</span></span>|<span data-ttu-id="b7f6e-203">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-203">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="b7f6e-204">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-204">nfcBlocked</span></span>|<span data-ttu-id="b7f6e-205">Логический</span><span class="sxs-lookup"><span data-stu-id="b7f6e-205">Boolean</span></span>|<span data-ttu-id="b7f6e-206">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-206">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="b7f6e-207">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b7f6e-207">passwordBlockSimple</span></span>|<span data-ttu-id="b7f6e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-208">Boolean</span></span>|<span data-ttu-id="b7f6e-209">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-209">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="b7f6e-210">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b7f6e-210">passwordExpirationDays</span></span>|<span data-ttu-id="b7f6e-211">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-211">Int32</span></span>|<span data-ttu-id="b7f6e-212">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-212">Number of days before the password expires.</span></span>|
|<span data-ttu-id="b7f6e-213">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b7f6e-213">passwordMinimumLength</span></span>|<span data-ttu-id="b7f6e-214">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-214">Int32</span></span>|<span data-ttu-id="b7f6e-215">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-215">Minimum length of passwords.</span></span>|
|<span data-ttu-id="b7f6e-216">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b7f6e-216">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b7f6e-217">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-217">Int32</span></span>|<span data-ttu-id="b7f6e-218">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-218">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="b7f6e-219">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b7f6e-219">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b7f6e-220">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-220">Int32</span></span>|<span data-ttu-id="b7f6e-221">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-221">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="b7f6e-222">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b7f6e-222">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b7f6e-223">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-223">Int32</span></span>|<span data-ttu-id="b7f6e-224">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-224">Number of previous passwords to block.</span></span> <span data-ttu-id="b7f6e-225">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-225">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b7f6e-226">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b7f6e-226">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b7f6e-227">Int32</span><span class="sxs-lookup"><span data-stu-id="b7f6e-227">Int32</span></span>|<span data-ttu-id="b7f6e-228">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-228">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="b7f6e-229">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b7f6e-229">passwordRequiredType</span></span>|[<span data-ttu-id="b7f6e-230">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b7f6e-230">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b7f6e-231">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-231">Password type that is required.</span></span> <span data-ttu-id="b7f6e-232">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-232">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b7f6e-233">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b7f6e-233">passwordRequired</span></span>|<span data-ttu-id="b7f6e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-234">Boolean</span></span>|<span data-ttu-id="b7f6e-235">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-235">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="b7f6e-236">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-236">screenCaptureBlocked</span></span>|<span data-ttu-id="b7f6e-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-237">Boolean</span></span>|<span data-ttu-id="b7f6e-238">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-238">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="b7f6e-239">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="b7f6e-239">storageBlockRemovableStorage</span></span>|<span data-ttu-id="b7f6e-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-240">Boolean</span></span>|<span data-ttu-id="b7f6e-241">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-241">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="b7f6e-242">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b7f6e-242">storageRequireEncryption</span></span>|<span data-ttu-id="b7f6e-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-243">Boolean</span></span>|<span data-ttu-id="b7f6e-244">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-244">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="b7f6e-245">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-245">webBrowserBlocked</span></span>|<span data-ttu-id="b7f6e-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-246">Boolean</span></span>|<span data-ttu-id="b7f6e-247">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-247">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="b7f6e-248">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-248">wifiBlocked</span></span>|<span data-ttu-id="b7f6e-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-249">Boolean</span></span>|<span data-ttu-id="b7f6e-250">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-250">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="b7f6e-251">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="b7f6e-251">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="b7f6e-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-252">Boolean</span></span>|<span data-ttu-id="b7f6e-253">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-253">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="b7f6e-254">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-254">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b7f6e-255">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="b7f6e-255">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="b7f6e-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-256">Boolean</span></span>|<span data-ttu-id="b7f6e-257">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-257">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="b7f6e-258">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-258">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b7f6e-259">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b7f6e-259">windowsStoreBlocked</span></span>|<span data-ttu-id="b7f6e-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7f6e-260">Boolean</span></span>|<span data-ttu-id="b7f6e-261">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-261">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="b7f6e-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f6e-262">Response</span></span>
<span data-ttu-id="b7f6e-263">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f6e-264">Пример</span><span class="sxs-lookup"><span data-stu-id="b7f6e-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7f6e-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7f6e-265">Request</span></span>
<span data-ttu-id="b7f6e-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1553

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="b7f6e-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f6e-267">Response</span></span>
<span data-ttu-id="b7f6e-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```




