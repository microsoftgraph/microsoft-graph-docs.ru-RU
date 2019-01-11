---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: edf38ba5b7bf308bfa2cd70846b310ca86f6758f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875560"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="c1879-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1879-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="c1879-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1879-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1879-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1879-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1879-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1879-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1879-107">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1879-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="c1879-108">Prerequisites</span></span>
<span data-ttu-id="c1879-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1879-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1879-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1879-111">Permission type</span></span>|<span data-ttu-id="c1879-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1879-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1879-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1879-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1879-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1879-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1879-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1879-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1879-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1879-116">Not supported.</span></span>|
|<span data-ttu-id="c1879-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1879-117">Application</span></span>|<span data-ttu-id="c1879-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1879-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1879-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1879-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1879-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1879-120">Request headers</span></span>
|<span data-ttu-id="c1879-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1879-121">Header</span></span>|<span data-ttu-id="c1879-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1879-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1879-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1879-123">Authorization</span></span>|<span data-ttu-id="c1879-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c1879-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1879-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1879-125">Accept</span></span>|<span data-ttu-id="c1879-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1879-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1879-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1879-127">Request body</span></span>
<span data-ttu-id="c1879-128">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1879-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="c1879-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="c1879-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1879-130">Property</span></span>|<span data-ttu-id="c1879-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1879-131">Type</span></span>|<span data-ttu-id="c1879-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1879-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1879-133">id</span><span class="sxs-lookup"><span data-stu-id="c1879-133">id</span></span>|<span data-ttu-id="c1879-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-134">String</span></span>|<span data-ttu-id="c1879-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1879-135">Key of the entity.</span></span> <span data-ttu-id="c1879-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1879-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1879-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1879-138">DateTimeOffset</span></span>|<span data-ttu-id="c1879-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c1879-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c1879-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1879-141">roleScopeTagIds</span></span>|<span data-ttu-id="c1879-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1879-142">String collection</span></span>|<span data-ttu-id="c1879-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c1879-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1879-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1879-145">supportsScopeTags</span></span>|<span data-ttu-id="c1879-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-146">Boolean</span></span>|<span data-ttu-id="c1879-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c1879-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1879-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c1879-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1879-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c1879-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1879-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1879-150">This property is read-only.</span></span> <span data-ttu-id="c1879-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1879-152">createdDateTime</span></span>|<span data-ttu-id="c1879-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1879-153">DateTimeOffset</span></span>|<span data-ttu-id="c1879-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c1879-154">DateTime the object was created.</span></span> <span data-ttu-id="c1879-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-156">описание</span><span class="sxs-lookup"><span data-stu-id="c1879-156">description</span></span>|<span data-ttu-id="c1879-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-157">String</span></span>|<span data-ttu-id="c1879-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1879-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1879-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c1879-160">displayName</span></span>|<span data-ttu-id="c1879-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-161">String</span></span>|<span data-ttu-id="c1879-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1879-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1879-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-164">version</span><span class="sxs-lookup"><span data-stu-id="c1879-164">version</span></span>|<span data-ttu-id="c1879-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c1879-165">Int32</span></span>|<span data-ttu-id="c1879-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1879-166">Version of the device configuration.</span></span> <span data-ttu-id="c1879-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1879-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1879-168">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="c1879-168">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="c1879-169">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-169">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-170">Это право используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="c1879-170">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="c1879-171">Сохраненные учетные данные пользователей могут быть раскрыты, если эта привилегия предоставляется другим лицам.</span><span class="sxs-lookup"><span data-stu-id="c1879-171">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="c1879-172">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-172">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-173">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="c1879-173">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="c1879-174">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-174">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-175">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="c1879-175">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="c1879-176">Поддерживается состояний разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-176">State Allowed is supported.</span></span>|
|<span data-ttu-id="c1879-177">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="c1879-177">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="c1879-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-179">Это право пользователя определяет, какие пользователи и группы, блока из подключение к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="c1879-179">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="c1879-180">Поддерживаемые состояния блокировки.</span><span class="sxs-lookup"><span data-stu-id="c1879-180">State Block is supported.</span></span>|
|<span data-ttu-id="c1879-181">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c1879-181">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="c1879-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-183">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c1879-183">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="c1879-184">Процесс таким образом можно получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1879-184">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="c1879-185">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-185">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-186">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="c1879-186">userRightsLocalLogOn</span></span>|[<span data-ttu-id="c1879-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-188">Это право пользователя определяет, какие пользователи могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="c1879-188">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="c1879-189">NotConfigured состояниях, разрешенные и заблокированные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="c1879-189">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="c1879-190">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="c1879-190">userRightsBackupData</span></span>|[<span data-ttu-id="c1879-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-192">Это право пользователя определяет пользователей, которые могут обойти файлов, каталогов, реестра и другие разрешения постоянные объекты при резервном копировании файлов и папок.</span><span class="sxs-lookup"><span data-stu-id="c1879-192">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="c1879-193">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-194">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="c1879-194">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="c1879-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-196">Это право пользователя определяет, какие пользователи и группы можно изменить время и дату на внутренних часов компьютера.</span><span class="sxs-lookup"><span data-stu-id="c1879-196">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="c1879-197">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-198">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="c1879-198">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="c1879-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-200">Этот параметр безопасности определяет, будет ли пользователи могут создавать глобальные объекты, которые доступны для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="c1879-200">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="c1879-201">Пользователи, создающие глобальных объектов может повлиять на процессы, которые выполняются в разделе сеансов другим пользователям, что может привести к повреждению данных или сбой приложения.</span><span class="sxs-lookup"><span data-stu-id="c1879-201">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="c1879-202">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-203">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="c1879-203">userRightsCreatePageFile</span></span>|[<span data-ttu-id="c1879-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-205">Это право пользователя определяет, какие пользователи и группы можно вызвать внутренним API для создания и изменения размера файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="c1879-205">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="c1879-206">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-207">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="c1879-207">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="c1879-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-209">Это право пользователя определяет, какие учетные записи можно использовать с процессами для создания объекта каталога с помощью объекта диспетчера.</span><span class="sxs-lookup"><span data-stu-id="c1879-209">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="c1879-210">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-211">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="c1879-211">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="c1879-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-213">Это право пользователя определяет, если пользователь может создавать символьной ссылки с компьютера, на который входе в систему.</span><span class="sxs-lookup"><span data-stu-id="c1879-213">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="c1879-214">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-215">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="c1879-215">userRightsCreateToken</span></span>|[<span data-ttu-id="c1879-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-217">Это право пользователя определяет, какие пользователи и группы можно использовать для процессов для создания маркер, который можно использовать для получения доступа к любым локальным ресурсам, если процесс использует внутренний интерфейс API для создания маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="c1879-217">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="c1879-218">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-219">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="c1879-219">userRightsDebugPrograms</span></span>|[<span data-ttu-id="c1879-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-221">Это право пользователя определяет, какие пользователи могут запускать программу отладки для любого процесса или ядра.</span><span class="sxs-lookup"><span data-stu-id="c1879-221">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="c1879-222">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="c1879-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="c1879-223">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="c1879-223">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="c1879-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-225">Это право пользователя определяет, какие пользователи и группы, не могут входить в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="c1879-225">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="c1879-226">Поддерживаются только состояния NotConfigured и заблокированные</span><span class="sxs-lookup"><span data-stu-id="c1879-226">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="c1879-227">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="c1879-227">userRightsDelegation</span></span>|[<span data-ttu-id="c1879-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-229">Это право пользователя определяет, какие пользователи могут устанавливать доверие для делегирования в объекте пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="c1879-229">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="c1879-230">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-230">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-231">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="c1879-231">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="c1879-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-233">Это право пользователя определяет, какие учетные записи можно использовать процессом для добавления записей в журнале безопасности.</span><span class="sxs-lookup"><span data-stu-id="c1879-233">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="c1879-234">Журнал безопасности используется для отслеживания несанкционированного доступа в систему.</span><span class="sxs-lookup"><span data-stu-id="c1879-234">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="c1879-235">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-235">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-236">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="c1879-236">userRightsImpersonateClient</span></span>|[<span data-ttu-id="c1879-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-238">Назначение это право пользователя позволяет программам, выполняемым от имени этого пользователя для олицетворения клиента.</span><span class="sxs-lookup"><span data-stu-id="c1879-238">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="c1879-239">Использование этого права пользователя для этого вида олицетворения не позволяет неавторизованных пользователей в качестве клиента для подключения к службе, если они были созданы и затем олицетворить клиента, который может повысить неавторизованных пользователей разрешения на административные или системного уровня.</span><span class="sxs-lookup"><span data-stu-id="c1879-239">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="c1879-240">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-240">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-241">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="c1879-241">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="c1879-242">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-242">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-243">Это право пользователя определяет, какие учетные записи могут использовать процесс записать свойство доступа к другим процессом для увеличения приоритета выполнения, назначенного для других процессов.</span><span class="sxs-lookup"><span data-stu-id="c1879-243">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="c1879-244">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-245">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="c1879-245">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="c1879-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-247">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="c1879-247">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="c1879-248">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-249">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="c1879-249">userRightsLockMemory</span></span>|[<span data-ttu-id="c1879-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-251">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, запрещающий подкачки страниц в виртуальной памяти на диске.</span><span class="sxs-lookup"><span data-stu-id="c1879-251">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="c1879-252">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-253">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="c1879-253">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="c1879-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-255">Это право пользователя определяет, какие пользователи могут задавать доступ к объекту параметров аудита для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="c1879-255">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="c1879-256">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-257">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="c1879-257">userRightsManageVolumes</span></span>|[<span data-ttu-id="c1879-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-259">Это право пользователя определяет, какие пользователи и группы можно выполнять задачи по обслуживанию тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="c1879-259">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="c1879-260">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-261">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="c1879-261">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="c1879-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-263">Право определяет, кто может изменять параметры среды оборудования.</span><span class="sxs-lookup"><span data-stu-id="c1879-263">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="c1879-264">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-265">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="c1879-265">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="c1879-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-267">Это право пользователя определяет, какие учетные записи пользователей можно изменять метки целостности объектов, например файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="c1879-267">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="c1879-268">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-269">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="c1879-269">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="c1879-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-271">Это право пользователя определяет пользователей, которые можно использовать средства мониторинга производительности для отслеживания производительности системных процессов.</span><span class="sxs-lookup"><span data-stu-id="c1879-271">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="c1879-272">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-273">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="c1879-273">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="c1879-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-275">Это право пользователя определяет, какие пользователи могут завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="c1879-275">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="c1879-276">Неправильное использование этого права пользователя может привести отказ в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="c1879-276">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="c1879-277">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-278">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="c1879-278">userRightsRestoreData</span></span>|[<span data-ttu-id="c1879-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-280">Это право пользователя определяет, какие пользователи могут файла, каталога, реестра и другие постоянные объекты разрешений при восстановлении резервных копий файлов и папок, а также определяет пользователей, которые можно назначить любого действительного участника безопасности владельцем объекта.</span><span class="sxs-lookup"><span data-stu-id="c1879-280">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="c1879-281">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-282">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="c1879-282">userRightsTakeOwnership</span></span>|[<span data-ttu-id="c1879-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-284">Это право пользователя определяет, какие пользователи могут стать владельцами любого защищаемого объекта в системе, в том числе объектов Active Directory, файлов и папок, принтеров, разделов реестра, процессов и потоков.</span><span class="sxs-lookup"><span data-stu-id="c1879-284">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="c1879-285">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="c1879-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="c1879-286">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="c1879-286">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="c1879-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="c1879-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="c1879-288">Этот параметр безопасности определяет, какие учетные записи служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="c1879-288">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="c1879-289">Примечание: Этот параметр безопасности не применяется к учетным записям системы, сетевая служба или локальная служба.</span><span class="sxs-lookup"><span data-stu-id="c1879-289">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="c1879-290">Поддерживается только состояние заблокирован.</span><span class="sxs-lookup"><span data-stu-id="c1879-290">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="c1879-291">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="c1879-291">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="c1879-292">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-292">Boolean</span></span>|<span data-ttu-id="c1879-293">Этот параметр определяет, является ли сохранить игры xbox включено (1) или отключено (0).</span><span class="sxs-lookup"><span data-stu-id="c1879-293">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="c1879-294">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="c1879-294">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="c1879-295">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="c1879-295">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="c1879-296">Этот параметр определяет, является ли тип запуска службы управления стандартную программу Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="c1879-296">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="c1879-297">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="c1879-297">Default: Manual.</span></span> <span data-ttu-id="c1879-298">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c1879-298">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="c1879-299">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="c1879-299">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="c1879-300">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="c1879-300">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="c1879-301">Этот параметр определяет, является ли тип запуска службы Live диспетчера проверкой подлинности на основе Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="c1879-301">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="c1879-302">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="c1879-302">Default: Manual.</span></span> <span data-ttu-id="c1879-303">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c1879-303">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="c1879-304">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="c1879-304">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="c1879-305">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="c1879-305">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="c1879-306">Этот параметр определяет, является ли Live игру сохранить тип запуска службы Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="c1879-306">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="c1879-307">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="c1879-307">Default: Manual.</span></span> <span data-ttu-id="c1879-308">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c1879-308">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="c1879-309">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="c1879-309">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="c1879-310">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="c1879-310">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="c1879-311">Этот параметр определяет, является ли тип запуска службы сети Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="c1879-311">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="c1879-312">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="c1879-312">Default: Manual.</span></span> <span data-ttu-id="c1879-313">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c1879-313">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="c1879-314">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="c1879-314">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="c1879-315">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-315">Boolean</span></span>|<span data-ttu-id="c1879-316">Запретить пользователям добавление новых учетных записей Майкрософт для этого компьютера.</span><span class="sxs-lookup"><span data-stu-id="c1879-316">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="c1879-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="c1879-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="c1879-318">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-318">Boolean</span></span>|<span data-ttu-id="c1879-319">Включение локальных учетных записей, которые не являются войти в систему из мест, отличных от физическое устройство защищены паролем. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="c1879-319">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="c1879-320">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="c1879-320">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="c1879-321">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-321">Boolean</span></span>|<span data-ttu-id="c1879-322">Определяет, включена ли учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="c1879-322">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="c1879-323">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="c1879-323">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="c1879-324">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-324">String</span></span>|<span data-ttu-id="c1879-325">Определите имя другой учетной записи необходимо сопоставить с идентификатором безопасности (SID) для учетной записи «Администратор».</span><span class="sxs-lookup"><span data-stu-id="c1879-325">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="c1879-326">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="c1879-326">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="c1879-327">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-327">Boolean</span></span>|<span data-ttu-id="c1879-328">Определяет, включен ли гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="c1879-328">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="c1879-329">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="c1879-329">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="c1879-330">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-330">String</span></span>|<span data-ttu-id="c1879-331">Определите имя другой учетной записи необходимо сопоставить с идентификатором безопасности (SID) для учетной записи «Гость».</span><span class="sxs-lookup"><span data-stu-id="c1879-331">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="c1879-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="c1879-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="c1879-333">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-333">Boolean</span></span>|<span data-ttu-id="c1879-334">Запретить портативных компьютеров извлечения без необходимости входа.</span><span class="sxs-lookup"><span data-stu-id="c1879-334">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="c1879-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="c1879-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="c1879-336">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-336">Boolean</span></span>|<span data-ttu-id="c1879-337">Следует ограничьте Установка драйверов принтера как часть подключение к принтеру только администраторам.</span><span class="sxs-lookup"><span data-stu-id="c1879-337">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="c1879-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="c1879-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="c1879-339">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-339">Boolean</span></span>|<span data-ttu-id="c1879-340">Включение этот параметр позволяет только интерактивно пользователя для доступа к компакт-диска носителя.</span><span class="sxs-lookup"><span data-stu-id="c1879-340">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="c1879-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="c1879-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="c1879-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="c1879-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="c1879-343">Определите, кому разрешено форматирование и извлечение съемных носителей файловой системы NTFS.</span><span class="sxs-lookup"><span data-stu-id="c1879-343">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="c1879-344">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="c1879-344">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="c1879-345">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="c1879-345">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="c1879-346">Int32</span><span class="sxs-lookup"><span data-stu-id="c1879-346">Int32</span></span>|<span data-ttu-id="c1879-347">Определите максимальное число минут бездействия пользователя на экране входа в систему интерактивного рабочего стола до запуска заставки экрана.</span><span class="sxs-lookup"><span data-stu-id="c1879-347">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="c1879-348">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="c1879-348">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="c1879-349">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="c1879-349">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="c1879-350">Int32</span><span class="sxs-lookup"><span data-stu-id="c1879-350">Int32</span></span>|<span data-ttu-id="c1879-351">Определите максимальное число минут бездействия пользователя на экране входа в систему интерактивного рабочего стола до запуска заставки экрана.</span><span class="sxs-lookup"><span data-stu-id="c1879-351">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="c1879-352">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="c1879-352">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="c1879-353">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="c1879-353">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="c1879-354">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-354">Boolean</span></span>|<span data-ttu-id="c1879-355">Требуется сочетание клавиш CTRL + ALT + DEL нажатие, прежде чем пользователь сможет войти.</span><span class="sxs-lookup"><span data-stu-id="c1879-355">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="c1879-356">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="c1879-356">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="c1879-357">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-357">Boolean</span></span>|<span data-ttu-id="c1879-358">Не отображать username последнего человека, который в системе на это устройство.</span><span class="sxs-lookup"><span data-stu-id="c1879-358">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="c1879-359">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="c1879-359">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="c1879-360">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-360">Boolean</span></span>|<span data-ttu-id="c1879-361">Не отображать имя пользователя человека, вход в это устройство после ввода учетных данных и перед отображением рабочий стол устройства.</span><span class="sxs-lookup"><span data-stu-id="c1879-361">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="c1879-362">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="c1879-362">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="c1879-363">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-363">String</span></span>|<span data-ttu-id="c1879-364">Задайте заголовок сообщения для пользователей при входе в.</span><span class="sxs-lookup"><span data-stu-id="c1879-364">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="c1879-365">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="c1879-365">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="c1879-366">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-366">String</span></span>|<span data-ttu-id="c1879-367">Задайте текст сообщения для пользователей при входе в.</span><span class="sxs-lookup"><span data-stu-id="c1879-367">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="c1879-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="c1879-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="c1879-369">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-369">Boolean</span></span>|<span data-ttu-id="c1879-370">Блок PKU2U запросы проверки подлинности для этого устройства для использования online удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c1879-370">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="c1879-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="c1879-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="c1879-372">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-372">Boolean</span></span>|<span data-ttu-id="c1879-373">Пользовательский Интерфейс вспомогательных логическое для сущности LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="c1879-373">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="c1879-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="c1879-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="c1879-375">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-375">String</span></span>|<span data-ttu-id="c1879-376">Измените строку языке по умолчанию, которую нужно разрешить или запретить пользователей и групп для удаленных вызовов для SAM.</span><span class="sxs-lookup"><span data-stu-id="c1879-376">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="c1879-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="c1879-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="c1879-378">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="c1879-378">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="c1879-379">Этот параметр безопасности позволяет клиенту требовать согласования 128-битового шифрования и/или безопасность сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="c1879-379">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="c1879-380">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="c1879-380">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="c1879-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="c1879-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="c1879-382">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="c1879-382">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="c1879-383">Этот параметр безопасности позволяет серверу требовать согласования 128-битового шифрования и/или безопасность сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="c1879-383">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="c1879-384">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="c1879-384">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="c1879-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="c1879-385">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="c1879-386">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="c1879-386">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="c1879-387">Этот параметр безопасности определяет, какой протокол проверки подлинности на запрос и ответ используется для регистрации в сети.</span><span class="sxs-lookup"><span data-stu-id="c1879-387">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="c1879-388">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="c1879-388">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="c1879-389">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="c1879-389">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="c1879-390">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-390">Boolean</span></span>|<span data-ttu-id="c1879-391">Если этот параметр включен, клиент SMB позволяет уязвимость гостевые входы в систему.</span><span class="sxs-lookup"><span data-stu-id="c1879-391">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="c1879-392">Если не настроена, клиент SMB будет отклонить уязвимость гостевые входы в систему.</span><span class="sxs-lookup"><span data-stu-id="c1879-392">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="c1879-393">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="c1879-393">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="c1879-394">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-394">Boolean</span></span>|<span data-ttu-id="c1879-395">Этот параметр безопасности определяет снят ли файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="c1879-395">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="c1879-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="c1879-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="c1879-397">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-397">Boolean</span></span>|<span data-ttu-id="c1879-398">Этот параметр безопасности определяет, можно ли завершать работу компьютера, без необходимости входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="c1879-398">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="c1879-399">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="c1879-399">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="c1879-400">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-400">Boolean</span></span>|<span data-ttu-id="c1879-401">Разрешить UIAccess приложения запрашивать повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="c1879-401">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="c1879-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="c1879-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="c1879-403">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-403">Boolean</span></span>|<span data-ttu-id="c1879-404">Виртуализация файлов и реестра неудачных операций записи для каждого пользователя расположения</span><span class="sxs-lookup"><span data-stu-id="c1879-404">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="c1879-405">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="c1879-405">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="c1879-406">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-406">Boolean</span></span>|<span data-ttu-id="c1879-407">Принудительное применение проверки путь сертификации PKI для указанного исполняемого файла перед разрешением на выполнение.</span><span class="sxs-lookup"><span data-stu-id="c1879-407">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="c1879-408">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="c1879-408">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="c1879-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="c1879-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="c1879-410">Определите поведение запроса на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="c1879-410">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="c1879-411">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="c1879-411">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="c1879-412">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="c1879-412">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="c1879-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="c1879-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="c1879-414">Определите поведение запроса на повышение прав для обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-414">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="c1879-415">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="c1879-415">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="c1879-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="c1879-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="c1879-417">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-417">Boolean</span></span>|<span data-ttu-id="c1879-418">Включите все запросы на повышение прав переход на рабочем столе интерактивного пользователя, а не защищенного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="c1879-418">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="c1879-419">Используются параметры политики вывода запросов для администраторов и обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-419">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="c1879-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="c1879-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="c1879-421">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-421">Boolean</span></span>|<span data-ttu-id="c1879-422">Установка приложения, которых необходимо будет запрашивать учетные данные администратора. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="c1879-422">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="c1879-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="c1879-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="c1879-424">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-424">Boolean</span></span>|<span data-ttu-id="c1879-425">Разрешить UIAccess приложения запрашивать повышение прав без использования безопасного рабочего стола. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="c1879-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="c1879-426">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="c1879-426">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="c1879-427">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-427">Boolean</span></span>|<span data-ttu-id="c1879-428">Определяет ли учетная запись администратора; встроенных использует режиме одобрения администратором или запускает все приложения с правами полного администрирования. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="c1879-428">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="c1879-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="c1879-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="c1879-430">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-430">Boolean</span></span>|<span data-ttu-id="c1879-431">Определение в режиме одобрения администратором и все параметры политики контроля учетных Записей, включены ли, включены по умолчанию</span><span class="sxs-lookup"><span data-stu-id="c1879-431">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="c1879-432">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="c1879-432">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="c1879-433">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="c1879-433">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="c1879-434">Настройка сведений о пользователе, которое отображается при сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="c1879-434">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="c1879-435">Если не настроен, показаны отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1879-435">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="c1879-436">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="c1879-436">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="c1879-437">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="c1879-437">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="c1879-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="c1879-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="c1879-439">Настройка сведений о пользователе, которое отображается при сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="c1879-439">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="c1879-440">Если не настроен, показаны отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1879-440">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="c1879-441">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="c1879-441">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="c1879-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="c1879-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="c1879-443">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-443">Boolean</span></span>|<span data-ttu-id="c1879-444">Этот параметр безопасности определяет, пытается ли SMB-клиент согласовать подписи SMB-пакетов.</span><span class="sxs-lookup"><span data-stu-id="c1879-444">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="c1879-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="c1879-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="c1879-446">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-446">Boolean</span></span>|<span data-ttu-id="c1879-447">Этот параметр безопасности определяет, требуется подпись пакетов SMB-компоненты клиента.</span><span class="sxs-lookup"><span data-stu-id="c1879-447">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="c1879-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="c1879-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="c1879-449">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-449">Boolean</span></span>|<span data-ttu-id="c1879-450">Если включен этот параметр безопасности, перенаправитель блок SMB (Server Message) разрешено отправлять пароли открытым текстом на серверы SMB сторонних разработчиков, которые не поддерживают шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c1879-450">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="c1879-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="c1879-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="c1879-452">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-452">Boolean</span></span>|<span data-ttu-id="c1879-453">Этот параметр безопасности определяет, требуется подпись пакетов SMB-компоненты сервера.</span><span class="sxs-lookup"><span data-stu-id="c1879-453">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="c1879-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="c1879-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="c1879-455">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-455">Boolean</span></span>|<span data-ttu-id="c1879-456">Этот параметр безопасности определяет, будет ли SMB-сервер согласовывать подписи с их клиенты SMB-пакетов.</span><span class="sxs-lookup"><span data-stu-id="c1879-456">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="c1879-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="c1879-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="c1879-458">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-458">Boolean</span></span>|<span data-ttu-id="c1879-459">По умолчанию этот параметр безопасности ограничивает анонимный доступ к общим папкам и каналы для параметров для именованных каналов, доступных анонимным и общих папок, которые могут быть анонимный доступ к</span><span class="sxs-lookup"><span data-stu-id="c1879-459">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="c1879-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="c1879-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="c1879-461">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-461">Boolean</span></span>|<span data-ttu-id="c1879-462">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключение к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="c1879-462">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="c1879-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="c1879-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="c1879-464">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-464">Boolean</span></span>|<span data-ttu-id="c1879-465">Этот параметр безопасности определяет, следует ли анонимные пользователи могут выполнять определенные операции, такие как перечисление имен учетных записей домена и сетевых папок.</span><span class="sxs-lookup"><span data-stu-id="c1879-465">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="c1879-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="c1879-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="c1879-467">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-467">Boolean</span></span>|<span data-ttu-id="c1879-468">Этот параметр безопасности определяет, если при следующей смене пароля хранятся значения хэш-функции LAN Manager (LM) для нового пароля.</span><span class="sxs-lookup"><span data-stu-id="c1879-468">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="c1879-469">По умолчанию не хранятся.</span><span class="sxs-lookup"><span data-stu-id="c1879-469">It’s not stored by default.</span></span>|
|<span data-ttu-id="c1879-470">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="c1879-470">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="c1879-471">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="c1879-471">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="c1879-472">Этот параметр безопасности определяет, что происходит при удалении смарт-карт для пользователя, вошедшего в систему с смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="c1879-472">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="c1879-473">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="c1879-473">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="c1879-474">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="c1879-474">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="c1879-475">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-475">Boolean</span></span>|<span data-ttu-id="c1879-476">Используется для отключения отображения области защиты приложений и веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="c1879-476">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="c1879-477">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="c1879-477">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="c1879-478">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-478">Boolean</span></span>|<span data-ttu-id="c1879-479">Используется для отключения отображения области семейства параметров.</span><span class="sxs-lookup"><span data-stu-id="c1879-479">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="c1879-480">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="c1879-480">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="c1879-481">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-481">Boolean</span></span>|<span data-ttu-id="c1879-482">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="c1879-482">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="c1879-483">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="c1879-483">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="c1879-484">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-484">Boolean</span></span>|<span data-ttu-id="c1879-485">Используется для отключения отображения области защиты брандмауэра и сети.</span><span class="sxs-lookup"><span data-stu-id="c1879-485">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="c1879-486">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="c1879-486">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="c1879-487">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-487">Boolean</span></span>|<span data-ttu-id="c1879-488">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="c1879-488">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="c1879-489">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="c1879-489">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="c1879-490">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-490">Boolean</span></span>|<span data-ttu-id="c1879-491">Используется для отключения отображения области защиты учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c1879-491">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="c1879-492">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="c1879-492">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="c1879-493">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-493">Boolean</span></span>|<span data-ttu-id="c1879-494">Используется для отключения отображения области защиты оборудования.</span><span class="sxs-lookup"><span data-stu-id="c1879-494">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="c1879-495">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="c1879-495">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="c1879-496">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-496">Boolean</span></span>|<span data-ttu-id="c1879-497">Используется для отключения отображения области ransomware защиты.</span><span class="sxs-lookup"><span data-stu-id="c1879-497">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="c1879-498">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="c1879-498">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="c1879-499">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-499">Boolean</span></span>|<span data-ttu-id="c1879-500">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройств.</span><span class="sxs-lookup"><span data-stu-id="c1879-500">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="c1879-501">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="c1879-501">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="c1879-502">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-502">Boolean</span></span>|<span data-ttu-id="c1879-503">Используется для отключения отображения процесса обеспечения безопасности, устранение неполадок в разделе Безопасность устройств.</span><span class="sxs-lookup"><span data-stu-id="c1879-503">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="c1879-504">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="c1879-504">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="c1879-505">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-505">String</span></span>|<span data-ttu-id="c1879-506">Имя компании, которая отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-506">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="c1879-507">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="c1879-507">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="c1879-508">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-508">String</span></span>|<span data-ttu-id="c1879-509">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-509">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="c1879-510">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="c1879-510">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="c1879-511">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-511">String</span></span>|<span data-ttu-id="c1879-512">Номер телефона или Скайп код, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-512">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="c1879-513">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="c1879-513">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="c1879-514">Строка</span><span class="sxs-lookup"><span data-stu-id="c1879-514">String</span></span>|<span data-ttu-id="c1879-515">Портал справки URL-адрес, оно отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-515">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="c1879-516">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="c1879-516">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="c1879-517">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="c1879-517">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="c1879-518">Уведомления для отображения из отображаемой области приложения.</span><span class="sxs-lookup"><span data-stu-id="c1879-518">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="c1879-519">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="c1879-519">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="c1879-520">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="c1879-520">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="c1879-521">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="c1879-521">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="c1879-522">Настройка места отображения контактов ИТ сведения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-522">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="c1879-523">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="c1879-523">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="c1879-524">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="c1879-524">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="c1879-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-525">Boolean</span></span>|<span data-ttu-id="c1879-526">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="c1879-526">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="c1879-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="c1879-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="c1879-528">Int32</span><span class="sxs-lookup"><span data-stu-id="c1879-528">Int32</span></span>|<span data-ttu-id="c1879-529">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="c1879-529">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="c1879-530">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="c1879-530">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="c1879-531">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="c1879-531">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="c1879-532">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="c1879-532">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="c1879-533">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="c1879-533">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="c1879-534">Выберите предварительный ключ, кодировка для использования.</span><span class="sxs-lookup"><span data-stu-id="c1879-534">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="c1879-535">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="c1879-535">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="c1879-536">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="c1879-536">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="c1879-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-537">Boolean</span></span>|<span data-ttu-id="c1879-538">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="c1879-538">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="c1879-539">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="c1879-539">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="c1879-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-540">Boolean</span></span>|<span data-ttu-id="c1879-541">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="c1879-541">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="c1879-542">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="c1879-542">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="c1879-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-543">Boolean</span></span>|<span data-ttu-id="c1879-544">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="c1879-544">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="c1879-545">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="c1879-545">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="c1879-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-546">Boolean</span></span>|<span data-ttu-id="c1879-547">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="c1879-547">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="c1879-548">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="c1879-548">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="c1879-549">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="c1879-549">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="c1879-550">Укажите, как быть реализовано списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c1879-550">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="c1879-551">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="c1879-551">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="c1879-552">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="c1879-552">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="c1879-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-553">Boolean</span></span>|<span data-ttu-id="c1879-554">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="c1879-554">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="c1879-555">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="c1879-555">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="c1879-556">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="c1879-556">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="c1879-557">Настраивает применения пакетов очередей в сценарии туннель шлюза.</span><span class="sxs-lookup"><span data-stu-id="c1879-557">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="c1879-558">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="c1879-558">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="c1879-559">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="c1879-559">firewallProfileDomain</span></span>|[<span data-ttu-id="c1879-560">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c1879-560">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="c1879-561">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="c1879-561">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="c1879-562">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="c1879-562">firewallProfilePublic</span></span>|[<span data-ttu-id="c1879-563">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c1879-563">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="c1879-564">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="c1879-564">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="c1879-565">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="c1879-565">firewallProfilePrivate</span></span>|[<span data-ttu-id="c1879-566">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c1879-566">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="c1879-567">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="c1879-567">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="c1879-568">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="c1879-568">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="c1879-569">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1879-569">String collection</span></span>|<span data-ttu-id="c1879-570">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="c1879-570">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="c1879-571">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-571">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="c1879-572">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-572">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-573">Значение, указывающее, поведение приложений Office, добавление в других процессов.</span><span class="sxs-lookup"><span data-stu-id="c1879-573">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="c1879-574">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-574">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-575">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="c1879-575">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="c1879-576">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-576">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-577">Значение, указывающее, поведение приложений Office, добавление в других процессов.</span><span class="sxs-lookup"><span data-stu-id="c1879-577">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="c1879-578">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-578">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="c1879-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="c1879-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-581">Значение, указывающее, поведение приложений/макросов Office Создание и запуск исполняемым содержимым.</span><span class="sxs-lookup"><span data-stu-id="c1879-581">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="c1879-582">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="c1879-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="c1879-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-585">Значение, указывающее, поведение приложений/макросов Office Создание и запуск исполняемым содержимым.</span><span class="sxs-lookup"><span data-stu-id="c1879-585">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="c1879-586">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-587">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="c1879-587">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="c1879-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-589">Значение, указывающее, поведение приложение Office для запуска дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="c1879-589">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="c1879-590">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-591">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="c1879-591">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="c1879-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-593">Значение, указывающее, поведение приложение Office для запуска дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="c1879-593">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="c1879-594">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-595">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="c1879-595">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="c1879-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-597">Значение, указывающее, поведение Win32 импортируется из код макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="c1879-597">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="c1879-598">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-599">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="c1879-599">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="c1879-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-601">Значение, указывающее, поведение Win32 импортируется из код макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="c1879-601">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="c1879-602">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-603">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="c1879-603">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="c1879-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-605">Значение, указывающее, поведение затемненные js/vbs/ps/макроса.</span><span class="sxs-lookup"><span data-stu-id="c1879-605">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="c1879-606">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-607">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="c1879-607">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="c1879-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-609">Значение, указывающее, поведение затемненные js/vbs/ps/макроса.</span><span class="sxs-lookup"><span data-stu-id="c1879-609">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="c1879-610">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-611">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="c1879-611">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="c1879-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-613">Значение, указывающее, поведение js/vbs выполнения полезных данных загружен из Интернета.</span><span class="sxs-lookup"><span data-stu-id="c1879-613">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="c1879-614">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-615">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="c1879-615">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="c1879-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-617">Значение, указывающее, поведение js/vbs выполнения полезных данных загружен из Интернета.</span><span class="sxs-lookup"><span data-stu-id="c1879-617">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="c1879-618">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-619">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="c1879-619">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="c1879-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-621">Значение, указывающее, если разрешен учетных данных, переноса из центра сертификации подсистемы локальной безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="c1879-621">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="c1879-622">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-623">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="c1879-623">defenderProcessCreationType</span></span>|[<span data-ttu-id="c1879-624">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-624">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-625">Значение, указывающее ответ на создание процесса, поступающих из команды PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="c1879-625">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="c1879-626">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-626">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-627">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="c1879-627">defenderProcessCreation</span></span>|[<span data-ttu-id="c1879-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-629">Значение, указывающее ответ на создание процесса, поступающих из команды PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="c1879-629">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="c1879-630">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-631">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="c1879-631">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="c1879-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-633">Значение, указывающее ответ на процессы ненадежные и без знака, на которых выполняется через порт USB.</span><span class="sxs-lookup"><span data-stu-id="c1879-633">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="c1879-634">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-635">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="c1879-635">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="c1879-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-637">Значение, указывающее ответ на процессы ненадежные и без знака, на которых выполняется через порт USB.</span><span class="sxs-lookup"><span data-stu-id="c1879-637">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="c1879-638">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-639">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="c1879-639">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="c1879-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-641">Значение, указывающее, ответ на исполняемые файлы, которые не соответствуют распространением домашних, срок хранения или список надежных критериев.</span><span class="sxs-lookup"><span data-stu-id="c1879-641">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="c1879-642">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-643">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="c1879-643">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="c1879-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-645">Значение, указывающее, ответ на исполняемые файлы, которые не соответствуют распространением домашних, срок хранения или список надежных критериев.</span><span class="sxs-lookup"><span data-stu-id="c1879-645">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="c1879-646">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-647">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="c1879-647">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="c1879-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="c1879-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="c1879-649">Значение, указывающее, если выполнение контента исполняемый файл (EXE-файл, DLL-библиотеку, ps, js, vbs, и т.д.) должны быть удалены из электронной почты (веб-почты/почты клиент).</span><span class="sxs-lookup"><span data-stu-id="c1879-649">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="c1879-650">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-651">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="c1879-651">defenderEmailContentExecution</span></span>|[<span data-ttu-id="c1879-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-653">Значение, указывающее, если выполнение контента исполняемый файл (EXE-файл, DLL-библиотеку, ps, js, vbs, и т.д.) должны быть удалены из электронной почты (веб-почты/почты клиент).</span><span class="sxs-lookup"><span data-stu-id="c1879-653">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="c1879-654">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-655">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-655">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="c1879-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-657">Значение, указывающее, использование дополнительную защиту от ransomeware.</span><span class="sxs-lookup"><span data-stu-id="c1879-657">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="c1879-658">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-659">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="c1879-659">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="c1879-660">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-660">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="c1879-661">Значение, указывающее, поведение защищенные папки.</span><span class="sxs-lookup"><span data-stu-id="c1879-661">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="c1879-662">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="c1879-662">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="c1879-663">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="c1879-663">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="c1879-664">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1879-664">String collection</span></span>|<span data-ttu-id="c1879-665">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="c1879-665">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="c1879-666">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="c1879-666">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="c1879-667">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1879-667">String collection</span></span>|<span data-ttu-id="c1879-668">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="c1879-668">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="c1879-669">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-669">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="c1879-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="c1879-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="c1879-671">Значение, указывающее, поведение NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="c1879-671">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="c1879-672">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="c1879-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="c1879-673">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="c1879-673">defenderExploitProtectionXml</span></span>|<span data-ttu-id="c1879-674">Binary</span><span class="sxs-lookup"><span data-stu-id="c1879-674">Binary</span></span>|<span data-ttu-id="c1879-675">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="c1879-675">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="c1879-676">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="c1879-676">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="c1879-677">String</span><span class="sxs-lookup"><span data-stu-id="c1879-677">String</span></span>|<span data-ttu-id="c1879-678">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="c1879-678">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="c1879-679">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="c1879-679">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="c1879-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-680">Boolean</span></span>|<span data-ttu-id="c1879-681">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="c1879-681">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="c1879-682">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="c1879-682">appLockerApplicationControl</span></span>|[<span data-ttu-id="c1879-683">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="c1879-683">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="c1879-684">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="c1879-684">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="c1879-685">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="c1879-685">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="c1879-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="c1879-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="c1879-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="c1879-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="c1879-688">Включение защиты учетных данных, если платформа уровень безопасности с помощью Secure загрузки и виртуализации на основе безопасности включены.</span><span class="sxs-lookup"><span data-stu-id="c1879-688">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="c1879-689">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="c1879-689">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="c1879-690">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="c1879-690">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="c1879-691">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-691">Boolean</span></span>|<span data-ttu-id="c1879-692">Включение виртуализации на основе Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="c1879-692">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="c1879-693">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="c1879-693">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="c1879-694">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-694">Boolean</span></span>|<span data-ttu-id="c1879-695">Указывает, включена ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="c1879-695">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="c1879-696">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="c1879-696">smartScreenEnableInShell</span></span>|<span data-ttu-id="c1879-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-697">Boolean</span></span>|<span data-ttu-id="c1879-698">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="c1879-698">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="c1879-699">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="c1879-699">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="c1879-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-700">Boolean</span></span>|<span data-ttu-id="c1879-701">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="c1879-701">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="c1879-702">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="c1879-702">applicationGuardEnabled</span></span>|<span data-ttu-id="c1879-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-703">Boolean</span></span>|<span data-ttu-id="c1879-704">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="c1879-704">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="c1879-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="c1879-705">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="c1879-706">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="c1879-706">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="c1879-707">Включение защиты приложения Защитник Windows для новой сборки Windows.</span><span class="sxs-lookup"><span data-stu-id="c1879-707">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="c1879-708">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="c1879-708">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="c1879-709">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="c1879-709">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="c1879-710">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="c1879-710">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="c1879-711">Блокировать буфера обмена передача файла изображения, текстовый файл или ни один из них.</span><span class="sxs-lookup"><span data-stu-id="c1879-711">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="c1879-712">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="c1879-712">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="c1879-713">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="c1879-713">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="c1879-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-714">Boolean</span></span>|<span data-ttu-id="c1879-715">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="c1879-715">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="c1879-716">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="c1879-716">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="c1879-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-717">Boolean</span></span>|<span data-ttu-id="c1879-718">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="c1879-718">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="c1879-719">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="c1879-719">applicationGuardForceAuditing</span></span>|<span data-ttu-id="c1879-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-720">Boolean</span></span>|<span data-ttu-id="c1879-721">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c1879-721">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="c1879-722">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="c1879-722">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="c1879-723">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="c1879-723">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="c1879-724">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="c1879-724">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="c1879-725">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="c1879-725">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="c1879-726">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="c1879-726">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="c1879-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-727">Boolean</span></span>|<span data-ttu-id="c1879-728">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="c1879-728">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="c1879-729">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="c1879-729">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="c1879-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-730">Boolean</span></span>|<span data-ttu-id="c1879-731">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="c1879-731">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="c1879-732">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="c1879-732">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="c1879-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-733">Boolean</span></span>|<span data-ttu-id="c1879-734">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="c1879-734">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="c1879-735">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="c1879-735">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="c1879-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-736">Boolean</span></span>|<span data-ttu-id="c1879-737">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="c1879-737">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="c1879-738">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="c1879-738">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="c1879-739">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-739">Boolean</span></span>|<span data-ttu-id="c1879-740">Разрешить безопасности приложения, чтобы использовать графического виртуальных Процессора</span><span class="sxs-lookup"><span data-stu-id="c1879-740">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="c1879-741">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="c1879-741">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="c1879-742">Логический</span><span class="sxs-lookup"><span data-stu-id="c1879-742">Boolean</span></span>|<span data-ttu-id="c1879-743">Разрешить пользователям загружать файлы из пограничного сервера в контейнере guard приложения и сохранение их на узле файловой системы</span><span class="sxs-lookup"><span data-stu-id="c1879-743">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="c1879-744">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="c1879-744">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="c1879-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-745">Boolean</span></span>|<span data-ttu-id="c1879-746">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1879-746">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="c1879-747">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="c1879-747">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="c1879-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-748">Boolean</span></span>|<span data-ttu-id="c1879-749">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c1879-749">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="c1879-750">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="c1879-750">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="c1879-751">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="c1879-751">bitLockerEncryptDevice</span></span>|<span data-ttu-id="c1879-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1879-752">Boolean</span></span>|<span data-ttu-id="c1879-753">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c1879-753">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="c1879-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c1879-754">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="c1879-755">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c1879-755">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="c1879-756">Политика BitLocker системного диска.</span><span class="sxs-lookup"><span data-stu-id="c1879-756">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="c1879-757">bitLockerFixedDrivePolicy;</span><span class="sxs-lookup"><span data-stu-id="c1879-757">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="c1879-758">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="c1879-758">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="c1879-759">Предопределенная политика диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c1879-759">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="c1879-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c1879-760">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="c1879-761">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c1879-761">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="c1879-762">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="c1879-762">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="c1879-763">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1879-763">Response</span></span>
<span data-ttu-id="c1879-764">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1879-764">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1879-765">Пример</span><span class="sxs-lookup"><span data-stu-id="c1879-765">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1879-766">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1879-766">Request</span></span>
<span data-ttu-id="c1879-767">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1879-767">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26312

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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

### <a name="response"></a><span data-ttu-id="c1879-768">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1879-768">Response</span></span>
<span data-ttu-id="c1879-p194">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c1879-p194">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26499

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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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





