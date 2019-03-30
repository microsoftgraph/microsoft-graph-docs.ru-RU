---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1fc2745ffe0a9c3274b23d424401f19f76cc50b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987239"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="64aa0-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aa0-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="64aa0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64aa0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64aa0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64aa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64aa0-106">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64aa0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64aa0-107">Prerequisites</span></span>
<span data-ttu-id="64aa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64aa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64aa0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64aa0-110">Permission type</span></span>|<span data-ttu-id="64aa0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64aa0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64aa0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64aa0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64aa0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64aa0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64aa0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64aa0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64aa0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64aa0-115">Not supported.</span></span>|
|<span data-ttu-id="64aa0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64aa0-116">Application</span></span>|<span data-ttu-id="64aa0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64aa0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64aa0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64aa0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64aa0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64aa0-119">Request headers</span></span>
|<span data-ttu-id="64aa0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64aa0-120">Header</span></span>|<span data-ttu-id="64aa0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64aa0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64aa0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64aa0-122">Authorization</span></span>|<span data-ttu-id="64aa0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64aa0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64aa0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64aa0-124">Accept</span></span>|<span data-ttu-id="64aa0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64aa0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64aa0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64aa0-126">Request body</span></span>
<span data-ttu-id="64aa0-127">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64aa0-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="64aa0-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="64aa0-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="64aa0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="64aa0-129">Property</span></span>|<span data-ttu-id="64aa0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="64aa0-130">Type</span></span>|<span data-ttu-id="64aa0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="64aa0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64aa0-132">id</span><span class="sxs-lookup"><span data-stu-id="64aa0-132">id</span></span>|<span data-ttu-id="64aa0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="64aa0-133">String</span></span>|<span data-ttu-id="64aa0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64aa0-134">Key of the entity.</span></span> <span data-ttu-id="64aa0-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64aa0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="64aa0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64aa0-137">DateTimeOffset</span></span>|<span data-ttu-id="64aa0-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="64aa0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="64aa0-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64aa0-140">roleScopeTagIds</span></span>|<span data-ttu-id="64aa0-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64aa0-141">String collection</span></span>|<span data-ttu-id="64aa0-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="64aa0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64aa0-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="64aa0-144">supportsScopeTags</span></span>|<span data-ttu-id="64aa0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-145">Boolean</span></span>|<span data-ttu-id="64aa0-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="64aa0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64aa0-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="64aa0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64aa0-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="64aa0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64aa0-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64aa0-149">This property is read-only.</span></span> <span data-ttu-id="64aa0-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64aa0-151">createdDateTime</span></span>|<span data-ttu-id="64aa0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64aa0-152">DateTimeOffset</span></span>|<span data-ttu-id="64aa0-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="64aa0-153">DateTime the object was created.</span></span> <span data-ttu-id="64aa0-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-155">description</span><span class="sxs-lookup"><span data-stu-id="64aa0-155">description</span></span>|<span data-ttu-id="64aa0-156">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-156">String</span></span>|<span data-ttu-id="64aa0-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64aa0-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="64aa0-159">displayName</span></span>|<span data-ttu-id="64aa0-160">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-160">String</span></span>|<span data-ttu-id="64aa0-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64aa0-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-163">version</span><span class="sxs-lookup"><span data-stu-id="64aa0-163">version</span></span>|<span data-ttu-id="64aa0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="64aa0-164">Int32</span></span>|<span data-ttu-id="64aa0-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-165">Version of the device configuration.</span></span> <span data-ttu-id="64aa0-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aa0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aa0-167">Дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="64aa0-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="64aa0-168">Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="64aa0-169">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="64aa0-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="64aa0-170">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="64aa0-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="64aa0-171">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="64aa0-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="64aa0-172">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="64aa0-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="64aa0-173">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="64aa0-174">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="64aa0-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="64aa0-175">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="64aa0-176">Фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="64aa0-176">firewallRules</span></span>|<span data-ttu-id="64aa0-177">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="64aa0-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="64aa0-178">НаСтраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="64aa0-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="64aa0-179">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="64aa0-180">Усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="64aa0-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="64aa0-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-182">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="64aa0-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="64aa0-183">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="64aa0-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="64aa0-184">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-185">Усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="64aa0-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="64aa0-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-187">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="64aa0-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="64aa0-188">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="64aa0-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="64aa0-189">Усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="64aa0-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="64aa0-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-191">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="64aa0-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="64aa0-192">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64aa0-192">State Block is supported.</span></span>|
|<span data-ttu-id="64aa0-193">Усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="64aa0-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="64aa0-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-195">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="64aa0-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="64aa0-196">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="64aa0-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="64aa0-197">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-198">Усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="64aa0-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="64aa0-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-200">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="64aa0-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="64aa0-201">Состояния NotConfigured, разрешенные и заблокированные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="64aa0-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="64aa0-202">Усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="64aa0-202">userRightsBackupData</span></span>|[<span data-ttu-id="64aa0-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-204">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="64aa0-205">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-206">Усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="64aa0-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="64aa0-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-208">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="64aa0-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="64aa0-209">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-210">Усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="64aa0-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="64aa0-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-212">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="64aa0-213">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="64aa0-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="64aa0-214">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-215">Усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="64aa0-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="64aa0-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-217">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="64aa0-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="64aa0-218">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-219">Усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="64aa0-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="64aa0-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-221">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="64aa0-222">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-223">Усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="64aa0-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="64aa0-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-225">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="64aa0-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="64aa0-226">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-227">Усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="64aa0-227">userRightsCreateToken</span></span>|[<span data-ttu-id="64aa0-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-229">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="64aa0-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="64aa0-230">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-231">Усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="64aa0-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="64aa0-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-233">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="64aa0-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="64aa0-234">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="64aa0-235">Усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="64aa0-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="64aa0-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-237">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="64aa0-238">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="64aa0-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="64aa0-239">Усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="64aa0-239">userRightsDelegation</span></span>|[<span data-ttu-id="64aa0-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-241">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="64aa0-242">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-243">Усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="64aa0-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="64aa0-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-245">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="64aa0-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="64aa0-246">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="64aa0-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="64aa0-247">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-248">Усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="64aa0-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="64aa0-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-250">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="64aa0-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="64aa0-251">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="64aa0-252">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-253">Усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="64aa0-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="64aa0-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-255">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="64aa0-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="64aa0-256">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-257">Усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="64aa0-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="64aa0-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-259">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="64aa0-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="64aa0-260">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-261">Усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="64aa0-261">userRightsLockMemory</span></span>|[<span data-ttu-id="64aa0-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-263">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="64aa0-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="64aa0-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-265">Усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="64aa0-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="64aa0-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-267">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="64aa0-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="64aa0-268">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-269">Усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="64aa0-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="64aa0-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-271">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="64aa0-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="64aa0-272">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-273">Усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="64aa0-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="64aa0-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-275">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="64aa0-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="64aa0-276">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-277">Усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="64aa0-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="64aa0-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-279">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="64aa0-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="64aa0-280">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-281">Усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="64aa0-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="64aa0-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-283">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="64aa0-284">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-285">Усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="64aa0-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="64aa0-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-287">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="64aa0-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="64aa0-288">НеПравильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="64aa0-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="64aa0-289">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-290">Усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="64aa0-290">userRightsRestoreData</span></span>|[<span data-ttu-id="64aa0-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-292">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="64aa0-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="64aa0-293">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-294">Усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="64aa0-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="64aa0-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-296">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="64aa0-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="64aa0-297">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="64aa0-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="64aa0-298">Усерригхтсрегистерпроцессассервице</span><span class="sxs-lookup"><span data-stu-id="64aa0-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="64aa0-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="64aa0-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="64aa0-300">Этот параметр безопасности определяет, каким учетным записям служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="64aa0-301">Примечание: этот параметр безопасности не применяется к системным, локальным или сетевым учетным записям служб.</span><span class="sxs-lookup"><span data-stu-id="64aa0-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="64aa0-302">Поддерживается только блокирование состояния.</span><span class="sxs-lookup"><span data-stu-id="64aa0-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="64aa0-303">Ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="64aa0-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="64aa0-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-304">Boolean</span></span>|<span data-ttu-id="64aa0-305">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="64aa0-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="64aa0-306">Ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="64aa0-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="64aa0-307">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="64aa0-308">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="64aa0-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="64aa0-309">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="64aa0-309">Default: Manual.</span></span> <span data-ttu-id="64aa0-310">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="64aa0-311">Ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="64aa0-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="64aa0-312">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="64aa0-313">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="64aa0-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="64aa0-314">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="64aa0-314">Default: Manual.</span></span> <span data-ttu-id="64aa0-315">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="64aa0-316">Ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="64aa0-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="64aa0-317">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="64aa0-318">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="64aa0-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="64aa0-319">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="64aa0-319">Default: Manual.</span></span> <span data-ttu-id="64aa0-320">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="64aa0-321">Ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="64aa0-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="64aa0-322">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="64aa0-323">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="64aa0-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="64aa0-324">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="64aa0-324">Default: Manual.</span></span> <span data-ttu-id="64aa0-325">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="64aa0-326">Локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="64aa0-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="64aa0-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-327">Boolean</span></span>|<span data-ttu-id="64aa0-328">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="64aa0-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="64aa0-329">Локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="64aa0-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="64aa0-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-330">Boolean</span></span>|<span data-ttu-id="64aa0-331">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="64aa0-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="64aa0-332">Локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="64aa0-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="64aa0-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-333">Boolean</span></span>|<span data-ttu-id="64aa0-334">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="64aa0-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="64aa0-335">Локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="64aa0-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="64aa0-336">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-336">String</span></span>|<span data-ttu-id="64aa0-337">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="64aa0-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="64aa0-338">Локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="64aa0-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="64aa0-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-339">Boolean</span></span>|<span data-ttu-id="64aa0-340">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="64aa0-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="64aa0-341">Локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="64aa0-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="64aa0-342">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-342">String</span></span>|<span data-ttu-id="64aa0-343">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="64aa0-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="64aa0-344">Локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="64aa0-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="64aa0-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-345">Boolean</span></span>|<span data-ttu-id="64aa0-346">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="64aa0-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="64aa0-347">Локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="64aa0-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="64aa0-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-348">Boolean</span></span>|<span data-ttu-id="64aa0-349">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="64aa0-350">Локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="64aa0-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="64aa0-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-351">Boolean</span></span>|<span data-ttu-id="64aa0-352">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="64aa0-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="64aa0-353">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="64aa0-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="64aa0-354">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="64aa0-355">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="64aa0-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="64aa0-356">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="64aa0-357">Локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="64aa0-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="64aa0-358">Int32</span><span class="sxs-lookup"><span data-stu-id="64aa0-358">Int32</span></span>|<span data-ttu-id="64aa0-359">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="64aa0-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="64aa0-360">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="64aa0-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="64aa0-361">Локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="64aa0-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="64aa0-362">Int32</span><span class="sxs-lookup"><span data-stu-id="64aa0-362">Int32</span></span>|<span data-ttu-id="64aa0-363">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="64aa0-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="64aa0-364">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="64aa0-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="64aa0-365">Локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="64aa0-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="64aa0-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-366">Boolean</span></span>|<span data-ttu-id="64aa0-367">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="64aa0-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="64aa0-368">Локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="64aa0-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="64aa0-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-369">Boolean</span></span>|<span data-ttu-id="64aa0-370">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="64aa0-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="64aa0-371">Локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="64aa0-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="64aa0-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-372">Boolean</span></span>|<span data-ttu-id="64aa0-373">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="64aa0-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="64aa0-374">Локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="64aa0-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="64aa0-375">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-375">String</span></span>|<span data-ttu-id="64aa0-376">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="64aa0-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="64aa0-377">Локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="64aa0-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="64aa0-378">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-378">String</span></span>|<span data-ttu-id="64aa0-379">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="64aa0-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="64aa0-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="64aa0-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="64aa0-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-381">Boolean</span></span>|<span data-ttu-id="64aa0-382">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="64aa0-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="64aa0-383">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="64aa0-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="64aa0-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-384">Boolean</span></span>|<span data-ttu-id="64aa0-385">Помощник по ПОЛЬЗОВАТЕЛЬСКОМу ИНТЕРФЕЙСу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="64aa0-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="64aa0-386">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="64aa0-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="64aa0-387">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-387">String</span></span>|<span data-ttu-id="64aa0-388">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="64aa0-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="64aa0-389">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="64aa0-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="64aa0-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="64aa0-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="64aa0-391">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="64aa0-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="64aa0-392">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="64aa0-393">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="64aa0-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="64aa0-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="64aa0-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="64aa0-395">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="64aa0-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="64aa0-396">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="64aa0-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="64aa0-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="64aa0-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="64aa0-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="64aa0-399">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="64aa0-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="64aa0-400">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="64aa0-401">Ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="64aa0-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="64aa0-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-402">Boolean</span></span>|<span data-ttu-id="64aa0-403">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="64aa0-404">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="64aa0-405">Локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="64aa0-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="64aa0-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-406">Boolean</span></span>|<span data-ttu-id="64aa0-407">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="64aa0-408">Локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="64aa0-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="64aa0-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-409">Boolean</span></span>|<span data-ttu-id="64aa0-410">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="64aa0-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="64aa0-411">Локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="64aa0-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="64aa0-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-412">Boolean</span></span>|<span data-ttu-id="64aa0-413">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="64aa0-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="64aa0-414">Локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="64aa0-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="64aa0-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-415">Boolean</span></span>|<span data-ttu-id="64aa0-416">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="64aa0-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="64aa0-417">Локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="64aa0-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="64aa0-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-418">Boolean</span></span>|<span data-ttu-id="64aa0-419">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="64aa0-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="64aa0-420">Локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="64aa0-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="64aa0-421">Локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="64aa0-422">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="64aa0-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="64aa0-423">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="64aa0-424">Локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="64aa0-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="64aa0-425">Локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="64aa0-426">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="64aa0-427">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="64aa0-428">Локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="64aa0-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="64aa0-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-429">Boolean</span></span>|<span data-ttu-id="64aa0-430">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="64aa0-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="64aa0-431">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="64aa0-432">Локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="64aa0-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="64aa0-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-433">Boolean</span></span>|<span data-ttu-id="64aa0-434">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="64aa0-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="64aa0-435">Локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="64aa0-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="64aa0-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-436">Boolean</span></span>|<span data-ttu-id="64aa0-437">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="64aa0-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="64aa0-438">Локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="64aa0-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="64aa0-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-439">Boolean</span></span>|<span data-ttu-id="64aa0-440">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="64aa0-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="64aa0-441">Локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="64aa0-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="64aa0-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-442">Boolean</span></span>|<span data-ttu-id="64aa0-443">Определить, включен ли режим одобрения администратором и все параметры политики контроля УЧЕТных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="64aa0-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="64aa0-444">Локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="64aa0-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="64aa0-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="64aa0-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="64aa0-446">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="64aa0-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="64aa0-447">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="64aa0-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="64aa0-448">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="64aa0-449">Локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="64aa0-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="64aa0-450">Локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="64aa0-451">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="64aa0-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="64aa0-452">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="64aa0-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="64aa0-453">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="64aa0-454">Локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="64aa0-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="64aa0-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-455">Boolean</span></span>|<span data-ttu-id="64aa0-456">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="64aa0-457">Локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="64aa0-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="64aa0-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-458">Boolean</span></span>|<span data-ttu-id="64aa0-459">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="64aa0-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="64aa0-460">Локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="64aa0-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="64aa0-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-461">Boolean</span></span>|<span data-ttu-id="64aa0-462">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="64aa0-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="64aa0-463">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="64aa0-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="64aa0-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-464">Boolean</span></span>|<span data-ttu-id="64aa0-465">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="64aa0-466">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="64aa0-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="64aa0-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-467">Boolean</span></span>|<span data-ttu-id="64aa0-468">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="64aa0-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="64aa0-469">Локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="64aa0-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="64aa0-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-470">Boolean</span></span>|<span data-ttu-id="64aa0-471">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="64aa0-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="64aa0-472">Локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="64aa0-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="64aa0-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-473">Boolean</span></span>|<span data-ttu-id="64aa0-474">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="64aa0-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="64aa0-475">Локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="64aa0-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="64aa0-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-476">Boolean</span></span>|<span data-ttu-id="64aa0-477">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="64aa0-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="64aa0-478">Локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="64aa0-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="64aa0-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-479">Boolean</span></span>|<span data-ttu-id="64aa0-480">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="64aa0-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="64aa0-481">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="64aa0-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="64aa0-482">Локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="64aa0-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="64aa0-483">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="64aa0-483">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="64aa0-484">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="64aa0-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="64aa0-485">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="64aa0-486">Дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="64aa0-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="64aa0-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-487">Boolean</span></span>|<span data-ttu-id="64aa0-488">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="64aa0-489">Дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="64aa0-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="64aa0-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-490">Boolean</span></span>|<span data-ttu-id="64aa0-491">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="64aa0-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="64aa0-492">Дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="64aa0-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-493">Boolean</span></span>|<span data-ttu-id="64aa0-494">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="64aa0-495">Дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="64aa0-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-496">Boolean</span></span>|<span data-ttu-id="64aa0-497">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="64aa0-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="64aa0-498">Дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="64aa0-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-499">Boolean</span></span>|<span data-ttu-id="64aa0-500">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="64aa0-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="64aa0-501">Дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="64aa0-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-502">Boolean</span></span>|<span data-ttu-id="64aa0-503">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="64aa0-504">Дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="64aa0-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-505">Boolean</span></span>|<span data-ttu-id="64aa0-506">Используется для отключения отображения кнопки Очистить ДОВЕРЕНный ПЛАТФОРМЕНный модуль.</span><span class="sxs-lookup"><span data-stu-id="64aa0-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="64aa0-507">Дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="64aa0-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-508">Boolean</span></span>|<span data-ttu-id="64aa0-509">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="64aa0-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="64aa0-510">Дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="64aa0-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="64aa0-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-511">Boolean</span></span>|<span data-ttu-id="64aa0-512">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="64aa0-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="64aa0-513">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="64aa0-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="64aa0-514">Дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="64aa0-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-515">Boolean</span></span>|<span data-ttu-id="64aa0-516">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="64aa0-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="64aa0-517">Дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="64aa0-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-518">Boolean</span></span>|<span data-ttu-id="64aa0-519">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="64aa0-520">Дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="64aa0-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-521">Boolean</span></span>|<span data-ttu-id="64aa0-522">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="64aa0-523">Дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="64aa0-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="64aa0-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-524">Boolean</span></span>|<span data-ttu-id="64aa0-525">Используется для отключения отображения обновления микроПрограммы ДОВЕРЕНного ПЛАТФОРМЕНного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="64aa0-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="64aa0-526">Дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="64aa0-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="64aa0-527">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-527">String</span></span>|<span data-ttu-id="64aa0-528">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="64aa0-529">Дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="64aa0-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="64aa0-530">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-530">String</span></span>|<span data-ttu-id="64aa0-531">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="64aa0-532">Дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="64aa0-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="64aa0-533">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-533">String</span></span>|<span data-ttu-id="64aa0-534">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="64aa0-535">Дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="64aa0-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="64aa0-536">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-536">String</span></span>|<span data-ttu-id="64aa0-537">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="64aa0-538">Дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="64aa0-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="64aa0-539">Дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="64aa0-540">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="64aa0-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="64aa0-541">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="64aa0-542">Дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="64aa0-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="64aa0-543">Дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="64aa0-544">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="64aa0-545">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="64aa0-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="64aa0-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="64aa0-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-547">Boolean</span></span>|<span data-ttu-id="64aa0-548">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="64aa0-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="64aa0-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="64aa0-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="64aa0-550">Int32</span><span class="sxs-lookup"><span data-stu-id="64aa0-550">Int32</span></span>|<span data-ttu-id="64aa0-551">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="64aa0-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="64aa0-552">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="64aa0-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="64aa0-553">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="64aa0-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="64aa0-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="64aa0-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="64aa0-555">Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="64aa0-556">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="64aa0-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="64aa0-557">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="64aa0-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="64aa0-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="64aa0-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-559">Boolean</span></span>|<span data-ttu-id="64aa0-560">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="64aa0-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="64aa0-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="64aa0-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="64aa0-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-562">Boolean</span></span>|<span data-ttu-id="64aa0-563">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="64aa0-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="64aa0-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="64aa0-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="64aa0-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-565">Boolean</span></span>|<span data-ttu-id="64aa0-566">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="64aa0-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="64aa0-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="64aa0-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="64aa0-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-568">Boolean</span></span>|<span data-ttu-id="64aa0-569">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="64aa0-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="64aa0-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="64aa0-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="64aa0-571">Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="64aa0-572">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="64aa0-573">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="64aa0-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="64aa0-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="64aa0-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-575">Boolean</span></span>|<span data-ttu-id="64aa0-576">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="64aa0-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="64aa0-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="64aa0-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="64aa0-578">Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="64aa0-579">НаСтраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="64aa0-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="64aa0-580">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="64aa0-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="64aa0-581">firewallProfileDomain</span></span>|[<span data-ttu-id="64aa0-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="64aa0-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="64aa0-583">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="64aa0-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="64aa0-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="64aa0-584">firewallProfilePublic</span></span>|[<span data-ttu-id="64aa0-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="64aa0-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="64aa0-586">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="64aa0-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="64aa0-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="64aa0-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="64aa0-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="64aa0-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="64aa0-589">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="64aa0-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="64aa0-590">Дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="64aa0-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="64aa0-591">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-592">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="64aa0-593">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="64aa0-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="64aa0-595">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64aa0-595">String collection</span></span>|<span data-ttu-id="64aa0-596">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="64aa0-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="64aa0-597">Дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="64aa0-598">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-599">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="64aa0-600">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-601">Дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="64aa0-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="64aa0-602">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-603">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="64aa0-604">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-605">Дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="64aa0-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="64aa0-606">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-607">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="64aa0-608">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-609">Дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="64aa0-610">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-611">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="64aa0-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="64aa0-612">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-613">Дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="64aa0-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="64aa0-614">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-615">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="64aa0-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="64aa0-616">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-617">Дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="64aa0-618">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-619">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="64aa0-620">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-621">Дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="64aa0-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="64aa0-622">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-623">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="64aa0-624">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="64aa0-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="64aa0-626">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-627">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="64aa0-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="64aa0-628">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="64aa0-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="64aa0-630">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-631">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="64aa0-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="64aa0-632">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-633">Дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="64aa0-634">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-635">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="64aa0-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="64aa0-636">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-637">Дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="64aa0-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="64aa0-638">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-639">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="64aa0-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="64aa0-640">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-641">Дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="64aa0-642">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-643">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="64aa0-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="64aa0-644">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-645">Дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="64aa0-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="64aa0-646">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-647">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="64aa0-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="64aa0-648">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-649">Дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="64aa0-650">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-651">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="64aa0-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="64aa0-652">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-653">Дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="64aa0-654">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-655">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="64aa0-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="64aa0-656">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-657">Дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="64aa0-657">defenderProcessCreation</span></span>|[<span data-ttu-id="64aa0-658">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-659">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="64aa0-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="64aa0-660">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-661">Дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="64aa0-662">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-663">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="64aa0-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="64aa0-664">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-665">Дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="64aa0-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="64aa0-666">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-667">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="64aa0-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="64aa0-668">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-669">Дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="64aa0-670">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-671">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="64aa0-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="64aa0-672">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-673">Дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="64aa0-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="64aa0-674">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-675">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="64aa0-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="64aa0-676">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-677">Дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="64aa0-678">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="64aa0-679">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="64aa0-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="64aa0-680">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-681">Дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="64aa0-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="64aa0-682">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-683">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="64aa0-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="64aa0-684">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-685">Дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="64aa0-686">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-687">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="64aa0-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="64aa0-688">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-689">Дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="64aa0-690">Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="64aa0-691">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="64aa0-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="64aa0-692">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="64aa0-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="64aa0-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="64aa0-694">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64aa0-694">String collection</span></span>|<span data-ttu-id="64aa0-695">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="64aa0-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="64aa0-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="64aa0-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="64aa0-697">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64aa0-697">String collection</span></span>|<span data-ttu-id="64aa0-698">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="64aa0-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="64aa0-699">Дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="64aa0-700">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="64aa0-701">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="64aa0-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="64aa0-702">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="64aa0-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="64aa0-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="64aa0-704">Binary</span><span class="sxs-lookup"><span data-stu-id="64aa0-704">Binary</span></span>|<span data-ttu-id="64aa0-705">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="64aa0-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="64aa0-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="64aa0-707">String</span><span class="sxs-lookup"><span data-stu-id="64aa0-707">String</span></span>|<span data-ttu-id="64aa0-708">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="64aa0-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="64aa0-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="64aa0-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="64aa0-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-710">Boolean</span></span>|<span data-ttu-id="64aa0-711">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="64aa0-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="64aa0-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="64aa0-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="64aa0-713">Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="64aa0-714">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="64aa0-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="64aa0-715">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="64aa0-716">Девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="64aa0-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="64aa0-717">Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="64aa0-718">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной заГрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="64aa0-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="64aa0-719">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="64aa0-720">Девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="64aa0-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="64aa0-721">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-721">Boolean</span></span>|<span data-ttu-id="64aa0-722">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="64aa0-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="64aa0-723">Девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="64aa0-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="64aa0-724">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-724">Boolean</span></span>|<span data-ttu-id="64aa0-725">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="64aa0-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="64aa0-726">Девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="64aa0-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="64aa0-727">Включение</span><span class="sxs-lookup"><span data-stu-id="64aa0-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="64aa0-728">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="64aa0-729">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="64aa0-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="64aa0-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="64aa0-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-731">Boolean</span></span>|<span data-ttu-id="64aa0-732">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="64aa0-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="64aa0-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="64aa0-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="64aa0-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-734">Boolean</span></span>|<span data-ttu-id="64aa0-735">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="64aa0-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="64aa0-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="64aa0-736">applicationGuardEnabled</span></span>|<span data-ttu-id="64aa0-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-737">Boolean</span></span>|<span data-ttu-id="64aa0-738">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="64aa0-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="64aa0-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="64aa0-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="64aa0-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="64aa0-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="64aa0-741">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="64aa0-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="64aa0-742">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="64aa0-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="64aa0-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="64aa0-744">Аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="64aa0-745">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="64aa0-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="64aa0-746">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="64aa0-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="64aa0-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="64aa0-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-748">Boolean</span></span>|<span data-ttu-id="64aa0-749">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="64aa0-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="64aa0-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="64aa0-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="64aa0-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-751">Boolean</span></span>|<span data-ttu-id="64aa0-752">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="64aa0-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="64aa0-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="64aa0-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="64aa0-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-754">Boolean</span></span>|<span data-ttu-id="64aa0-755">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="64aa0-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="64aa0-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="64aa0-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="64aa0-757">Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="64aa0-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="64aa0-758">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="64aa0-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="64aa0-759">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="64aa0-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="64aa0-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="64aa0-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="64aa0-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-761">Boolean</span></span>|<span data-ttu-id="64aa0-762">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="64aa0-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="64aa0-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="64aa0-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-764">Boolean</span></span>|<span data-ttu-id="64aa0-765">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="64aa0-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="64aa0-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="64aa0-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-767">Boolean</span></span>|<span data-ttu-id="64aa0-768">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="64aa0-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="64aa0-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="64aa0-770">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-770">Boolean</span></span>|<span data-ttu-id="64aa0-771">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="64aa0-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="64aa0-772">Аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="64aa0-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="64aa0-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-773">Boolean</span></span>|<span data-ttu-id="64aa0-774">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="64aa0-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="64aa0-775">Аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="64aa0-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="64aa0-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-776">Boolean</span></span>|<span data-ttu-id="64aa0-777">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="64aa0-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="64aa0-778">Битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="64aa0-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="64aa0-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-779">Boolean</span></span>|<span data-ttu-id="64aa0-780">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время приСоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="64aa0-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="64aa0-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="64aa0-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="64aa0-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-782">Boolean</span></span>|<span data-ttu-id="64aa0-783">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="64aa0-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="64aa0-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="64aa0-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="64aa0-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-785">Boolean</span></span>|<span data-ttu-id="64aa0-786">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="64aa0-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="64aa0-787">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="64aa0-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="64aa0-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="64aa0-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="64aa0-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="64aa0-789">Boolean</span></span>|<span data-ttu-id="64aa0-790">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="64aa0-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="64aa0-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="64aa0-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="64aa0-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="64aa0-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="64aa0-793">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="64aa0-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="64aa0-794">bitLockerFixedDrivePolicy;</span><span class="sxs-lookup"><span data-stu-id="64aa0-794">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="64aa0-795">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="64aa0-795">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="64aa0-796">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="64aa0-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="64aa0-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="64aa0-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="64aa0-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="64aa0-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="64aa0-799">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="64aa0-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="64aa0-800">Отклик</span><span class="sxs-lookup"><span data-stu-id="64aa0-800">Response</span></span>
<span data-ttu-id="64aa0-801">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64aa0-801">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64aa0-802">Пример</span><span class="sxs-lookup"><span data-stu-id="64aa0-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="64aa0-803">Запрос</span><span class="sxs-lookup"><span data-stu-id="64aa0-803">Request</span></span>
<span data-ttu-id="64aa0-804">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64aa0-804">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 27641

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
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="64aa0-805">Отклик</span><span class="sxs-lookup"><span data-stu-id="64aa0-805">Response</span></span>
<span data-ttu-id="64aa0-p199">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64aa0-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 27813

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
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
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




