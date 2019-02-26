---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8330a5bbce36d486d579a87b762d962a5fab2118
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140238"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="8d255-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d255-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="8d255-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d255-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d255-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d255-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d255-106">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d255-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8d255-107">Prerequisites</span></span>
<span data-ttu-id="8d255-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d255-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d255-110">Permission type</span></span>|<span data-ttu-id="8d255-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d255-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d255-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d255-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d255-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d255-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d255-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d255-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d255-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d255-115">Not supported.</span></span>|
|<span data-ttu-id="8d255-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d255-116">Application</span></span>|<span data-ttu-id="8d255-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d255-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d255-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d255-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d255-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d255-119">Request headers</span></span>
|<span data-ttu-id="8d255-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d255-120">Header</span></span>|<span data-ttu-id="8d255-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d255-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d255-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d255-122">Authorization</span></span>|<span data-ttu-id="8d255-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8d255-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d255-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d255-124">Accept</span></span>|<span data-ttu-id="8d255-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d255-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d255-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d255-126">Request body</span></span>
<span data-ttu-id="8d255-127">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d255-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="8d255-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d255-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="8d255-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d255-129">Property</span></span>|<span data-ttu-id="8d255-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d255-130">Type</span></span>|<span data-ttu-id="8d255-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d255-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d255-132">id</span><span class="sxs-lookup"><span data-stu-id="8d255-132">id</span></span>|<span data-ttu-id="8d255-133">String</span><span class="sxs-lookup"><span data-stu-id="8d255-133">String</span></span>|<span data-ttu-id="8d255-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d255-134">Key of the entity.</span></span> <span data-ttu-id="8d255-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d255-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d255-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d255-137">DateTimeOffset</span></span>|<span data-ttu-id="8d255-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8d255-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8d255-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d255-140">roleScopeTagIds</span></span>|<span data-ttu-id="8d255-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d255-141">String collection</span></span>|<span data-ttu-id="8d255-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8d255-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d255-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8d255-144">supportsScopeTags</span></span>|<span data-ttu-id="8d255-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-145">Boolean</span></span>|<span data-ttu-id="8d255-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8d255-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d255-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8d255-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d255-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8d255-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d255-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d255-149">This property is read-only.</span></span> <span data-ttu-id="8d255-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d255-151">createdDateTime</span></span>|<span data-ttu-id="8d255-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d255-152">DateTimeOffset</span></span>|<span data-ttu-id="8d255-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8d255-153">DateTime the object was created.</span></span> <span data-ttu-id="8d255-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-155">description</span><span class="sxs-lookup"><span data-stu-id="8d255-155">description</span></span>|<span data-ttu-id="8d255-156">String</span><span class="sxs-lookup"><span data-stu-id="8d255-156">String</span></span>|<span data-ttu-id="8d255-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d255-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d255-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8d255-159">displayName</span></span>|<span data-ttu-id="8d255-160">String</span><span class="sxs-lookup"><span data-stu-id="8d255-160">String</span></span>|<span data-ttu-id="8d255-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d255-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d255-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-163">version</span><span class="sxs-lookup"><span data-stu-id="8d255-163">version</span></span>|<span data-ttu-id="8d255-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8d255-164">Int32</span></span>|<span data-ttu-id="8d255-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d255-165">Version of the device configuration.</span></span> <span data-ttu-id="8d255-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d255-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d255-167">Дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="8d255-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="8d255-168">Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="8d255-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="8d255-169">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="8d255-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="8d255-170">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="8d255-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="8d255-171">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="8d255-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="8d255-172">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d255-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="8d255-173">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="8d255-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="8d255-174">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="8d255-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="8d255-175">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="8d255-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="8d255-176">Усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="8d255-176">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="8d255-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-178">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="8d255-178">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="8d255-179">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="8d255-179">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="8d255-180">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-180">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-181">Усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="8d255-181">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="8d255-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-183">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="8d255-183">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="8d255-184">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="8d255-184">State Allowed is supported.</span></span>|
|<span data-ttu-id="8d255-185">Усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="8d255-185">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="8d255-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-187">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="8d255-187">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="8d255-188">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d255-188">State Block is supported.</span></span>|
|<span data-ttu-id="8d255-189">Усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="8d255-189">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="8d255-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-191">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8d255-191">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="8d255-192">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="8d255-192">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="8d255-193">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-194">Усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="8d255-194">userRightsLocalLogOn</span></span>|[<span data-ttu-id="8d255-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-196">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="8d255-196">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="8d255-197">Состояния NotConfigured, разрешенные и заблокированные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="8d255-197">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="8d255-198">Усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="8d255-198">userRightsBackupData</span></span>|[<span data-ttu-id="8d255-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-200">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="8d255-200">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="8d255-201">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-202">Усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="8d255-202">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="8d255-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-204">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="8d255-204">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="8d255-205">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-206">Усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="8d255-206">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="8d255-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-208">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="8d255-208">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="8d255-209">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="8d255-209">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="8d255-210">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-211">Усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="8d255-211">userRightsCreatePageFile</span></span>|[<span data-ttu-id="8d255-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-213">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="8d255-213">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="8d255-214">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-215">Усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="8d255-215">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="8d255-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-217">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="8d255-217">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="8d255-218">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-219">Усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="8d255-219">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="8d255-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-221">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="8d255-221">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="8d255-222">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-223">Усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="8d255-223">userRightsCreateToken</span></span>|[<span data-ttu-id="8d255-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-225">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="8d255-225">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="8d255-226">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-227">Усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="8d255-227">userRightsDebugPrograms</span></span>|[<span data-ttu-id="8d255-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-229">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="8d255-229">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="8d255-230">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="8d255-231">Усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="8d255-231">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="8d255-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-233">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="8d255-233">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="8d255-234">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="8d255-234">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="8d255-235">Усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="8d255-235">userRightsDelegation</span></span>|[<span data-ttu-id="8d255-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-237">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="8d255-237">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="8d255-238">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-238">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-239">Усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="8d255-239">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="8d255-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-241">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="8d255-241">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="8d255-242">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="8d255-242">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="8d255-243">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-244">Усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="8d255-244">userRightsImpersonateClient</span></span>|[<span data-ttu-id="8d255-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-246">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="8d255-246">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="8d255-247">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="8d255-247">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="8d255-248">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-249">Усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="8d255-249">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="8d255-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-251">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="8d255-251">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="8d255-252">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-253">Усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="8d255-253">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="8d255-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-255">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="8d255-255">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="8d255-256">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-257">Усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="8d255-257">userRightsLockMemory</span></span>|[<span data-ttu-id="8d255-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-259">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="8d255-259">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="8d255-260">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-261">Усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="8d255-261">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="8d255-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-263">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="8d255-263">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="8d255-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-265">Усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="8d255-265">userRightsManageVolumes</span></span>|[<span data-ttu-id="8d255-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-267">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="8d255-267">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="8d255-268">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-269">Усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="8d255-269">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="8d255-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-271">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="8d255-271">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="8d255-272">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-273">Усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="8d255-273">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="8d255-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-275">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="8d255-275">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="8d255-276">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-277">Усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="8d255-277">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="8d255-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-279">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="8d255-279">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="8d255-280">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-281">Усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="8d255-281">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="8d255-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-283">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="8d255-283">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="8d255-284">НеПравильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="8d255-284">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="8d255-285">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-286">Усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="8d255-286">userRightsRestoreData</span></span>|[<span data-ttu-id="8d255-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-288">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="8d255-288">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="8d255-289">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-290">Усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="8d255-290">userRightsTakeOwnership</span></span>|[<span data-ttu-id="8d255-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-292">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="8d255-292">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="8d255-293">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="8d255-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="8d255-294">Усерригхтсрегистерпроцессассервице</span><span class="sxs-lookup"><span data-stu-id="8d255-294">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="8d255-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8d255-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="8d255-296">Этот параметр безопасности определяет, каким учетным записям служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="8d255-296">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="8d255-297">Примечание: этот параметр безопасности не применяется к системным, локальным или сетевым учетным записям служб.</span><span class="sxs-lookup"><span data-stu-id="8d255-297">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="8d255-298">Поддерживается только блокирование состояния.</span><span class="sxs-lookup"><span data-stu-id="8d255-298">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="8d255-299">Ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="8d255-299">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="8d255-300">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-300">Boolean</span></span>|<span data-ttu-id="8d255-301">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="8d255-301">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="8d255-302">Ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="8d255-302">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="8d255-303">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="8d255-303">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="8d255-304">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="8d255-304">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="8d255-305">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="8d255-305">Default: Manual.</span></span> <span data-ttu-id="8d255-306">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8d255-306">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="8d255-307">Ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="8d255-307">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="8d255-308">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="8d255-308">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="8d255-309">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="8d255-309">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="8d255-310">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="8d255-310">Default: Manual.</span></span> <span data-ttu-id="8d255-311">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8d255-311">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="8d255-312">Ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="8d255-312">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="8d255-313">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="8d255-313">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="8d255-314">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="8d255-314">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="8d255-315">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="8d255-315">Default: Manual.</span></span> <span data-ttu-id="8d255-316">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8d255-316">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="8d255-317">Ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="8d255-317">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="8d255-318">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="8d255-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="8d255-319">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="8d255-319">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="8d255-320">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="8d255-320">Default: Manual.</span></span> <span data-ttu-id="8d255-321">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8d255-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="8d255-322">Локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="8d255-322">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="8d255-323">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-323">Boolean</span></span>|<span data-ttu-id="8d255-324">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="8d255-324">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="8d255-325">Локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="8d255-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="8d255-326">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-326">Boolean</span></span>|<span data-ttu-id="8d255-327">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8d255-327">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="8d255-328">Локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="8d255-328">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="8d255-329">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-329">Boolean</span></span>|<span data-ttu-id="8d255-330">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="8d255-330">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="8d255-331">Локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="8d255-331">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="8d255-332">String</span><span class="sxs-lookup"><span data-stu-id="8d255-332">String</span></span>|<span data-ttu-id="8d255-333">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="8d255-333">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="8d255-334">Локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="8d255-334">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="8d255-335">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-335">Boolean</span></span>|<span data-ttu-id="8d255-336">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="8d255-336">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="8d255-337">Локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="8d255-337">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="8d255-338">String</span><span class="sxs-lookup"><span data-stu-id="8d255-338">String</span></span>|<span data-ttu-id="8d255-339">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="8d255-339">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="8d255-340">Локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="8d255-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="8d255-341">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-341">Boolean</span></span>|<span data-ttu-id="8d255-342">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="8d255-342">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="8d255-343">Локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="8d255-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="8d255-344">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-344">Boolean</span></span>|<span data-ttu-id="8d255-345">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="8d255-345">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="8d255-346">Локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="8d255-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="8d255-347">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-347">Boolean</span></span>|<span data-ttu-id="8d255-348">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="8d255-348">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="8d255-349">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="8d255-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="8d255-350">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="8d255-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="8d255-351">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="8d255-351">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="8d255-352">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="8d255-352">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="8d255-353">Локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="8d255-353">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="8d255-354">Int32</span><span class="sxs-lookup"><span data-stu-id="8d255-354">Int32</span></span>|<span data-ttu-id="8d255-355">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="8d255-355">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="8d255-356">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="8d255-356">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="8d255-357">Локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="8d255-357">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="8d255-358">Int32</span><span class="sxs-lookup"><span data-stu-id="8d255-358">Int32</span></span>|<span data-ttu-id="8d255-359">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="8d255-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="8d255-360">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="8d255-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="8d255-361">Локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="8d255-361">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="8d255-362">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-362">Boolean</span></span>|<span data-ttu-id="8d255-363">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="8d255-363">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="8d255-364">Локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="8d255-364">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="8d255-365">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-365">Boolean</span></span>|<span data-ttu-id="8d255-366">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="8d255-366">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="8d255-367">Локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="8d255-367">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="8d255-368">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-368">Boolean</span></span>|<span data-ttu-id="8d255-369">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8d255-369">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="8d255-370">Локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="8d255-370">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="8d255-371">String</span><span class="sxs-lookup"><span data-stu-id="8d255-371">String</span></span>|<span data-ttu-id="8d255-372">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="8d255-372">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="8d255-373">Локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="8d255-373">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="8d255-374">String</span><span class="sxs-lookup"><span data-stu-id="8d255-374">String</span></span>|<span data-ttu-id="8d255-375">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="8d255-375">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="8d255-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="8d255-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="8d255-377">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-377">Boolean</span></span>|<span data-ttu-id="8d255-378">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="8d255-378">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="8d255-379">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="8d255-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="8d255-380">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-380">Boolean</span></span>|<span data-ttu-id="8d255-381">Помощник по ПОЛЬЗОВАТЕЛЬСКОМу ИНТЕРФЕЙСу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="8d255-381">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="8d255-382">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="8d255-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="8d255-383">String</span><span class="sxs-lookup"><span data-stu-id="8d255-383">String</span></span>|<span data-ttu-id="8d255-384">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="8d255-384">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="8d255-385">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="8d255-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="8d255-386">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8d255-386">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="8d255-387">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="8d255-387">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="8d255-388">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="8d255-388">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="8d255-389">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="8d255-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="8d255-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8d255-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="8d255-391">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="8d255-391">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="8d255-392">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="8d255-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="8d255-393">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="8d255-393">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="8d255-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="8d255-394">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="8d255-395">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="8d255-395">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="8d255-396">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="8d255-396">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="8d255-397">Ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="8d255-397">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="8d255-398">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-398">Boolean</span></span>|<span data-ttu-id="8d255-399">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="8d255-399">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="8d255-400">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="8d255-400">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="8d255-401">Локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="8d255-401">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="8d255-402">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-402">Boolean</span></span>|<span data-ttu-id="8d255-403">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="8d255-403">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="8d255-404">Локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="8d255-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="8d255-405">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-405">Boolean</span></span>|<span data-ttu-id="8d255-406">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="8d255-406">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="8d255-407">Локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="8d255-407">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="8d255-408">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-408">Boolean</span></span>|<span data-ttu-id="8d255-409">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="8d255-409">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="8d255-410">Локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="8d255-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="8d255-411">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-411">Boolean</span></span>|<span data-ttu-id="8d255-412">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="8d255-412">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="8d255-413">Локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="8d255-413">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="8d255-414">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-414">Boolean</span></span>|<span data-ttu-id="8d255-415">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="8d255-415">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="8d255-416">Локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="8d255-416">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="8d255-417">Локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="8d255-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="8d255-418">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="8d255-418">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="8d255-419">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="8d255-419">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="8d255-420">Локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="8d255-420">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="8d255-421">Локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="8d255-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="8d255-422">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-422">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="8d255-423">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="8d255-423">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="8d255-424">Локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="8d255-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="8d255-425">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-425">Boolean</span></span>|<span data-ttu-id="8d255-426">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="8d255-426">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="8d255-427">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-427">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="8d255-428">Локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="8d255-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="8d255-429">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-429">Boolean</span></span>|<span data-ttu-id="8d255-430">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8d255-430">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="8d255-431">Локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="8d255-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="8d255-432">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-432">Boolean</span></span>|<span data-ttu-id="8d255-433">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8d255-433">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="8d255-434">Локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="8d255-434">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="8d255-435">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-435">Boolean</span></span>|<span data-ttu-id="8d255-436">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8d255-436">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="8d255-437">Локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="8d255-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="8d255-438">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-438">Boolean</span></span>|<span data-ttu-id="8d255-439">Определить, включен ли режим одобрения администратором и все параметры политики контроля УЧЕТных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="8d255-439">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="8d255-440">Локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="8d255-440">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="8d255-441">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="8d255-441">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="8d255-442">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="8d255-442">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="8d255-443">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d255-443">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="8d255-444">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="8d255-444">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="8d255-445">Локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="8d255-445">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="8d255-446">Локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="8d255-447">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="8d255-447">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="8d255-448">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d255-448">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="8d255-449">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="8d255-449">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="8d255-450">Локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="8d255-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="8d255-451">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-451">Boolean</span></span>|<span data-ttu-id="8d255-452">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="8d255-452">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="8d255-453">Локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="8d255-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="8d255-454">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-454">Boolean</span></span>|<span data-ttu-id="8d255-455">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="8d255-455">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="8d255-456">Локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="8d255-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="8d255-457">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-457">Boolean</span></span>|<span data-ttu-id="8d255-458">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8d255-458">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="8d255-459">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="8d255-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="8d255-460">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-460">Boolean</span></span>|<span data-ttu-id="8d255-461">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="8d255-461">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="8d255-462">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="8d255-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="8d255-463">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-463">Boolean</span></span>|<span data-ttu-id="8d255-464">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="8d255-464">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="8d255-465">Локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="8d255-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="8d255-466">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-466">Boolean</span></span>|<span data-ttu-id="8d255-467">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="8d255-467">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="8d255-468">Локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="8d255-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="8d255-469">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-469">Boolean</span></span>|<span data-ttu-id="8d255-470">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="8d255-470">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="8d255-471">Локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="8d255-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="8d255-472">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-472">Boolean</span></span>|<span data-ttu-id="8d255-473">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="8d255-473">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="8d255-474">Локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="8d255-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="8d255-475">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-475">Boolean</span></span>|<span data-ttu-id="8d255-476">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="8d255-476">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="8d255-477">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="8d255-477">It’s not stored by default.</span></span>|
|<span data-ttu-id="8d255-478">Локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="8d255-478">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="8d255-479">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="8d255-479">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="8d255-480">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="8d255-480">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="8d255-481">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="8d255-481">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="8d255-482">Дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="8d255-482">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="8d255-483">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-483">Boolean</span></span>|<span data-ttu-id="8d255-484">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="8d255-484">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="8d255-485">Дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="8d255-485">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="8d255-486">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-486">Boolean</span></span>|<span data-ttu-id="8d255-487">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="8d255-487">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="8d255-488">Дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="8d255-488">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="8d255-489">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-489">Boolean</span></span>|<span data-ttu-id="8d255-490">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="8d255-490">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="8d255-491">Дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="8d255-491">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="8d255-492">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-492">Boolean</span></span>|<span data-ttu-id="8d255-493">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="8d255-493">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="8d255-494">Дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="8d255-494">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="8d255-495">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-495">Boolean</span></span>|<span data-ttu-id="8d255-496">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="8d255-496">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="8d255-497">Дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="8d255-497">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="8d255-498">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-498">Boolean</span></span>|<span data-ttu-id="8d255-499">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="8d255-499">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="8d255-500">Дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="8d255-500">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="8d255-501">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-501">Boolean</span></span>|<span data-ttu-id="8d255-502">Используется для отключения отображения кнопки Очистить ДОВЕРЕНный ПЛАТФОРМЕНный модуль.</span><span class="sxs-lookup"><span data-stu-id="8d255-502">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="8d255-503">Дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="8d255-503">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="8d255-504">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-504">Boolean</span></span>|<span data-ttu-id="8d255-505">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="8d255-505">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="8d255-506">Дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="8d255-506">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="8d255-507">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-507">Boolean</span></span>|<span data-ttu-id="8d255-508">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="8d255-508">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="8d255-509">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="8d255-509">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="8d255-510">Дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="8d255-510">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="8d255-511">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-511">Boolean</span></span>|<span data-ttu-id="8d255-512">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="8d255-512">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="8d255-513">Дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="8d255-513">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="8d255-514">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-514">Boolean</span></span>|<span data-ttu-id="8d255-515">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="8d255-515">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="8d255-516">Дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="8d255-516">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="8d255-517">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-517">Boolean</span></span>|<span data-ttu-id="8d255-518">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="8d255-518">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="8d255-519">Дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="8d255-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="8d255-520">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-520">Boolean</span></span>|<span data-ttu-id="8d255-521">Используется для отключения отображения обновления микроПрограммы ДОВЕРЕНного ПЛАТФОРМЕНного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="8d255-521">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="8d255-522">Дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="8d255-522">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="8d255-523">String</span><span class="sxs-lookup"><span data-stu-id="8d255-523">String</span></span>|<span data-ttu-id="8d255-524">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-524">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="8d255-525">Дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="8d255-525">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="8d255-526">String</span><span class="sxs-lookup"><span data-stu-id="8d255-526">String</span></span>|<span data-ttu-id="8d255-527">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-527">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="8d255-528">Дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="8d255-528">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="8d255-529">String</span><span class="sxs-lookup"><span data-stu-id="8d255-529">String</span></span>|<span data-ttu-id="8d255-530">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-530">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="8d255-531">Дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="8d255-531">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="8d255-532">String</span><span class="sxs-lookup"><span data-stu-id="8d255-532">String</span></span>|<span data-ttu-id="8d255-533">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-533">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="8d255-534">Дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="8d255-534">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="8d255-535">Дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="8d255-535">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="8d255-536">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="8d255-536">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="8d255-537">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="8d255-537">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="8d255-538">Дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="8d255-538">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="8d255-539">Дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-539">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="8d255-540">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-540">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="8d255-541">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="8d255-541">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="8d255-542">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="8d255-542">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="8d255-543">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-543">Boolean</span></span>|<span data-ttu-id="8d255-544">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="8d255-544">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="8d255-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="8d255-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="8d255-546">Int32</span><span class="sxs-lookup"><span data-stu-id="8d255-546">Int32</span></span>|<span data-ttu-id="8d255-547">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="8d255-547">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="8d255-548">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="8d255-548">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="8d255-549">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="8d255-549">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="8d255-550">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="8d255-550">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="8d255-551">Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-551">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="8d255-552">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="8d255-552">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="8d255-553">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="8d255-553">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="8d255-554">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="8d255-554">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="8d255-555">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-555">Boolean</span></span>|<span data-ttu-id="8d255-556">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="8d255-556">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="8d255-557">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="8d255-557">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="8d255-558">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-558">Boolean</span></span>|<span data-ttu-id="8d255-559">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="8d255-559">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="8d255-560">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="8d255-560">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="8d255-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d255-561">Boolean</span></span>|<span data-ttu-id="8d255-562">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="8d255-562">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="8d255-563">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="8d255-563">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="8d255-564">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-564">Boolean</span></span>|<span data-ttu-id="8d255-565">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="8d255-565">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="8d255-566">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="8d255-566">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="8d255-567">Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-567">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="8d255-568">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8d255-568">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="8d255-569">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="8d255-569">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="8d255-570">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="8d255-570">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="8d255-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d255-571">Boolean</span></span>|<span data-ttu-id="8d255-572">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="8d255-572">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="8d255-573">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="8d255-573">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="8d255-574">Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-574">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="8d255-575">НаСтраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="8d255-575">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="8d255-576">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="8d255-576">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="8d255-577">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="8d255-577">firewallProfileDomain</span></span>|[<span data-ttu-id="8d255-578">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d255-578">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="8d255-579">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="8d255-579">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="8d255-580">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="8d255-580">firewallProfilePublic</span></span>|[<span data-ttu-id="8d255-581">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d255-581">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="8d255-582">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="8d255-582">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="8d255-583">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="8d255-583">firewallProfilePrivate</span></span>|[<span data-ttu-id="8d255-584">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d255-584">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="8d255-585">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="8d255-585">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="8d255-586">Дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="8d255-586">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="8d255-587">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-587">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-588">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="8d255-588">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="8d255-589">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-589">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-590">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="8d255-590">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="8d255-591">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d255-591">String collection</span></span>|<span data-ttu-id="8d255-592">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="8d255-592">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="8d255-593">Дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-593">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="8d255-594">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-594">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-595">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="8d255-595">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="8d255-596">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-596">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-597">Дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="8d255-597">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="8d255-598">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-598">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-599">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="8d255-599">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="8d255-600">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-600">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-601">Дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="8d255-601">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="8d255-602">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-603">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="8d255-603">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="8d255-604">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-605">Дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="8d255-606">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-606">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-607">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="8d255-607">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="8d255-608">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-608">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-609">Дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="8d255-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="8d255-610">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-611">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="8d255-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="8d255-612">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-612">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-613">Дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="8d255-613">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="8d255-614">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-615">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="8d255-615">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="8d255-616">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-617">Дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="8d255-617">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="8d255-618">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-619">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="8d255-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="8d255-620">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-621">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="8d255-621">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="8d255-622">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-623">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="8d255-623">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="8d255-624">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-625">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="8d255-625">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="8d255-626">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-627">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="8d255-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="8d255-628">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-629">Дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-629">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="8d255-630">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-631">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="8d255-631">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="8d255-632">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-633">Дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="8d255-633">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="8d255-634">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-635">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="8d255-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="8d255-636">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-637">Дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-637">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="8d255-638">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-639">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="8d255-639">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="8d255-640">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-641">Дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="8d255-641">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="8d255-642">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-643">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="8d255-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="8d255-644">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-645">Дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-645">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="8d255-646">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-647">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="8d255-647">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="8d255-648">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-649">Дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-649">defenderProcessCreationType</span></span>|[<span data-ttu-id="8d255-650">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-651">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="8d255-651">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="8d255-652">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-653">Дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="8d255-653">defenderProcessCreation</span></span>|[<span data-ttu-id="8d255-654">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-655">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="8d255-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="8d255-656">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-657">Дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="8d255-657">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="8d255-658">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-659">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="8d255-659">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="8d255-660">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-661">Дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="8d255-661">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="8d255-662">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-663">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="8d255-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="8d255-664">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-665">Дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-665">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="8d255-666">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-667">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="8d255-667">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="8d255-668">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-669">Дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="8d255-669">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="8d255-670">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-671">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="8d255-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="8d255-672">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-673">Дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-673">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="8d255-674">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="8d255-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="8d255-675">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="8d255-675">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="8d255-676">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-677">Дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="8d255-677">defenderEmailContentExecution</span></span>|[<span data-ttu-id="8d255-678">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-679">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="8d255-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="8d255-680">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-681">Дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-681">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="8d255-682">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-683">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="8d255-683">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="8d255-684">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-685">Дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="8d255-685">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="8d255-686">Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-686">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="8d255-687">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="8d255-687">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="8d255-688">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="8d255-688">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="8d255-689">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="8d255-689">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="8d255-690">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d255-690">String collection</span></span>|<span data-ttu-id="8d255-691">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="8d255-691">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="8d255-692">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="8d255-692">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="8d255-693">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d255-693">String collection</span></span>|<span data-ttu-id="8d255-694">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="8d255-694">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="8d255-695">Дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-695">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="8d255-696">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-696">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="8d255-697">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="8d255-697">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="8d255-698">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="8d255-698">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="8d255-699">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="8d255-699">defenderExploitProtectionXml</span></span>|<span data-ttu-id="8d255-700">Binary</span><span class="sxs-lookup"><span data-stu-id="8d255-700">Binary</span></span>|<span data-ttu-id="8d255-701">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="8d255-701">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="8d255-702">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="8d255-702">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="8d255-703">String</span><span class="sxs-lookup"><span data-stu-id="8d255-703">String</span></span>|<span data-ttu-id="8d255-704">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="8d255-704">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="8d255-705">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="8d255-705">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="8d255-706">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-706">Boolean</span></span>|<span data-ttu-id="8d255-707">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="8d255-707">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="8d255-708">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="8d255-708">appLockerApplicationControl</span></span>|[<span data-ttu-id="8d255-709">Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-709">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="8d255-710">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="8d255-710">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="8d255-711">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="8d255-711">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="8d255-712">Девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="8d255-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="8d255-713">Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="8d255-714">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной заГрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="8d255-714">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="8d255-715">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="8d255-715">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="8d255-716">Девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="8d255-716">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="8d255-717">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-717">Boolean</span></span>|<span data-ttu-id="8d255-718">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="8d255-718">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="8d255-719">Девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="8d255-719">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="8d255-720">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-720">Boolean</span></span>|<span data-ttu-id="8d255-721">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="8d255-721">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="8d255-722">Девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="8d255-722">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="8d255-723">Включение</span><span class="sxs-lookup"><span data-stu-id="8d255-723">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8d255-724">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="8d255-724">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="8d255-725">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8d255-725">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8d255-726">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="8d255-726">smartScreenEnableInShell</span></span>|<span data-ttu-id="8d255-727">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-727">Boolean</span></span>|<span data-ttu-id="8d255-728">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="8d255-728">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="8d255-729">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="8d255-729">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="8d255-730">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-730">Boolean</span></span>|<span data-ttu-id="8d255-731">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="8d255-731">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="8d255-732">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="8d255-732">applicationGuardEnabled</span></span>|<span data-ttu-id="8d255-733">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-733">Boolean</span></span>|<span data-ttu-id="8d255-734">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="8d255-734">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="8d255-735">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="8d255-735">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="8d255-736">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="8d255-736">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="8d255-737">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="8d255-737">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="8d255-738">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="8d255-738">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="8d255-739">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="8d255-739">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="8d255-740">Аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="8d255-740">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="8d255-741">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="8d255-741">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="8d255-742">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="8d255-742">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="8d255-743">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="8d255-743">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="8d255-744">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-744">Boolean</span></span>|<span data-ttu-id="8d255-745">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="8d255-745">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="8d255-746">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="8d255-746">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="8d255-747">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-747">Boolean</span></span>|<span data-ttu-id="8d255-748">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="8d255-748">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="8d255-749">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="8d255-749">applicationGuardForceAuditing</span></span>|<span data-ttu-id="8d255-750">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-750">Boolean</span></span>|<span data-ttu-id="8d255-751">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="8d255-751">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="8d255-752">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="8d255-752">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="8d255-753">Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="8d255-753">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="8d255-754">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="8d255-754">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="8d255-755">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="8d255-755">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="8d255-756">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="8d255-756">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="8d255-757">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-757">Boolean</span></span>|<span data-ttu-id="8d255-758">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="8d255-758">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="8d255-759">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="8d255-759">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="8d255-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d255-760">Boolean</span></span>|<span data-ttu-id="8d255-761">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="8d255-761">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="8d255-762">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="8d255-762">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="8d255-763">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-763">Boolean</span></span>|<span data-ttu-id="8d255-764">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="8d255-764">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="8d255-765">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="8d255-765">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="8d255-766">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-766">Boolean</span></span>|<span data-ttu-id="8d255-767">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="8d255-767">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="8d255-768">Аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="8d255-768">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="8d255-769">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-769">Boolean</span></span>|<span data-ttu-id="8d255-770">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="8d255-770">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="8d255-771">Аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="8d255-771">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="8d255-772">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-772">Boolean</span></span>|<span data-ttu-id="8d255-773">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="8d255-773">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="8d255-774">Битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="8d255-774">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="8d255-775">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-775">Boolean</span></span>|<span data-ttu-id="8d255-776">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время приСоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d255-776">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="8d255-777">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="8d255-777">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="8d255-778">Логический</span><span class="sxs-lookup"><span data-stu-id="8d255-778">Boolean</span></span>|<span data-ttu-id="8d255-779">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d255-779">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="8d255-780">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="8d255-780">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="8d255-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d255-781">Boolean</span></span>|<span data-ttu-id="8d255-782">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8d255-782">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="8d255-783">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="8d255-783">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="8d255-784">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="8d255-784">bitLockerEncryptDevice</span></span>|<span data-ttu-id="8d255-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d255-785">Boolean</span></span>|<span data-ttu-id="8d255-786">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8d255-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="8d255-787">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="8d255-787">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="8d255-788">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="8d255-788">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="8d255-789">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8d255-789">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="8d255-790">bitLockerFixedDrivePolicy;</span><span class="sxs-lookup"><span data-stu-id="8d255-790">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="8d255-791">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="8d255-791">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="8d255-792">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8d255-792">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="8d255-793">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="8d255-793">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="8d255-794">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="8d255-794">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="8d255-795">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="8d255-795">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8d255-796">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d255-796">Response</span></span>
<span data-ttu-id="8d255-797">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d255-797">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d255-798">Пример</span><span class="sxs-lookup"><span data-stu-id="8d255-798">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d255-799">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d255-799">Request</span></span>
<span data-ttu-id="8d255-800">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d255-800">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26778

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="8d255-801">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d255-801">Response</span></span>
<span data-ttu-id="8d255-p198">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d255-p198">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26950

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```




