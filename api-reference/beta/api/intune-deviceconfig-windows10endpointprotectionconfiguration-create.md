---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bdc31fed7797a448239bc7ed19ac57750692646
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402589"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="84803-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="84803-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="84803-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84803-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84803-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84803-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84803-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84803-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84803-107">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84803-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="84803-108">Prerequisites</span></span>
<span data-ttu-id="84803-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84803-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84803-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84803-111">Permission type</span></span>|<span data-ttu-id="84803-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84803-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84803-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84803-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84803-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84803-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84803-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84803-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84803-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84803-116">Not supported.</span></span>|
|<span data-ttu-id="84803-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84803-117">Application</span></span>|<span data-ttu-id="84803-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84803-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84803-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84803-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84803-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84803-120">Request headers</span></span>
|<span data-ttu-id="84803-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84803-121">Header</span></span>|<span data-ttu-id="84803-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84803-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84803-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84803-123">Authorization</span></span>|<span data-ttu-id="84803-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84803-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84803-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84803-125">Accept</span></span>|<span data-ttu-id="84803-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84803-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84803-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84803-127">Request body</span></span>
<span data-ttu-id="84803-128">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84803-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="84803-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84803-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="84803-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84803-130">Property</span></span>|<span data-ttu-id="84803-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84803-131">Type</span></span>|<span data-ttu-id="84803-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84803-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84803-133">id</span><span class="sxs-lookup"><span data-stu-id="84803-133">id</span></span>|<span data-ttu-id="84803-134">String</span><span class="sxs-lookup"><span data-stu-id="84803-134">String</span></span>|<span data-ttu-id="84803-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84803-135">Key of the entity.</span></span> <span data-ttu-id="84803-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84803-137">lastModifiedDateTime</span></span>|<span data-ttu-id="84803-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84803-138">DateTimeOffset</span></span>|<span data-ttu-id="84803-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="84803-139">DateTime the object was last modified.</span></span> <span data-ttu-id="84803-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84803-141">roleScopeTagIds</span></span>|<span data-ttu-id="84803-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84803-142">String collection</span></span>|<span data-ttu-id="84803-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="84803-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84803-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84803-145">supportsScopeTags</span></span>|<span data-ttu-id="84803-146">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-146">Boolean</span></span>|<span data-ttu-id="84803-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="84803-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84803-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="84803-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84803-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="84803-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84803-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84803-150">This property is read-only.</span></span> <span data-ttu-id="84803-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84803-152">createdDateTime</span></span>|<span data-ttu-id="84803-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84803-153">DateTimeOffset</span></span>|<span data-ttu-id="84803-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="84803-154">DateTime the object was created.</span></span> <span data-ttu-id="84803-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-156">description</span><span class="sxs-lookup"><span data-stu-id="84803-156">description</span></span>|<span data-ttu-id="84803-157">String</span><span class="sxs-lookup"><span data-stu-id="84803-157">String</span></span>|<span data-ttu-id="84803-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84803-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84803-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-160">displayName</span><span class="sxs-lookup"><span data-stu-id="84803-160">displayName</span></span>|<span data-ttu-id="84803-161">String</span><span class="sxs-lookup"><span data-stu-id="84803-161">String</span></span>|<span data-ttu-id="84803-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84803-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84803-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-164">version</span><span class="sxs-lookup"><span data-stu-id="84803-164">version</span></span>|<span data-ttu-id="84803-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84803-165">Int32</span></span>|<span data-ttu-id="84803-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84803-166">Version of the device configuration.</span></span> <span data-ttu-id="84803-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84803-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84803-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="84803-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="84803-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="84803-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="84803-170">Эта политика предназначена для обеспечения повышенной безопасности для внешних устройств с поддержкой DMA.</span><span class="sxs-lookup"><span data-stu-id="84803-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="84803-171">Она позволяет лучше контролировать перечисление внешних устройств с поддержкой DMA несовместимым с DMA Remapping и устройства памяти изоляции и "песочницы".</span><span class="sxs-lookup"><span data-stu-id="84803-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="84803-172">Эта политика только вступает в силу при включены встроенного по и поддерживаются защиты DMA ядра.</span><span class="sxs-lookup"><span data-stu-id="84803-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="84803-173">Защита от DMA ядра — это платформа функциональная возможность, которая не может управляться с помощью политики или конечный пользователь.</span><span class="sxs-lookup"><span data-stu-id="84803-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="84803-174">Он должен поддерживаться системой во время производства.</span><span class="sxs-lookup"><span data-stu-id="84803-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="84803-175">Чтобы проверить, поддерживает ли система защиты DMA ядра, проверьте защиты DMA ядра поля на странице сводки MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="84803-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="84803-176">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="84803-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="84803-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="84803-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="84803-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-179">Это право используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="84803-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="84803-180">Сохраненные учетные данные пользователей могут быть раскрыты, если эта привилегия предоставляется другим лицам.</span><span class="sxs-lookup"><span data-stu-id="84803-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="84803-181">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="84803-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="84803-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-184">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="84803-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="84803-185">Поддерживается состояний разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="84803-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="84803-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="84803-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-188">Это право пользователя определяет, какие пользователи и группы, блока из подключение к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="84803-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="84803-189">Поддерживаемые состояния блокировки.</span><span class="sxs-lookup"><span data-stu-id="84803-189">State Block is supported.</span></span>|
|<span data-ttu-id="84803-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="84803-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="84803-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-192">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="84803-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="84803-193">Процесс таким образом можно получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="84803-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="84803-194">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="84803-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="84803-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-197">Это право пользователя определяет, какие пользователи могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="84803-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="84803-198">NotConfigured состояниях, разрешенные и заблокированные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="84803-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="84803-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="84803-199">userRightsBackupData</span></span>|[<span data-ttu-id="84803-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-201">Это право пользователя определяет пользователей, которые могут обойти файлов, каталогов, реестра и другие разрешения постоянные объекты при резервном копировании файлов и папок.</span><span class="sxs-lookup"><span data-stu-id="84803-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="84803-202">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="84803-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="84803-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-205">Это право пользователя определяет, какие пользователи и группы можно изменить время и дату на внутренних часов компьютера.</span><span class="sxs-lookup"><span data-stu-id="84803-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="84803-206">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="84803-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="84803-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-209">Этот параметр безопасности определяет, будет ли пользователи могут создавать глобальные объекты, которые доступны для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="84803-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="84803-210">Пользователи, создающие глобальных объектов может повлиять на процессы, которые выполняются в разделе сеансов другим пользователям, что может привести к повреждению данных или сбой приложения.</span><span class="sxs-lookup"><span data-stu-id="84803-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="84803-211">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="84803-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="84803-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-214">Это право пользователя определяет, какие пользователи и группы можно вызвать внутренним API для создания и изменения размера файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="84803-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="84803-215">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="84803-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="84803-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-218">Это право пользователя определяет, какие учетные записи можно использовать с процессами для создания объекта каталога с помощью объекта диспетчера.</span><span class="sxs-lookup"><span data-stu-id="84803-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="84803-219">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="84803-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="84803-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-222">Это право пользователя определяет, если пользователь может создавать символьной ссылки с компьютера, на который входе в систему.</span><span class="sxs-lookup"><span data-stu-id="84803-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="84803-223">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="84803-224">userRightsCreateToken</span></span>|[<span data-ttu-id="84803-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-226">Это право пользователя определяет, какие пользователи и группы можно использовать для процессов для создания маркер, который можно использовать для получения доступа к любым локальным ресурсам, если процесс использует внутренний интерфейс API для создания маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="84803-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="84803-227">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="84803-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="84803-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-230">Это право пользователя определяет, какие пользователи могут запускать программу отладки для любого процесса или ядра.</span><span class="sxs-lookup"><span data-stu-id="84803-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="84803-231">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="84803-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="84803-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="84803-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="84803-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-234">Это право пользователя определяет, какие пользователи и группы, не могут входить в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="84803-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="84803-235">Поддерживаются только состояния NotConfigured и заблокированные</span><span class="sxs-lookup"><span data-stu-id="84803-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="84803-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="84803-236">userRightsDelegation</span></span>|[<span data-ttu-id="84803-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-238">Это право пользователя определяет, какие пользователи могут устанавливать доверие для делегирования в объекте пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="84803-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="84803-239">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="84803-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="84803-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-242">Это право пользователя определяет, какие учетные записи можно использовать процессом для добавления записей в журнале безопасности.</span><span class="sxs-lookup"><span data-stu-id="84803-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="84803-243">Журнал безопасности используется для отслеживания несанкционированного доступа в систему.</span><span class="sxs-lookup"><span data-stu-id="84803-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="84803-244">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="84803-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="84803-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-247">Назначение это право пользователя позволяет программам, выполняемым от имени этого пользователя для олицетворения клиента.</span><span class="sxs-lookup"><span data-stu-id="84803-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="84803-248">Использование этого права пользователя для этого вида олицетворения не позволяет неавторизованных пользователей в качестве клиента для подключения к службе, если они были созданы и затем олицетворить клиента, который может повысить неавторизованных пользователей разрешения на административные или системного уровня.</span><span class="sxs-lookup"><span data-stu-id="84803-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="84803-249">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="84803-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="84803-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-252">Это право пользователя определяет, какие учетные записи могут использовать процесс записать свойство доступа к другим процессом для увеличения приоритета выполнения, назначенного для других процессов.</span><span class="sxs-lookup"><span data-stu-id="84803-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="84803-253">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="84803-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="84803-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-256">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="84803-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="84803-257">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="84803-258">userRightsLockMemory</span></span>|[<span data-ttu-id="84803-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-260">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, запрещающий подкачки страниц в виртуальной памяти на диске.</span><span class="sxs-lookup"><span data-stu-id="84803-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="84803-261">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="84803-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="84803-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-264">Это право пользователя определяет, какие пользователи могут задавать доступ к объекту параметров аудита для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="84803-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="84803-265">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="84803-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="84803-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-268">Это право пользователя определяет, какие пользователи и группы можно выполнять задачи по обслуживанию тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="84803-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="84803-269">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="84803-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="84803-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-272">Право определяет, кто может изменять параметры среды оборудования.</span><span class="sxs-lookup"><span data-stu-id="84803-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="84803-273">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="84803-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="84803-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-276">Это право пользователя определяет, какие учетные записи пользователей можно изменять метки целостности объектов, например файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="84803-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="84803-277">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="84803-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="84803-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-280">Это право пользователя определяет пользователей, которые можно использовать средства мониторинга производительности для отслеживания производительности системных процессов.</span><span class="sxs-lookup"><span data-stu-id="84803-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="84803-281">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="84803-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="84803-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-284">Это право пользователя определяет, какие пользователи могут завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="84803-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="84803-285">Неправильное использование этого права пользователя может привести отказ в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="84803-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="84803-286">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="84803-287">userRightsRestoreData</span></span>|[<span data-ttu-id="84803-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-289">Это право пользователя определяет, какие пользователи могут файла, каталога, реестра и другие постоянные объекты разрешений при восстановлении резервных копий файлов и папок, а также определяет пользователей, которые можно назначить любого действительного участника безопасности владельцем объекта.</span><span class="sxs-lookup"><span data-stu-id="84803-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="84803-290">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="84803-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="84803-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-293">Это право пользователя определяет, какие пользователи могут стать владельцами любого защищаемого объекта в системе, в том числе объектов Active Directory, файлов и папок, принтеров, разделов реестра, процессов и потоков.</span><span class="sxs-lookup"><span data-stu-id="84803-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="84803-294">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="84803-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="84803-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="84803-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="84803-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="84803-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="84803-297">Этот параметр безопасности определяет, какие учетные записи служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="84803-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="84803-298">Примечание: Этот параметр безопасности не применяется к учетным записям системы, сетевая служба или локальная служба.</span><span class="sxs-lookup"><span data-stu-id="84803-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="84803-299">Поддерживается только состояние заблокирован.</span><span class="sxs-lookup"><span data-stu-id="84803-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="84803-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="84803-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="84803-301">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-301">Boolean</span></span>|<span data-ttu-id="84803-302">Этот параметр определяет, является ли сохранить игры xbox включено (1) или отключено (0).</span><span class="sxs-lookup"><span data-stu-id="84803-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="84803-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="84803-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="84803-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="84803-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="84803-305">Этот параметр определяет, является ли тип запуска службы управления стандартную программу Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="84803-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="84803-306">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="84803-306">Default: Manual.</span></span> <span data-ttu-id="84803-307">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="84803-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="84803-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="84803-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="84803-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="84803-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="84803-310">Этот параметр определяет, является ли тип запуска службы Live диспетчера проверкой подлинности на основе Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="84803-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="84803-311">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="84803-311">Default: Manual.</span></span> <span data-ttu-id="84803-312">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="84803-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="84803-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="84803-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="84803-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="84803-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="84803-315">Этот параметр определяет, является ли Live игру сохранить тип запуска службы Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="84803-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="84803-316">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="84803-316">Default: Manual.</span></span> <span data-ttu-id="84803-317">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="84803-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="84803-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="84803-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="84803-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="84803-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="84803-320">Этот параметр определяет, является ли тип запуска службы сети Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="84803-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="84803-321">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="84803-321">Default: Manual.</span></span> <span data-ttu-id="84803-322">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="84803-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="84803-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="84803-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="84803-324">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-324">Boolean</span></span>|<span data-ttu-id="84803-325">Запретить пользователям добавление новых учетных записей Майкрософт для этого компьютера.</span><span class="sxs-lookup"><span data-stu-id="84803-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="84803-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="84803-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="84803-327">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-327">Boolean</span></span>|<span data-ttu-id="84803-328">Включение локальных учетных записей, которые не являются войти в систему из мест, отличных от физическое устройство защищены паролем. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="84803-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="84803-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="84803-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="84803-330">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-330">Boolean</span></span>|<span data-ttu-id="84803-331">Определяет, включена ли учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="84803-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="84803-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="84803-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="84803-333">String</span><span class="sxs-lookup"><span data-stu-id="84803-333">String</span></span>|<span data-ttu-id="84803-334">Определите имя другой учетной записи необходимо сопоставить с идентификатором безопасности (SID) для учетной записи «Администратор».</span><span class="sxs-lookup"><span data-stu-id="84803-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="84803-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="84803-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="84803-336">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-336">Boolean</span></span>|<span data-ttu-id="84803-337">Определяет, включен ли гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="84803-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="84803-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="84803-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="84803-339">String</span><span class="sxs-lookup"><span data-stu-id="84803-339">String</span></span>|<span data-ttu-id="84803-340">Определите имя другой учетной записи необходимо сопоставить с идентификатором безопасности (SID) для учетной записи «Гость».</span><span class="sxs-lookup"><span data-stu-id="84803-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="84803-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="84803-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="84803-342">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-342">Boolean</span></span>|<span data-ttu-id="84803-343">Запретить портативных компьютеров извлечения без необходимости входа.</span><span class="sxs-lookup"><span data-stu-id="84803-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="84803-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="84803-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="84803-345">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-345">Boolean</span></span>|<span data-ttu-id="84803-346">Следует ограничьте Установка драйверов принтера как часть подключение к принтеру только администраторам.</span><span class="sxs-lookup"><span data-stu-id="84803-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="84803-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="84803-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="84803-348">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-348">Boolean</span></span>|<span data-ttu-id="84803-349">Включение этот параметр позволяет только интерактивно пользователя для доступа к компакт-диска носителя.</span><span class="sxs-lookup"><span data-stu-id="84803-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="84803-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="84803-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="84803-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="84803-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="84803-352">Определите, кому разрешено форматирование и извлечение съемных носителей файловой системы NTFS.</span><span class="sxs-lookup"><span data-stu-id="84803-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="84803-353">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="84803-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="84803-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="84803-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="84803-355">Int32</span><span class="sxs-lookup"><span data-stu-id="84803-355">Int32</span></span>|<span data-ttu-id="84803-356">Определите максимальное число минут бездействия пользователя на экране входа в систему интерактивного рабочего стола до запуска заставки экрана.</span><span class="sxs-lookup"><span data-stu-id="84803-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="84803-357">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="84803-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="84803-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="84803-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="84803-359">Int32</span><span class="sxs-lookup"><span data-stu-id="84803-359">Int32</span></span>|<span data-ttu-id="84803-360">Определите максимальное число минут бездействия пользователя на экране входа в систему интерактивного рабочего стола до запуска заставки экрана.</span><span class="sxs-lookup"><span data-stu-id="84803-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="84803-361">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="84803-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="84803-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="84803-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="84803-363">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-363">Boolean</span></span>|<span data-ttu-id="84803-364">Требуется сочетание клавиш CTRL + ALT + DEL нажатие, прежде чем пользователь сможет войти.</span><span class="sxs-lookup"><span data-stu-id="84803-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="84803-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="84803-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="84803-366">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-366">Boolean</span></span>|<span data-ttu-id="84803-367">Не отображать username последнего человека, который в системе на это устройство.</span><span class="sxs-lookup"><span data-stu-id="84803-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="84803-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="84803-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="84803-369">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-369">Boolean</span></span>|<span data-ttu-id="84803-370">Не отображать имя пользователя человека, вход в это устройство после ввода учетных данных и перед отображением рабочий стол устройства.</span><span class="sxs-lookup"><span data-stu-id="84803-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="84803-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="84803-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="84803-372">String</span><span class="sxs-lookup"><span data-stu-id="84803-372">String</span></span>|<span data-ttu-id="84803-373">Задайте заголовок сообщения для пользователей при входе в.</span><span class="sxs-lookup"><span data-stu-id="84803-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="84803-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="84803-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="84803-375">String</span><span class="sxs-lookup"><span data-stu-id="84803-375">String</span></span>|<span data-ttu-id="84803-376">Задайте текст сообщения для пользователей при входе в.</span><span class="sxs-lookup"><span data-stu-id="84803-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="84803-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="84803-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="84803-378">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-378">Boolean</span></span>|<span data-ttu-id="84803-379">Блок PKU2U запросы проверки подлинности для этого устройства для использования online удостоверения.</span><span class="sxs-lookup"><span data-stu-id="84803-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="84803-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="84803-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="84803-381">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-381">Boolean</span></span>|<span data-ttu-id="84803-382">Пользовательский Интерфейс вспомогательных логическое для сущности LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="84803-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="84803-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="84803-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="84803-384">String</span><span class="sxs-lookup"><span data-stu-id="84803-384">String</span></span>|<span data-ttu-id="84803-385">Измените строку языке по умолчанию, которую нужно разрешить или запретить пользователей и групп для удаленных вызовов для SAM.</span><span class="sxs-lookup"><span data-stu-id="84803-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="84803-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="84803-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="84803-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="84803-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="84803-388">Этот параметр безопасности позволяет клиенту требовать согласования 128-битового шифрования и/или безопасность сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="84803-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="84803-389">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="84803-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="84803-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="84803-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="84803-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="84803-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="84803-392">Этот параметр безопасности позволяет серверу требовать согласования 128-битового шифрования и/или безопасность сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="84803-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="84803-393">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="84803-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="84803-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="84803-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="84803-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="84803-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="84803-396">Этот параметр безопасности определяет, какой протокол проверки подлинности на запрос и ответ используется для регистрации в сети.</span><span class="sxs-lookup"><span data-stu-id="84803-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="84803-397">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="84803-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="84803-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="84803-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="84803-399">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-399">Boolean</span></span>|<span data-ttu-id="84803-400">Если этот параметр включен, клиент SMB позволяет уязвимость гостевые входы в систему.</span><span class="sxs-lookup"><span data-stu-id="84803-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="84803-401">Если не настроена, клиент SMB будет отклонить уязвимость гостевые входы в систему.</span><span class="sxs-lookup"><span data-stu-id="84803-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="84803-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="84803-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="84803-403">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-403">Boolean</span></span>|<span data-ttu-id="84803-404">Этот параметр безопасности определяет снят ли файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="84803-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="84803-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="84803-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="84803-406">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-406">Boolean</span></span>|<span data-ttu-id="84803-407">Этот параметр безопасности определяет, можно ли завершать работу компьютера, без необходимости входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="84803-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="84803-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="84803-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="84803-409">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-409">Boolean</span></span>|<span data-ttu-id="84803-410">Разрешить UIAccess приложения запрашивать повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="84803-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="84803-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="84803-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="84803-412">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-412">Boolean</span></span>|<span data-ttu-id="84803-413">Виртуализация файлов и реестра неудачных операций записи для каждого пользователя расположения</span><span class="sxs-lookup"><span data-stu-id="84803-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="84803-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="84803-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="84803-415">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-415">Boolean</span></span>|<span data-ttu-id="84803-416">Принудительное применение проверки путь сертификации PKI для указанного исполняемого файла перед разрешением на выполнение.</span><span class="sxs-lookup"><span data-stu-id="84803-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="84803-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="84803-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="84803-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="84803-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="84803-419">Определите поведение запроса на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="84803-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="84803-420">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="84803-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="84803-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="84803-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="84803-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="84803-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="84803-423">Определите поведение запроса на повышение прав для обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="84803-424">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="84803-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="84803-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="84803-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="84803-426">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-426">Boolean</span></span>|<span data-ttu-id="84803-427">Включите все запросы на повышение прав переход на рабочем столе интерактивного пользователя, а не защищенного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="84803-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="84803-428">Используются параметры политики вывода запросов для администраторов и обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="84803-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="84803-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="84803-430">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-430">Boolean</span></span>|<span data-ttu-id="84803-431">Установка приложения, которых необходимо будет запрашивать учетные данные администратора. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="84803-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="84803-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="84803-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="84803-433">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-433">Boolean</span></span>|<span data-ttu-id="84803-434">Разрешить UIAccess приложения запрашивать повышение прав без использования безопасного рабочего стола. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="84803-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="84803-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="84803-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="84803-436">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-436">Boolean</span></span>|<span data-ttu-id="84803-437">Определяет ли учетная запись администратора; встроенных использует режиме одобрения администратором или запускает все приложения с правами полного администрирования. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="84803-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="84803-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="84803-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="84803-439">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-439">Boolean</span></span>|<span data-ttu-id="84803-440">Определение в режиме одобрения администратором и все параметры политики контроля учетных Записей, включены ли, включены по умолчанию</span><span class="sxs-lookup"><span data-stu-id="84803-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="84803-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="84803-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="84803-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="84803-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="84803-443">Настройка сведений о пользователе, которое отображается при сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="84803-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="84803-444">Если не настроен, показаны отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="84803-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="84803-445">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="84803-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="84803-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="84803-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="84803-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="84803-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="84803-448">Настройка сведений о пользователе, которое отображается при сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="84803-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="84803-449">Если не настроен, показаны отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="84803-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="84803-450">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="84803-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="84803-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="84803-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="84803-452">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-452">Boolean</span></span>|<span data-ttu-id="84803-453">Этот параметр безопасности определяет, пытается ли SMB-клиент согласовать подписи SMB-пакетов.</span><span class="sxs-lookup"><span data-stu-id="84803-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="84803-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="84803-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="84803-455">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-455">Boolean</span></span>|<span data-ttu-id="84803-456">Этот параметр безопасности определяет, требуется подпись пакетов SMB-компоненты клиента.</span><span class="sxs-lookup"><span data-stu-id="84803-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="84803-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="84803-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="84803-458">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-458">Boolean</span></span>|<span data-ttu-id="84803-459">Если включен этот параметр безопасности, перенаправитель блок SMB (Server Message) разрешено отправлять пароли открытым текстом на серверы SMB сторонних разработчиков, которые не поддерживают шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="84803-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="84803-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="84803-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="84803-461">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-461">Boolean</span></span>|<span data-ttu-id="84803-462">Этот параметр безопасности определяет, требуется подпись пакетов SMB-компоненты сервера.</span><span class="sxs-lookup"><span data-stu-id="84803-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="84803-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="84803-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="84803-464">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-464">Boolean</span></span>|<span data-ttu-id="84803-465">Этот параметр безопасности определяет, будет ли SMB-сервер согласовывать подписи с их клиенты SMB-пакетов.</span><span class="sxs-lookup"><span data-stu-id="84803-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="84803-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="84803-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="84803-467">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-467">Boolean</span></span>|<span data-ttu-id="84803-468">По умолчанию этот параметр безопасности ограничивает анонимный доступ к общим папкам и каналы для параметров для именованных каналов, доступных анонимным и общих папок, которые могут быть анонимный доступ к</span><span class="sxs-lookup"><span data-stu-id="84803-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="84803-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="84803-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="84803-470">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-470">Boolean</span></span>|<span data-ttu-id="84803-471">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключение к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="84803-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="84803-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="84803-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="84803-473">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-473">Boolean</span></span>|<span data-ttu-id="84803-474">Этот параметр безопасности определяет, следует ли анонимные пользователи могут выполнять определенные операции, такие как перечисление имен учетных записей домена и сетевых папок.</span><span class="sxs-lookup"><span data-stu-id="84803-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="84803-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="84803-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="84803-476">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-476">Boolean</span></span>|<span data-ttu-id="84803-477">Этот параметр безопасности определяет, если при следующей смене пароля хранятся значения хэш-функции LAN Manager (LM) для нового пароля.</span><span class="sxs-lookup"><span data-stu-id="84803-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="84803-478">По умолчанию не хранятся.</span><span class="sxs-lookup"><span data-stu-id="84803-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="84803-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="84803-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="84803-480">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="84803-480">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="84803-481">Этот параметр безопасности определяет, что происходит при удалении смарт-карт для пользователя, вошедшего в систему с смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="84803-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="84803-482">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="84803-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="84803-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="84803-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="84803-484">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-484">Boolean</span></span>|<span data-ttu-id="84803-485">Используется для отключения отображения области защиты приложений и веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="84803-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="84803-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="84803-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="84803-487">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-487">Boolean</span></span>|<span data-ttu-id="84803-488">Используется для отключения отображения области семейства параметров.</span><span class="sxs-lookup"><span data-stu-id="84803-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="84803-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="84803-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="84803-490">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-490">Boolean</span></span>|<span data-ttu-id="84803-491">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="84803-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="84803-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="84803-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="84803-493">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-493">Boolean</span></span>|<span data-ttu-id="84803-494">Используется для отключения отображения области защиты брандмауэра и сети.</span><span class="sxs-lookup"><span data-stu-id="84803-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="84803-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="84803-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="84803-496">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-496">Boolean</span></span>|<span data-ttu-id="84803-497">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="84803-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="84803-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="84803-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="84803-499">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-499">Boolean</span></span>|<span data-ttu-id="84803-500">Используется для отключения отображения области защиты учетной записи.</span><span class="sxs-lookup"><span data-stu-id="84803-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="84803-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="84803-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="84803-502">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-502">Boolean</span></span>|<span data-ttu-id="84803-503">Используется для отключения отображения области защиты оборудования.</span><span class="sxs-lookup"><span data-stu-id="84803-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="84803-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="84803-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="84803-505">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-505">Boolean</span></span>|<span data-ttu-id="84803-506">Используется для отключения отображения области ransomware защиты.</span><span class="sxs-lookup"><span data-stu-id="84803-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="84803-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="84803-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="84803-508">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-508">Boolean</span></span>|<span data-ttu-id="84803-509">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройств.</span><span class="sxs-lookup"><span data-stu-id="84803-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="84803-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="84803-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="84803-511">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-511">Boolean</span></span>|<span data-ttu-id="84803-512">Используется для отключения отображения процесса обеспечения безопасности, устранение неполадок в разделе Безопасность устройств.</span><span class="sxs-lookup"><span data-stu-id="84803-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="84803-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="84803-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="84803-514">String</span><span class="sxs-lookup"><span data-stu-id="84803-514">String</span></span>|<span data-ttu-id="84803-515">Имя компании, которая отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="84803-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="84803-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="84803-517">String</span><span class="sxs-lookup"><span data-stu-id="84803-517">String</span></span>|<span data-ttu-id="84803-518">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="84803-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="84803-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="84803-520">String</span><span class="sxs-lookup"><span data-stu-id="84803-520">String</span></span>|<span data-ttu-id="84803-521">Номер телефона или Скайп код, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="84803-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="84803-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="84803-523">String</span><span class="sxs-lookup"><span data-stu-id="84803-523">String</span></span>|<span data-ttu-id="84803-524">Портал справки URL-адрес, оно отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="84803-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="84803-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="84803-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="84803-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="84803-527">Уведомления для отображения из отображаемой области приложения.</span><span class="sxs-lookup"><span data-stu-id="84803-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="84803-528">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="84803-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="84803-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="84803-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="84803-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="84803-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="84803-531">Настройка места отображения контактов ИТ сведения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="84803-532">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="84803-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="84803-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="84803-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="84803-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-534">Boolean</span></span>|<span data-ttu-id="84803-535">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="84803-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="84803-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="84803-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="84803-537">Int32</span><span class="sxs-lookup"><span data-stu-id="84803-537">Int32</span></span>|<span data-ttu-id="84803-538">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="84803-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="84803-539">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="84803-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="84803-540">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="84803-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="84803-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="84803-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="84803-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="84803-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="84803-543">Выберите предварительный ключ, кодировка для использования.</span><span class="sxs-lookup"><span data-stu-id="84803-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="84803-544">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="84803-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="84803-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="84803-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="84803-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-546">Boolean</span></span>|<span data-ttu-id="84803-547">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="84803-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="84803-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="84803-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="84803-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-549">Boolean</span></span>|<span data-ttu-id="84803-550">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="84803-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="84803-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="84803-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="84803-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-552">Boolean</span></span>|<span data-ttu-id="84803-553">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="84803-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="84803-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="84803-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="84803-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-555">Boolean</span></span>|<span data-ttu-id="84803-556">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="84803-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="84803-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="84803-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="84803-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="84803-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="84803-559">Укажите, как быть реализовано списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="84803-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="84803-560">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="84803-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="84803-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="84803-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="84803-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-562">Boolean</span></span>|<span data-ttu-id="84803-563">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="84803-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="84803-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="84803-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="84803-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="84803-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="84803-566">Настраивает применения пакетов очередей в сценарии туннель шлюза.</span><span class="sxs-lookup"><span data-stu-id="84803-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="84803-567">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="84803-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="84803-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="84803-568">firewallProfileDomain</span></span>|[<span data-ttu-id="84803-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="84803-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="84803-570">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="84803-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="84803-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="84803-571">firewallProfilePublic</span></span>|[<span data-ttu-id="84803-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="84803-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="84803-573">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="84803-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="84803-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="84803-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="84803-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="84803-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="84803-576">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="84803-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="84803-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="84803-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="84803-578">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84803-578">String collection</span></span>|<span data-ttu-id="84803-579">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="84803-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="84803-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="84803-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="84803-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-582">Значение, указывающее, поведение приложений Office, добавление в других процессов.</span><span class="sxs-lookup"><span data-stu-id="84803-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="84803-583">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="84803-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="84803-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-586">Значение, указывающее, поведение приложений Office, добавление в других процессов.</span><span class="sxs-lookup"><span data-stu-id="84803-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="84803-587">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="84803-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="84803-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-590">Значение, указывающее, поведение приложений/макросов Office Создание и запуск исполняемым содержимым.</span><span class="sxs-lookup"><span data-stu-id="84803-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="84803-591">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="84803-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="84803-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-594">Значение, указывающее, поведение приложений/макросов Office Создание и запуск исполняемым содержимым.</span><span class="sxs-lookup"><span data-stu-id="84803-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="84803-595">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="84803-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="84803-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-598">Значение, указывающее, поведение приложение Office для запуска дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="84803-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="84803-599">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="84803-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="84803-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-602">Значение, указывающее, поведение приложение Office для запуска дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="84803-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="84803-603">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="84803-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="84803-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-606">Значение, указывающее, поведение Win32 импортируется из код макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="84803-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="84803-607">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="84803-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="84803-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-610">Значение, указывающее, поведение Win32 импортируется из код макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="84803-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="84803-611">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="84803-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="84803-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-614">Значение, указывающее, поведение затемненные js/vbs/ps/макроса.</span><span class="sxs-lookup"><span data-stu-id="84803-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="84803-615">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="84803-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="84803-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-618">Значение, указывающее, поведение затемненные js/vbs/ps/макроса.</span><span class="sxs-lookup"><span data-stu-id="84803-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="84803-619">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="84803-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="84803-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-622">Значение, указывающее, поведение js/vbs выполнения полезных данных загружен из Интернета.</span><span class="sxs-lookup"><span data-stu-id="84803-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="84803-623">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="84803-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="84803-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-626">Значение, указывающее, поведение js/vbs выполнения полезных данных загружен из Интернета.</span><span class="sxs-lookup"><span data-stu-id="84803-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="84803-627">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="84803-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="84803-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-630">Значение, указывающее, если разрешен учетных данных, переноса из центра сертификации подсистемы локальной безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="84803-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="84803-631">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="84803-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="84803-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-634">Значение, указывающее ответ на создание процесса, поступающих из команды PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="84803-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="84803-635">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="84803-636">defenderProcessCreation</span></span>|[<span data-ttu-id="84803-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-638">Значение, указывающее ответ на создание процесса, поступающих из команды PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="84803-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="84803-639">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="84803-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="84803-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-642">Значение, указывающее ответ на процессы ненадежные и без знака, на которых выполняется через порт USB.</span><span class="sxs-lookup"><span data-stu-id="84803-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="84803-643">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="84803-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="84803-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-646">Значение, указывающее ответ на процессы ненадежные и без знака, на которых выполняется через порт USB.</span><span class="sxs-lookup"><span data-stu-id="84803-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="84803-647">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="84803-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="84803-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-650">Значение, указывающее, ответ на исполняемые файлы, которые не соответствуют распространением домашних, срок хранения или список надежных критериев.</span><span class="sxs-lookup"><span data-stu-id="84803-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="84803-651">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="84803-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="84803-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-654">Значение, указывающее, ответ на исполняемые файлы, которые не соответствуют распространением домашних, срок хранения или список надежных критериев.</span><span class="sxs-lookup"><span data-stu-id="84803-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="84803-655">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="84803-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="84803-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="84803-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="84803-658">Значение, указывающее, если выполнение контента исполняемый файл (EXE-файл, DLL-библиотеку, ps, js, vbs, и т.д.) должны быть удалены из электронной почты (веб-почты/почты клиент).</span><span class="sxs-lookup"><span data-stu-id="84803-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="84803-659">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="84803-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="84803-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-662">Значение, указывающее, если выполнение контента исполняемый файл (EXE-файл, DLL-библиотеку, ps, js, vbs, и т.д.) должны быть удалены из электронной почты (веб-почты/почты клиент).</span><span class="sxs-lookup"><span data-stu-id="84803-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="84803-663">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="84803-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-666">Значение, указывающее, использование дополнительную защиту от ransomeware.</span><span class="sxs-lookup"><span data-stu-id="84803-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="84803-667">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="84803-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="84803-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="84803-670">Значение, указывающее, поведение защищенные папки.</span><span class="sxs-lookup"><span data-stu-id="84803-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="84803-671">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="84803-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="84803-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="84803-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="84803-673">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84803-673">String collection</span></span>|<span data-ttu-id="84803-674">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="84803-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="84803-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="84803-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="84803-676">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84803-676">String collection</span></span>|<span data-ttu-id="84803-677">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="84803-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="84803-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="84803-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="84803-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="84803-680">Значение, указывающее, поведение NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="84803-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="84803-681">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="84803-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="84803-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="84803-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="84803-683">Binary</span><span class="sxs-lookup"><span data-stu-id="84803-683">Binary</span></span>|<span data-ttu-id="84803-684">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="84803-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="84803-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="84803-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="84803-686">String</span><span class="sxs-lookup"><span data-stu-id="84803-686">String</span></span>|<span data-ttu-id="84803-687">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="84803-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="84803-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="84803-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="84803-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-689">Boolean</span></span>|<span data-ttu-id="84803-690">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="84803-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="84803-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="84803-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="84803-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="84803-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="84803-693">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="84803-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="84803-694">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="84803-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="84803-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="84803-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="84803-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="84803-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="84803-697">Включение защиты учетных данных, если платформа уровень безопасности с помощью Secure загрузки и виртуализации на основе безопасности включены.</span><span class="sxs-lookup"><span data-stu-id="84803-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="84803-698">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="84803-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="84803-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="84803-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="84803-700">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-700">Boolean</span></span>|<span data-ttu-id="84803-701">Включение виртуализации на основе Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="84803-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="84803-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="84803-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="84803-703">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-703">Boolean</span></span>|<span data-ttu-id="84803-704">Указывает, включена ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="84803-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="84803-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="84803-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="84803-706">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="84803-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="84803-707">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="84803-707">.md)</span></span>|<span data-ttu-id="84803-708">Позволяет ИТ-администратор для настройки запуска системы защиты.</span><span class="sxs-lookup"><span data-stu-id="84803-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="84803-709">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="84803-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="84803-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="84803-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="84803-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-711">Boolean</span></span>|<span data-ttu-id="84803-712">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="84803-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="84803-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="84803-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="84803-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-714">Boolean</span></span>|<span data-ttu-id="84803-715">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="84803-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="84803-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="84803-716">applicationGuardEnabled</span></span>|<span data-ttu-id="84803-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-717">Boolean</span></span>|<span data-ttu-id="84803-718">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="84803-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="84803-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="84803-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="84803-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="84803-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="84803-721">Включение защиты приложения Защитник Windows для новой сборки Windows.</span><span class="sxs-lookup"><span data-stu-id="84803-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="84803-722">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="84803-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="84803-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="84803-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="84803-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="84803-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="84803-725">Блокировать буфера обмена передача файла изображения, текстовый файл или ни один из них.</span><span class="sxs-lookup"><span data-stu-id="84803-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="84803-726">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="84803-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="84803-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="84803-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="84803-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-728">Boolean</span></span>|<span data-ttu-id="84803-729">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="84803-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="84803-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="84803-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="84803-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-731">Boolean</span></span>|<span data-ttu-id="84803-732">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="84803-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="84803-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="84803-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="84803-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-734">Boolean</span></span>|<span data-ttu-id="84803-735">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="84803-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="84803-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="84803-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="84803-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="84803-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="84803-738">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="84803-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="84803-739">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="84803-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="84803-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="84803-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="84803-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-741">Boolean</span></span>|<span data-ttu-id="84803-742">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="84803-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="84803-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="84803-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="84803-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-744">Boolean</span></span>|<span data-ttu-id="84803-745">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="84803-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="84803-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="84803-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="84803-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-747">Boolean</span></span>|<span data-ttu-id="84803-748">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="84803-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="84803-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="84803-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="84803-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-750">Boolean</span></span>|<span data-ttu-id="84803-751">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="84803-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="84803-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="84803-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="84803-753">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-753">Boolean</span></span>|<span data-ttu-id="84803-754">Разрешить безопасности приложения, чтобы использовать графического виртуальных Процессора</span><span class="sxs-lookup"><span data-stu-id="84803-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="84803-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="84803-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="84803-756">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-756">Boolean</span></span>|<span data-ttu-id="84803-757">Разрешить пользователям загружать файлы из пограничного сервера в контейнере guard приложения и сохранение их на узле файловой системы</span><span class="sxs-lookup"><span data-stu-id="84803-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="84803-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="84803-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="84803-759">Логический</span><span class="sxs-lookup"><span data-stu-id="84803-759">Boolean</span></span>|<span data-ttu-id="84803-760">Позволяет администраторам стандартные пользователи могут включить encrpytion во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84803-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="84803-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="84803-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="84803-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-762">Boolean</span></span>|<span data-ttu-id="84803-763">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="84803-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="84803-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="84803-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="84803-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-765">Boolean</span></span>|<span data-ttu-id="84803-766">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="84803-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="84803-767">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="84803-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="84803-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="84803-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="84803-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="84803-769">Boolean</span></span>|<span data-ttu-id="84803-770">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="84803-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="84803-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="84803-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="84803-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="84803-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="84803-773">Политика BitLocker системного диска.</span><span class="sxs-lookup"><span data-stu-id="84803-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="84803-774">bitLockerFixedDrivePolicy;</span><span class="sxs-lookup"><span data-stu-id="84803-774">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="84803-775">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="84803-775">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="84803-776">Предопределенная политика диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="84803-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="84803-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="84803-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="84803-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="84803-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="84803-779">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="84803-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="84803-780">Отклик</span><span class="sxs-lookup"><span data-stu-id="84803-780">Response</span></span>
<span data-ttu-id="84803-781">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="84803-781">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84803-782">Пример</span><span class="sxs-lookup"><span data-stu-id="84803-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="84803-783">Запрос</span><span class="sxs-lookup"><span data-stu-id="84803-783">Request</span></span>
<span data-ttu-id="84803-784">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84803-784">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26475

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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

### <a name="response"></a><span data-ttu-id="84803-785">Отклик</span><span class="sxs-lookup"><span data-stu-id="84803-785">Response</span></span>
<span data-ttu-id="84803-p196">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84803-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26647

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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




