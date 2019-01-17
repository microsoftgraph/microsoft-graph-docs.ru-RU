---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e0a9ccd6e6e675614e21ddcca947db87cf76b52b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940780"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="79d2a-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="79d2a-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="79d2a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79d2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79d2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79d2a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79d2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79d2a-107">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79d2a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79d2a-108">Prerequisites</span></span>
<span data-ttu-id="79d2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79d2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79d2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79d2a-111">Permission type</span></span>|<span data-ttu-id="79d2a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79d2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79d2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79d2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79d2a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d2a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79d2a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79d2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79d2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d2a-116">Not supported.</span></span>|
|<span data-ttu-id="79d2a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79d2a-117">Application</span></span>|<span data-ttu-id="79d2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79d2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79d2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79d2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79d2a-120">Request headers</span></span>
|<span data-ttu-id="79d2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79d2a-121">Header</span></span>|<span data-ttu-id="79d2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="79d2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79d2a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79d2a-123">Authorization</span></span>|<span data-ttu-id="79d2a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="79d2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79d2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79d2a-125">Accept</span></span>|<span data-ttu-id="79d2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79d2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79d2a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79d2a-127">Request body</span></span>
<span data-ttu-id="79d2a-128">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79d2a-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="79d2a-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79d2a-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="79d2a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="79d2a-130">Property</span></span>|<span data-ttu-id="79d2a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79d2a-131">Type</span></span>|<span data-ttu-id="79d2a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79d2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d2a-133">id</span><span class="sxs-lookup"><span data-stu-id="79d2a-133">id</span></span>|<span data-ttu-id="79d2a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-134">String</span></span>|<span data-ttu-id="79d2a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79d2a-135">Key of the entity.</span></span> <span data-ttu-id="79d2a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79d2a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="79d2a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d2a-138">DateTimeOffset</span></span>|<span data-ttu-id="79d2a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="79d2a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="79d2a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79d2a-141">roleScopeTagIds</span></span>|<span data-ttu-id="79d2a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79d2a-142">String collection</span></span>|<span data-ttu-id="79d2a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="79d2a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79d2a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="79d2a-145">supportsScopeTags</span></span>|<span data-ttu-id="79d2a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-146">Boolean</span></span>|<span data-ttu-id="79d2a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="79d2a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79d2a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="79d2a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79d2a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="79d2a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79d2a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79d2a-150">This property is read-only.</span></span> <span data-ttu-id="79d2a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79d2a-152">createdDateTime</span></span>|<span data-ttu-id="79d2a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d2a-153">DateTimeOffset</span></span>|<span data-ttu-id="79d2a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="79d2a-154">DateTime the object was created.</span></span> <span data-ttu-id="79d2a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-156">описание</span><span class="sxs-lookup"><span data-stu-id="79d2a-156">description</span></span>|<span data-ttu-id="79d2a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-157">String</span></span>|<span data-ttu-id="79d2a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79d2a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79d2a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="79d2a-160">displayName</span></span>|<span data-ttu-id="79d2a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-161">String</span></span>|<span data-ttu-id="79d2a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79d2a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79d2a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-164">version</span><span class="sxs-lookup"><span data-stu-id="79d2a-164">version</span></span>|<span data-ttu-id="79d2a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="79d2a-165">Int32</span></span>|<span data-ttu-id="79d2a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79d2a-166">Version of the device configuration.</span></span> <span data-ttu-id="79d2a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79d2a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79d2a-168">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="79d2a-168">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="79d2a-169">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-169">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-170">Это право используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="79d2a-170">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="79d2a-171">Сохраненные учетные данные пользователей могут быть раскрыты, если эта привилегия предоставляется другим лицам.</span><span class="sxs-lookup"><span data-stu-id="79d2a-171">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="79d2a-172">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-172">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-173">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="79d2a-173">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="79d2a-174">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-174">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-175">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="79d2a-175">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="79d2a-176">Поддерживается состояний разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-176">State Allowed is supported.</span></span>|
|<span data-ttu-id="79d2a-177">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="79d2a-177">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="79d2a-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-179">Это право пользователя определяет, какие пользователи и группы, блока из подключение к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="79d2a-179">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="79d2a-180">Поддерживаемые состояния блокировки.</span><span class="sxs-lookup"><span data-stu-id="79d2a-180">State Block is supported.</span></span>|
|<span data-ttu-id="79d2a-181">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79d2a-181">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="79d2a-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-183">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="79d2a-183">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="79d2a-184">Процесс таким образом можно получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="79d2a-184">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="79d2a-185">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-185">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-186">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="79d2a-186">userRightsLocalLogOn</span></span>|[<span data-ttu-id="79d2a-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-188">Это право пользователя определяет, какие пользователи могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="79d2a-188">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="79d2a-189">NotConfigured состояниях, разрешенные и заблокированные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="79d2a-189">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="79d2a-190">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="79d2a-190">userRightsBackupData</span></span>|[<span data-ttu-id="79d2a-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-192">Это право пользователя определяет пользователей, которые могут обойти файлов, каталогов, реестра и другие разрешения постоянные объекты при резервном копировании файлов и папок.</span><span class="sxs-lookup"><span data-stu-id="79d2a-192">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="79d2a-193">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-194">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="79d2a-194">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="79d2a-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-196">Это право пользователя определяет, какие пользователи и группы можно изменить время и дату на внутренних часов компьютера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-196">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="79d2a-197">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-198">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="79d2a-198">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="79d2a-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-200">Этот параметр безопасности определяет, будет ли пользователи могут создавать глобальные объекты, которые доступны для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-200">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="79d2a-201">Пользователи, создающие глобальных объектов может повлиять на процессы, которые выполняются в разделе сеансов другим пользователям, что может привести к повреждению данных или сбой приложения.</span><span class="sxs-lookup"><span data-stu-id="79d2a-201">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="79d2a-202">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-203">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="79d2a-203">userRightsCreatePageFile</span></span>|[<span data-ttu-id="79d2a-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-205">Это право пользователя определяет, какие пользователи и группы можно вызвать внутренним API для создания и изменения размера файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="79d2a-205">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="79d2a-206">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-207">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="79d2a-207">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="79d2a-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-209">Это право пользователя определяет, какие учетные записи можно использовать с процессами для создания объекта каталога с помощью объекта диспетчера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-209">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="79d2a-210">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-211">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="79d2a-211">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="79d2a-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-213">Это право пользователя определяет, если пользователь может создавать символьной ссылки с компьютера, на который входе в систему.</span><span class="sxs-lookup"><span data-stu-id="79d2a-213">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="79d2a-214">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-215">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="79d2a-215">userRightsCreateToken</span></span>|[<span data-ttu-id="79d2a-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-217">Это право пользователя определяет, какие пользователи и группы можно использовать для процессов для создания маркер, который можно использовать для получения доступа к любым локальным ресурсам, если процесс использует внутренний интерфейс API для создания маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="79d2a-217">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="79d2a-218">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-219">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="79d2a-219">userRightsDebugPrograms</span></span>|[<span data-ttu-id="79d2a-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-221">Это право пользователя определяет, какие пользователи могут запускать программу отладки для любого процесса или ядра.</span><span class="sxs-lookup"><span data-stu-id="79d2a-221">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="79d2a-222">Поддерживаются только состояния NotConfigured и разрешено</span><span class="sxs-lookup"><span data-stu-id="79d2a-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="79d2a-223">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="79d2a-223">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="79d2a-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-225">Это право пользователя определяет, какие пользователи и группы, не могут входить в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-225">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="79d2a-226">Поддерживаются только состояния NotConfigured и заблокированные</span><span class="sxs-lookup"><span data-stu-id="79d2a-226">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="79d2a-227">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="79d2a-227">userRightsDelegation</span></span>|[<span data-ttu-id="79d2a-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-229">Это право пользователя определяет, какие пользователи могут устанавливать доверие для делегирования в объекте пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-229">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="79d2a-230">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-230">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-231">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="79d2a-231">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="79d2a-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-233">Это право пользователя определяет, какие учетные записи можно использовать процессом для добавления записей в журнале безопасности.</span><span class="sxs-lookup"><span data-stu-id="79d2a-233">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="79d2a-234">Журнал безопасности используется для отслеживания несанкционированного доступа в систему.</span><span class="sxs-lookup"><span data-stu-id="79d2a-234">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="79d2a-235">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-235">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-236">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="79d2a-236">userRightsImpersonateClient</span></span>|[<span data-ttu-id="79d2a-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-238">Назначение это право пользователя позволяет программам, выполняемым от имени этого пользователя для олицетворения клиента.</span><span class="sxs-lookup"><span data-stu-id="79d2a-238">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="79d2a-239">Использование этого права пользователя для этого вида олицетворения не позволяет неавторизованных пользователей в качестве клиента для подключения к службе, если они были созданы и затем олицетворить клиента, который может повысить неавторизованных пользователей разрешения на административные или системного уровня.</span><span class="sxs-lookup"><span data-stu-id="79d2a-239">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="79d2a-240">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-240">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-241">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="79d2a-241">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="79d2a-242">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-242">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-243">Это право пользователя определяет, какие учетные записи могут использовать процесс записать свойство доступа к другим процессом для увеличения приоритета выполнения, назначенного для других процессов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-243">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="79d2a-244">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-245">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="79d2a-245">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="79d2a-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-247">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="79d2a-247">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="79d2a-248">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-249">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="79d2a-249">userRightsLockMemory</span></span>|[<span data-ttu-id="79d2a-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-251">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, запрещающий подкачки страниц в виртуальной памяти на диске.</span><span class="sxs-lookup"><span data-stu-id="79d2a-251">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="79d2a-252">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-253">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="79d2a-253">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="79d2a-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-255">Это право пользователя определяет, какие пользователи могут задавать доступ к объекту параметров аудита для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="79d2a-255">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="79d2a-256">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-257">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="79d2a-257">userRightsManageVolumes</span></span>|[<span data-ttu-id="79d2a-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-259">Это право пользователя определяет, какие пользователи и группы можно выполнять задачи по обслуживанию тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="79d2a-259">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="79d2a-260">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-261">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="79d2a-261">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="79d2a-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-263">Право определяет, кто может изменять параметры среды оборудования.</span><span class="sxs-lookup"><span data-stu-id="79d2a-263">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="79d2a-264">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-265">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="79d2a-265">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="79d2a-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-267">Это право пользователя определяет, какие учетные записи пользователей можно изменять метки целостности объектов, например файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="79d2a-267">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="79d2a-268">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-269">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="79d2a-269">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="79d2a-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-271">Это право пользователя определяет пользователей, которые можно использовать средства мониторинга производительности для отслеживания производительности системных процессов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-271">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="79d2a-272">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-273">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="79d2a-273">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="79d2a-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-275">Это право пользователя определяет, какие пользователи могут завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="79d2a-275">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="79d2a-276">Неправильное использование этого права пользователя может привести отказ в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="79d2a-276">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="79d2a-277">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-278">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="79d2a-278">userRightsRestoreData</span></span>|[<span data-ttu-id="79d2a-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-280">Это право пользователя определяет, какие пользователи могут файла, каталога, реестра и другие постоянные объекты разрешений при восстановлении резервных копий файлов и папок, а также определяет пользователей, которые можно назначить любого действительного участника безопасности владельцем объекта.</span><span class="sxs-lookup"><span data-stu-id="79d2a-280">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="79d2a-281">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-282">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="79d2a-282">userRightsTakeOwnership</span></span>|[<span data-ttu-id="79d2a-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-284">Это право пользователя определяет, какие пользователи могут стать владельцами любого защищаемого объекта в системе, в том числе объектов Active Directory, файлов и папок, принтеров, разделов реестра, процессов и потоков.</span><span class="sxs-lookup"><span data-stu-id="79d2a-284">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="79d2a-285">Поддерживаются только состояния NotConfigured и разрешено.</span><span class="sxs-lookup"><span data-stu-id="79d2a-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="79d2a-286">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="79d2a-286">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="79d2a-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="79d2a-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="79d2a-288">Этот параметр безопасности определяет, какие учетные записи служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="79d2a-288">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="79d2a-289">Примечание: Этот параметр безопасности не применяется к учетным записям системы, сетевая служба или локальная служба.</span><span class="sxs-lookup"><span data-stu-id="79d2a-289">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="79d2a-290">Поддерживается только состояние заблокирован.</span><span class="sxs-lookup"><span data-stu-id="79d2a-290">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="79d2a-291">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="79d2a-291">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="79d2a-292">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-292">Boolean</span></span>|<span data-ttu-id="79d2a-293">Этот параметр определяет, является ли сохранить игры xbox включено (1) или отключено (0).</span><span class="sxs-lookup"><span data-stu-id="79d2a-293">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="79d2a-294">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="79d2a-294">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="79d2a-295">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="79d2a-295">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="79d2a-296">Этот параметр определяет, является ли тип запуска службы управления стандартную программу Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="79d2a-296">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="79d2a-297">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="79d2a-297">Default: Manual.</span></span> <span data-ttu-id="79d2a-298">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-298">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="79d2a-299">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="79d2a-299">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="79d2a-300">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="79d2a-300">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="79d2a-301">Этот параметр определяет, является ли тип запуска службы Live диспетчера проверкой подлинности на основе Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="79d2a-301">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="79d2a-302">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="79d2a-302">Default: Manual.</span></span> <span data-ttu-id="79d2a-303">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-303">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="79d2a-304">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="79d2a-304">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="79d2a-305">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="79d2a-305">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="79d2a-306">Этот параметр определяет, является ли Live игру сохранить тип запуска службы Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="79d2a-306">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="79d2a-307">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="79d2a-307">Default: Manual.</span></span> <span data-ttu-id="79d2a-308">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-308">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="79d2a-309">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="79d2a-309">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="79d2a-310">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="79d2a-310">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="79d2a-311">Этот параметр определяет, является ли тип запуска службы сети Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="79d2a-311">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="79d2a-312">Значение по умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="79d2a-312">Default: Manual.</span></span> <span data-ttu-id="79d2a-313">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-313">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="79d2a-314">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="79d2a-314">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="79d2a-315">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-315">Boolean</span></span>|<span data-ttu-id="79d2a-316">Запретить пользователям добавление новых учетных записей Майкрософт для этого компьютера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-316">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="79d2a-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="79d2a-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="79d2a-318">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-318">Boolean</span></span>|<span data-ttu-id="79d2a-319">Включение локальных учетных записей, которые не являются войти в систему из мест, отличных от физическое устройство защищены паролем. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="79d2a-319">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="79d2a-320">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="79d2a-320">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="79d2a-321">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-321">Boolean</span></span>|<span data-ttu-id="79d2a-322">Определяет, включена ли учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="79d2a-322">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="79d2a-323">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="79d2a-323">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="79d2a-324">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-324">String</span></span>|<span data-ttu-id="79d2a-325">Определите имя другой учетной записи необходимо сопоставить с идентификатором безопасности (SID) для учетной записи «Администратор».</span><span class="sxs-lookup"><span data-stu-id="79d2a-325">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="79d2a-326">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="79d2a-326">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="79d2a-327">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-327">Boolean</span></span>|<span data-ttu-id="79d2a-328">Определяет, включен ли гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="79d2a-328">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="79d2a-329">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="79d2a-329">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="79d2a-330">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-330">String</span></span>|<span data-ttu-id="79d2a-331">Определите имя другой учетной записи необходимо сопоставить с идентификатором безопасности (SID) для учетной записи «Гость».</span><span class="sxs-lookup"><span data-stu-id="79d2a-331">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="79d2a-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="79d2a-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="79d2a-333">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-333">Boolean</span></span>|<span data-ttu-id="79d2a-334">Запретить портативных компьютеров извлечения без необходимости входа.</span><span class="sxs-lookup"><span data-stu-id="79d2a-334">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="79d2a-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="79d2a-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="79d2a-336">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-336">Boolean</span></span>|<span data-ttu-id="79d2a-337">Следует ограничьте Установка драйверов принтера как часть подключение к принтеру только администраторам.</span><span class="sxs-lookup"><span data-stu-id="79d2a-337">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="79d2a-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="79d2a-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="79d2a-339">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-339">Boolean</span></span>|<span data-ttu-id="79d2a-340">Включение этот параметр позволяет только интерактивно пользователя для доступа к компакт-диска носителя.</span><span class="sxs-lookup"><span data-stu-id="79d2a-340">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="79d2a-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="79d2a-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="79d2a-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="79d2a-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="79d2a-343">Определите, кому разрешено форматирование и извлечение съемных носителей файловой системы NTFS.</span><span class="sxs-lookup"><span data-stu-id="79d2a-343">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="79d2a-344">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-344">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="79d2a-345">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="79d2a-345">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="79d2a-346">Int32</span><span class="sxs-lookup"><span data-stu-id="79d2a-346">Int32</span></span>|<span data-ttu-id="79d2a-347">Определите максимальное число минут бездействия пользователя на экране входа в систему интерактивного рабочего стола до запуска заставки экрана.</span><span class="sxs-lookup"><span data-stu-id="79d2a-347">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="79d2a-348">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="79d2a-348">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="79d2a-349">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="79d2a-349">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="79d2a-350">Int32</span><span class="sxs-lookup"><span data-stu-id="79d2a-350">Int32</span></span>|<span data-ttu-id="79d2a-351">Определите максимальное число минут бездействия пользователя на экране входа в систему интерактивного рабочего стола до запуска заставки экрана.</span><span class="sxs-lookup"><span data-stu-id="79d2a-351">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="79d2a-352">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="79d2a-352">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="79d2a-353">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="79d2a-353">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="79d2a-354">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-354">Boolean</span></span>|<span data-ttu-id="79d2a-355">Требуется сочетание клавиш CTRL + ALT + DEL нажатие, прежде чем пользователь сможет войти.</span><span class="sxs-lookup"><span data-stu-id="79d2a-355">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="79d2a-356">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="79d2a-356">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="79d2a-357">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-357">Boolean</span></span>|<span data-ttu-id="79d2a-358">Не отображать username последнего человека, который в системе на это устройство.</span><span class="sxs-lookup"><span data-stu-id="79d2a-358">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="79d2a-359">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="79d2a-359">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="79d2a-360">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-360">Boolean</span></span>|<span data-ttu-id="79d2a-361">Не отображать имя пользователя человека, вход в это устройство после ввода учетных данных и перед отображением рабочий стол устройства.</span><span class="sxs-lookup"><span data-stu-id="79d2a-361">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="79d2a-362">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="79d2a-362">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="79d2a-363">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-363">String</span></span>|<span data-ttu-id="79d2a-364">Задайте заголовок сообщения для пользователей при входе в.</span><span class="sxs-lookup"><span data-stu-id="79d2a-364">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="79d2a-365">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="79d2a-365">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="79d2a-366">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-366">String</span></span>|<span data-ttu-id="79d2a-367">Задайте текст сообщения для пользователей при входе в.</span><span class="sxs-lookup"><span data-stu-id="79d2a-367">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="79d2a-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="79d2a-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="79d2a-369">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-369">Boolean</span></span>|<span data-ttu-id="79d2a-370">Блок PKU2U запросы проверки подлинности для этого устройства для использования online удостоверения.</span><span class="sxs-lookup"><span data-stu-id="79d2a-370">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="79d2a-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="79d2a-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="79d2a-372">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-372">Boolean</span></span>|<span data-ttu-id="79d2a-373">Пользовательский Интерфейс вспомогательных логическое для сущности LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="79d2a-373">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="79d2a-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="79d2a-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="79d2a-375">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-375">String</span></span>|<span data-ttu-id="79d2a-376">Измените строку языке по умолчанию, которую нужно разрешить или запретить пользователей и групп для удаленных вызовов для SAM.</span><span class="sxs-lookup"><span data-stu-id="79d2a-376">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="79d2a-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="79d2a-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="79d2a-378">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="79d2a-378">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="79d2a-379">Этот параметр безопасности позволяет клиенту требовать согласования 128-битового шифрования и/или безопасность сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="79d2a-379">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="79d2a-380">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-380">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="79d2a-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="79d2a-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="79d2a-382">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="79d2a-382">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="79d2a-383">Этот параметр безопасности позволяет серверу требовать согласования 128-битового шифрования и/или безопасность сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="79d2a-383">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="79d2a-384">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-384">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="79d2a-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="79d2a-385">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="79d2a-386">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="79d2a-386">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="79d2a-387">Этот параметр безопасности определяет, какой протокол проверки подлинности на запрос и ответ используется для регистрации в сети.</span><span class="sxs-lookup"><span data-stu-id="79d2a-387">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="79d2a-388">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-388">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="79d2a-389">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="79d2a-389">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="79d2a-390">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-390">Boolean</span></span>|<span data-ttu-id="79d2a-391">Если этот параметр включен, клиент SMB позволяет уязвимость гостевые входы в систему.</span><span class="sxs-lookup"><span data-stu-id="79d2a-391">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="79d2a-392">Если не настроена, клиент SMB будет отклонить уязвимость гостевые входы в систему.</span><span class="sxs-lookup"><span data-stu-id="79d2a-392">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="79d2a-393">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="79d2a-393">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="79d2a-394">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-394">Boolean</span></span>|<span data-ttu-id="79d2a-395">Этот параметр безопасности определяет снят ли файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="79d2a-395">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="79d2a-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="79d2a-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="79d2a-397">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-397">Boolean</span></span>|<span data-ttu-id="79d2a-398">Этот параметр безопасности определяет, можно ли завершать работу компьютера, без необходимости входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="79d2a-398">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="79d2a-399">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="79d2a-399">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="79d2a-400">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-400">Boolean</span></span>|<span data-ttu-id="79d2a-401">Разрешить UIAccess приложения запрашивать повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="79d2a-401">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="79d2a-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="79d2a-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="79d2a-403">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-403">Boolean</span></span>|<span data-ttu-id="79d2a-404">Виртуализация файлов и реестра неудачных операций записи для каждого пользователя расположения</span><span class="sxs-lookup"><span data-stu-id="79d2a-404">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="79d2a-405">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="79d2a-405">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="79d2a-406">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-406">Boolean</span></span>|<span data-ttu-id="79d2a-407">Принудительное применение проверки путь сертификации PKI для указанного исполняемого файла перед разрешением на выполнение.</span><span class="sxs-lookup"><span data-stu-id="79d2a-407">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="79d2a-408">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="79d2a-408">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="79d2a-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="79d2a-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="79d2a-410">Определите поведение запроса на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="79d2a-410">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="79d2a-411">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-411">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="79d2a-412">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="79d2a-412">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="79d2a-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="79d2a-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="79d2a-414">Определите поведение запроса на повышение прав для обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-414">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="79d2a-415">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-415">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="79d2a-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="79d2a-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="79d2a-417">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-417">Boolean</span></span>|<span data-ttu-id="79d2a-418">Включите все запросы на повышение прав переход на рабочем столе интерактивного пользователя, а не защищенного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="79d2a-418">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="79d2a-419">Используются параметры политики вывода запросов для администраторов и обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-419">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="79d2a-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="79d2a-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="79d2a-421">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-421">Boolean</span></span>|<span data-ttu-id="79d2a-422">Установка приложения, которых необходимо будет запрашивать учетные данные администратора. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="79d2a-422">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="79d2a-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="79d2a-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="79d2a-424">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-424">Boolean</span></span>|<span data-ttu-id="79d2a-425">Разрешить UIAccess приложения запрашивать повышение прав без использования безопасного рабочего стола. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="79d2a-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="79d2a-426">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="79d2a-426">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="79d2a-427">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-427">Boolean</span></span>|<span data-ttu-id="79d2a-428">Определяет ли учетная запись администратора; встроенных использует режиме одобрения администратором или запускает все приложения с правами полного администрирования. По умолчанию — включена</span><span class="sxs-lookup"><span data-stu-id="79d2a-428">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="79d2a-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="79d2a-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="79d2a-430">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-430">Boolean</span></span>|<span data-ttu-id="79d2a-431">Определение в режиме одобрения администратором и все параметры политики контроля учетных Записей, включены ли, включены по умолчанию</span><span class="sxs-lookup"><span data-stu-id="79d2a-431">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="79d2a-432">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="79d2a-432">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="79d2a-433">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="79d2a-433">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="79d2a-434">Настройка сведений о пользователе, которое отображается при сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="79d2a-434">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="79d2a-435">Если не настроен, показаны отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="79d2a-435">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="79d2a-436">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-436">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="79d2a-437">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="79d2a-437">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="79d2a-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="79d2a-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="79d2a-439">Настройка сведений о пользователе, которое отображается при сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="79d2a-439">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="79d2a-440">Если не настроен, показаны отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="79d2a-440">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="79d2a-441">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-441">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="79d2a-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="79d2a-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="79d2a-443">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-443">Boolean</span></span>|<span data-ttu-id="79d2a-444">Этот параметр безопасности определяет, пытается ли SMB-клиент согласовать подписи SMB-пакетов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-444">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="79d2a-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="79d2a-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="79d2a-446">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-446">Boolean</span></span>|<span data-ttu-id="79d2a-447">Этот параметр безопасности определяет, требуется подпись пакетов SMB-компоненты клиента.</span><span class="sxs-lookup"><span data-stu-id="79d2a-447">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="79d2a-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="79d2a-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="79d2a-449">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-449">Boolean</span></span>|<span data-ttu-id="79d2a-450">Если включен этот параметр безопасности, перенаправитель блок SMB (Server Message) разрешено отправлять пароли открытым текстом на серверы SMB сторонних разработчиков, которые не поддерживают шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="79d2a-450">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="79d2a-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="79d2a-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="79d2a-452">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-452">Boolean</span></span>|<span data-ttu-id="79d2a-453">Этот параметр безопасности определяет, требуется подпись пакетов SMB-компоненты сервера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-453">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="79d2a-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="79d2a-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="79d2a-455">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-455">Boolean</span></span>|<span data-ttu-id="79d2a-456">Этот параметр безопасности определяет, будет ли SMB-сервер согласовывать подписи с их клиенты SMB-пакетов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-456">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="79d2a-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="79d2a-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="79d2a-458">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-458">Boolean</span></span>|<span data-ttu-id="79d2a-459">По умолчанию этот параметр безопасности ограничивает анонимный доступ к общим папкам и каналы для параметров для именованных каналов, доступных анонимным и общих папок, которые могут быть анонимный доступ к</span><span class="sxs-lookup"><span data-stu-id="79d2a-459">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="79d2a-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="79d2a-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="79d2a-461">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-461">Boolean</span></span>|<span data-ttu-id="79d2a-462">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключение к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="79d2a-462">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="79d2a-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="79d2a-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="79d2a-464">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-464">Boolean</span></span>|<span data-ttu-id="79d2a-465">Этот параметр безопасности определяет, следует ли анонимные пользователи могут выполнять определенные операции, такие как перечисление имен учетных записей домена и сетевых папок.</span><span class="sxs-lookup"><span data-stu-id="79d2a-465">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="79d2a-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="79d2a-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="79d2a-467">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-467">Boolean</span></span>|<span data-ttu-id="79d2a-468">Этот параметр безопасности определяет, если при следующей смене пароля хранятся значения хэш-функции LAN Manager (LM) для нового пароля.</span><span class="sxs-lookup"><span data-stu-id="79d2a-468">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="79d2a-469">По умолчанию не хранятся.</span><span class="sxs-lookup"><span data-stu-id="79d2a-469">It’s not stored by default.</span></span>|
|<span data-ttu-id="79d2a-470">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="79d2a-470">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="79d2a-471">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="79d2a-471">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="79d2a-472">Этот параметр безопасности определяет, что происходит при удалении смарт-карт для пользователя, вошедшего в систему с смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="79d2a-472">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="79d2a-473">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-473">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="79d2a-474">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-474">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="79d2a-475">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-475">Boolean</span></span>|<span data-ttu-id="79d2a-476">Используется для отключения отображения области защиты приложений и веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="79d2a-476">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="79d2a-477">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-477">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="79d2a-478">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-478">Boolean</span></span>|<span data-ttu-id="79d2a-479">Используется для отключения отображения области семейства параметров.</span><span class="sxs-lookup"><span data-stu-id="79d2a-479">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="79d2a-480">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-480">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="79d2a-481">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-481">Boolean</span></span>|<span data-ttu-id="79d2a-482">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="79d2a-482">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="79d2a-483">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-483">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="79d2a-484">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-484">Boolean</span></span>|<span data-ttu-id="79d2a-485">Используется для отключения отображения области защиты брандмауэра и сети.</span><span class="sxs-lookup"><span data-stu-id="79d2a-485">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="79d2a-486">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-486">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="79d2a-487">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-487">Boolean</span></span>|<span data-ttu-id="79d2a-488">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="79d2a-488">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="79d2a-489">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-489">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="79d2a-490">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-490">Boolean</span></span>|<span data-ttu-id="79d2a-491">Используется для отключения отображения области защиты учетной записи.</span><span class="sxs-lookup"><span data-stu-id="79d2a-491">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="79d2a-492">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-492">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="79d2a-493">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-493">Boolean</span></span>|<span data-ttu-id="79d2a-494">Используется для отключения отображения области защиты оборудования.</span><span class="sxs-lookup"><span data-stu-id="79d2a-494">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="79d2a-495">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-495">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="79d2a-496">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-496">Boolean</span></span>|<span data-ttu-id="79d2a-497">Используется для отключения отображения области ransomware защиты.</span><span class="sxs-lookup"><span data-stu-id="79d2a-497">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="79d2a-498">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-498">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="79d2a-499">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-499">Boolean</span></span>|<span data-ttu-id="79d2a-500">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройств.</span><span class="sxs-lookup"><span data-stu-id="79d2a-500">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="79d2a-501">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="79d2a-501">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="79d2a-502">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-502">Boolean</span></span>|<span data-ttu-id="79d2a-503">Используется для отключения отображения процесса обеспечения безопасности, устранение неполадок в разделе Безопасность устройств.</span><span class="sxs-lookup"><span data-stu-id="79d2a-503">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="79d2a-504">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="79d2a-504">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="79d2a-505">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-505">String</span></span>|<span data-ttu-id="79d2a-506">Имя компании, которая отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-506">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="79d2a-507">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="79d2a-507">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="79d2a-508">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-508">String</span></span>|<span data-ttu-id="79d2a-509">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-509">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="79d2a-510">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="79d2a-510">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="79d2a-511">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-511">String</span></span>|<span data-ttu-id="79d2a-512">Номер телефона или Скайп код, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-512">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="79d2a-513">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="79d2a-513">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="79d2a-514">Строка</span><span class="sxs-lookup"><span data-stu-id="79d2a-514">String</span></span>|<span data-ttu-id="79d2a-515">Портал справки URL-адрес, оно отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-515">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="79d2a-516">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="79d2a-516">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="79d2a-517">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="79d2a-517">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="79d2a-518">Уведомления для отображения из отображаемой области приложения.</span><span class="sxs-lookup"><span data-stu-id="79d2a-518">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="79d2a-519">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-519">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="79d2a-520">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="79d2a-520">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="79d2a-521">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="79d2a-521">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="79d2a-522">Настройка места отображения контактов ИТ сведения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-522">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="79d2a-523">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-523">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="79d2a-524">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="79d2a-524">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="79d2a-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-525">Boolean</span></span>|<span data-ttu-id="79d2a-526">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="79d2a-526">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="79d2a-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="79d2a-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="79d2a-528">Int32</span><span class="sxs-lookup"><span data-stu-id="79d2a-528">Int32</span></span>|<span data-ttu-id="79d2a-529">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="79d2a-529">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="79d2a-530">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="79d2a-530">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="79d2a-531">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="79d2a-531">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="79d2a-532">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="79d2a-532">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="79d2a-533">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="79d2a-533">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="79d2a-534">Выберите предварительный ключ, кодировка для использования.</span><span class="sxs-lookup"><span data-stu-id="79d2a-534">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="79d2a-535">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-535">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="79d2a-536">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="79d2a-536">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="79d2a-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-537">Boolean</span></span>|<span data-ttu-id="79d2a-538">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="79d2a-538">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="79d2a-539">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="79d2a-539">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="79d2a-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-540">Boolean</span></span>|<span data-ttu-id="79d2a-541">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="79d2a-541">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="79d2a-542">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="79d2a-542">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="79d2a-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-543">Boolean</span></span>|<span data-ttu-id="79d2a-544">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="79d2a-544">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="79d2a-545">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="79d2a-545">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="79d2a-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-546">Boolean</span></span>|<span data-ttu-id="79d2a-547">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="79d2a-547">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="79d2a-548">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="79d2a-548">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="79d2a-549">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="79d2a-549">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="79d2a-550">Укажите, как быть реализовано списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-550">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="79d2a-551">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-551">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="79d2a-552">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="79d2a-552">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="79d2a-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-553">Boolean</span></span>|<span data-ttu-id="79d2a-554">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="79d2a-554">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="79d2a-555">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="79d2a-555">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="79d2a-556">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="79d2a-556">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="79d2a-557">Настраивает применения пакетов очередей в сценарии туннель шлюза.</span><span class="sxs-lookup"><span data-stu-id="79d2a-557">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="79d2a-558">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-558">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="79d2a-559">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="79d2a-559">firewallProfileDomain</span></span>|[<span data-ttu-id="79d2a-560">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79d2a-560">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="79d2a-561">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="79d2a-561">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="79d2a-562">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="79d2a-562">firewallProfilePublic</span></span>|[<span data-ttu-id="79d2a-563">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79d2a-563">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="79d2a-564">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="79d2a-564">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="79d2a-565">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="79d2a-565">firewallProfilePrivate</span></span>|[<span data-ttu-id="79d2a-566">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79d2a-566">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="79d2a-567">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="79d2a-567">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="79d2a-568">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="79d2a-568">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="79d2a-569">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79d2a-569">String collection</span></span>|<span data-ttu-id="79d2a-570">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="79d2a-570">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="79d2a-571">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-571">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="79d2a-572">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-572">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-573">Значение, указывающее, поведение приложений Office, добавление в других процессов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-573">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="79d2a-574">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-574">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-575">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="79d2a-575">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="79d2a-576">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-576">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-577">Значение, указывающее, поведение приложений Office, добавление в других процессов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-577">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="79d2a-578">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-578">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="79d2a-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="79d2a-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-581">Значение, указывающее, поведение приложений/макросов Office Создание и запуск исполняемым содержимым.</span><span class="sxs-lookup"><span data-stu-id="79d2a-581">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="79d2a-582">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="79d2a-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="79d2a-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-585">Значение, указывающее, поведение приложений/макросов Office Создание и запуск исполняемым содержимым.</span><span class="sxs-lookup"><span data-stu-id="79d2a-585">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="79d2a-586">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-587">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="79d2a-587">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="79d2a-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-589">Значение, указывающее, поведение приложение Office для запуска дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-589">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="79d2a-590">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-591">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="79d2a-591">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="79d2a-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-593">Значение, указывающее, поведение приложение Office для запуска дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-593">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="79d2a-594">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-595">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="79d2a-595">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="79d2a-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-597">Значение, указывающее, поведение Win32 импортируется из код макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="79d2a-597">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="79d2a-598">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-599">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="79d2a-599">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="79d2a-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-601">Значение, указывающее, поведение Win32 импортируется из код макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="79d2a-601">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="79d2a-602">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-603">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="79d2a-603">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="79d2a-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-605">Значение, указывающее, поведение затемненные js/vbs/ps/макроса.</span><span class="sxs-lookup"><span data-stu-id="79d2a-605">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="79d2a-606">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-607">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="79d2a-607">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="79d2a-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-609">Значение, указывающее, поведение затемненные js/vbs/ps/макроса.</span><span class="sxs-lookup"><span data-stu-id="79d2a-609">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="79d2a-610">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-611">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-611">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="79d2a-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-613">Значение, указывающее, поведение js/vbs выполнения полезных данных загружен из Интернета.</span><span class="sxs-lookup"><span data-stu-id="79d2a-613">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="79d2a-614">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-615">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="79d2a-615">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="79d2a-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-617">Значение, указывающее, поведение js/vbs выполнения полезных данных загружен из Интернета.</span><span class="sxs-lookup"><span data-stu-id="79d2a-617">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="79d2a-618">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-619">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="79d2a-619">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="79d2a-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-621">Значение, указывающее, если разрешен учетных данных, переноса из центра сертификации подсистемы локальной безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="79d2a-621">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="79d2a-622">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-623">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="79d2a-623">defenderProcessCreationType</span></span>|[<span data-ttu-id="79d2a-624">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-624">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-625">Значение, указывающее ответ на создание процесса, поступающих из команды PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="79d2a-625">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="79d2a-626">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-626">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-627">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="79d2a-627">defenderProcessCreation</span></span>|[<span data-ttu-id="79d2a-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-629">Значение, указывающее ответ на создание процесса, поступающих из команды PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="79d2a-629">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="79d2a-630">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-631">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="79d2a-631">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="79d2a-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-633">Значение, указывающее ответ на процессы ненадежные и без знака, на которых выполняется через порт USB.</span><span class="sxs-lookup"><span data-stu-id="79d2a-633">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="79d2a-634">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-635">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="79d2a-635">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="79d2a-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-637">Значение, указывающее ответ на процессы ненадежные и без знака, на которых выполняется через порт USB.</span><span class="sxs-lookup"><span data-stu-id="79d2a-637">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="79d2a-638">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-639">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="79d2a-639">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="79d2a-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-641">Значение, указывающее, ответ на исполняемые файлы, которые не соответствуют распространением домашних, срок хранения или список надежных критериев.</span><span class="sxs-lookup"><span data-stu-id="79d2a-641">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="79d2a-642">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-643">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="79d2a-643">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="79d2a-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-645">Значение, указывающее, ответ на исполняемые файлы, которые не соответствуют распространением домашних, срок хранения или список надежных критериев.</span><span class="sxs-lookup"><span data-stu-id="79d2a-645">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="79d2a-646">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-647">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-647">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="79d2a-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="79d2a-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="79d2a-649">Значение, указывающее, если выполнение контента исполняемый файл (EXE-файл, DLL-библиотеку, ps, js, vbs, и т.д.) должны быть удалены из электронной почты (веб-почты/почты клиент).</span><span class="sxs-lookup"><span data-stu-id="79d2a-649">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="79d2a-650">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-651">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="79d2a-651">defenderEmailContentExecution</span></span>|[<span data-ttu-id="79d2a-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-653">Значение, указывающее, если выполнение контента исполняемый файл (EXE-файл, DLL-библиотеку, ps, js, vbs, и т.д.) должны быть удалены из электронной почты (веб-почты/почты клиент).</span><span class="sxs-lookup"><span data-stu-id="79d2a-653">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="79d2a-654">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-655">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-655">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="79d2a-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-657">Значение, указывающее, использование дополнительную защиту от ransomeware.</span><span class="sxs-lookup"><span data-stu-id="79d2a-657">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="79d2a-658">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-659">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="79d2a-659">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="79d2a-660">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-660">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="79d2a-661">Значение, указывающее, поведение защищенные папки.</span><span class="sxs-lookup"><span data-stu-id="79d2a-661">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="79d2a-662">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-662">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="79d2a-663">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="79d2a-663">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="79d2a-664">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79d2a-664">String collection</span></span>|<span data-ttu-id="79d2a-665">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="79d2a-665">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="79d2a-666">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="79d2a-666">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="79d2a-667">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79d2a-667">String collection</span></span>|<span data-ttu-id="79d2a-668">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="79d2a-668">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="79d2a-669">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-669">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="79d2a-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="79d2a-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="79d2a-671">Значение, указывающее, поведение NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="79d2a-671">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="79d2a-672">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="79d2a-673">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="79d2a-673">defenderExploitProtectionXml</span></span>|<span data-ttu-id="79d2a-674">Binary</span><span class="sxs-lookup"><span data-stu-id="79d2a-674">Binary</span></span>|<span data-ttu-id="79d2a-675">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-675">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="79d2a-676">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="79d2a-676">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="79d2a-677">String</span><span class="sxs-lookup"><span data-stu-id="79d2a-677">String</span></span>|<span data-ttu-id="79d2a-678">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="79d2a-678">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="79d2a-679">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="79d2a-679">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="79d2a-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-680">Boolean</span></span>|<span data-ttu-id="79d2a-681">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="79d2a-681">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="79d2a-682">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="79d2a-682">appLockerApplicationControl</span></span>|[<span data-ttu-id="79d2a-683">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="79d2a-683">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="79d2a-684">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="79d2a-684">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="79d2a-685">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-685">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="79d2a-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="79d2a-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="79d2a-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="79d2a-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="79d2a-688">Включение защиты учетных данных, если платформа уровень безопасности с помощью Secure загрузки и виртуализации на основе безопасности включены.</span><span class="sxs-lookup"><span data-stu-id="79d2a-688">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="79d2a-689">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-689">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="79d2a-690">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="79d2a-690">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="79d2a-691">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-691">Boolean</span></span>|<span data-ttu-id="79d2a-692">Включение виртуализации на основе Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="79d2a-692">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="79d2a-693">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="79d2a-693">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="79d2a-694">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-694">Boolean</span></span>|<span data-ttu-id="79d2a-695">Указывает, включена ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="79d2a-695">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="79d2a-696">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="79d2a-696">smartScreenEnableInShell</span></span>|<span data-ttu-id="79d2a-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-697">Boolean</span></span>|<span data-ttu-id="79d2a-698">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="79d2a-698">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="79d2a-699">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="79d2a-699">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="79d2a-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-700">Boolean</span></span>|<span data-ttu-id="79d2a-701">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="79d2a-701">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="79d2a-702">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="79d2a-702">applicationGuardEnabled</span></span>|<span data-ttu-id="79d2a-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-703">Boolean</span></span>|<span data-ttu-id="79d2a-704">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="79d2a-704">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="79d2a-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="79d2a-705">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="79d2a-706">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="79d2a-706">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="79d2a-707">Включение защиты приложения Защитник Windows для новой сборки Windows.</span><span class="sxs-lookup"><span data-stu-id="79d2a-707">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="79d2a-708">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-708">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="79d2a-709">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="79d2a-709">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="79d2a-710">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="79d2a-710">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="79d2a-711">Блокировать буфера обмена передача файла изображения, текстовый файл или ни один из них.</span><span class="sxs-lookup"><span data-stu-id="79d2a-711">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="79d2a-712">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-712">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="79d2a-713">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="79d2a-713">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="79d2a-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-714">Boolean</span></span>|<span data-ttu-id="79d2a-715">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="79d2a-715">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="79d2a-716">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="79d2a-716">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="79d2a-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-717">Boolean</span></span>|<span data-ttu-id="79d2a-718">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="79d2a-718">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="79d2a-719">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="79d2a-719">applicationGuardForceAuditing</span></span>|<span data-ttu-id="79d2a-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-720">Boolean</span></span>|<span data-ttu-id="79d2a-721">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="79d2a-721">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="79d2a-722">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="79d2a-722">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="79d2a-723">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="79d2a-723">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="79d2a-724">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="79d2a-724">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="79d2a-725">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="79d2a-725">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="79d2a-726">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="79d2a-726">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="79d2a-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-727">Boolean</span></span>|<span data-ttu-id="79d2a-728">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-728">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="79d2a-729">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="79d2a-729">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="79d2a-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-730">Boolean</span></span>|<span data-ttu-id="79d2a-731">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-731">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="79d2a-732">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="79d2a-732">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="79d2a-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-733">Boolean</span></span>|<span data-ttu-id="79d2a-734">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-734">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="79d2a-735">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="79d2a-735">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="79d2a-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-736">Boolean</span></span>|<span data-ttu-id="79d2a-737">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="79d2a-737">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="79d2a-738">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="79d2a-738">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="79d2a-739">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-739">Boolean</span></span>|<span data-ttu-id="79d2a-740">Разрешить безопасности приложения, чтобы использовать графического виртуальных Процессора</span><span class="sxs-lookup"><span data-stu-id="79d2a-740">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="79d2a-741">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="79d2a-741">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="79d2a-742">Логический</span><span class="sxs-lookup"><span data-stu-id="79d2a-742">Boolean</span></span>|<span data-ttu-id="79d2a-743">Разрешить пользователям загружать файлы из пограничного сервера в контейнере guard приложения и сохранение их на узле файловой системы</span><span class="sxs-lookup"><span data-stu-id="79d2a-743">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="79d2a-744">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="79d2a-744">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="79d2a-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-745">Boolean</span></span>|<span data-ttu-id="79d2a-746">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="79d2a-746">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="79d2a-747">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="79d2a-747">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="79d2a-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-748">Boolean</span></span>|<span data-ttu-id="79d2a-749">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="79d2a-749">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="79d2a-750">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="79d2a-750">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="79d2a-751">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="79d2a-751">bitLockerEncryptDevice</span></span>|<span data-ttu-id="79d2a-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d2a-752">Boolean</span></span>|<span data-ttu-id="79d2a-753">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="79d2a-753">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="79d2a-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="79d2a-754">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="79d2a-755">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="79d2a-755">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="79d2a-756">Политика BitLocker системного диска.</span><span class="sxs-lookup"><span data-stu-id="79d2a-756">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="79d2a-757">bitLockerFixedDrivePolicy;</span><span class="sxs-lookup"><span data-stu-id="79d2a-757">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="79d2a-758">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="79d2a-758">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="79d2a-759">Предопределенная политика диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="79d2a-759">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="79d2a-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="79d2a-760">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="79d2a-761">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="79d2a-761">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="79d2a-762">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="79d2a-762">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="79d2a-763">Отклик</span><span class="sxs-lookup"><span data-stu-id="79d2a-763">Response</span></span>
<span data-ttu-id="79d2a-764">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79d2a-764">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79d2a-765">Пример</span><span class="sxs-lookup"><span data-stu-id="79d2a-765">Example</span></span>
### <a name="request"></a><span data-ttu-id="79d2a-766">Запрос</span><span class="sxs-lookup"><span data-stu-id="79d2a-766">Request</span></span>
<span data-ttu-id="79d2a-767">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79d2a-767">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26391

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="79d2a-768">Ответ</span><span class="sxs-lookup"><span data-stu-id="79d2a-768">Response</span></span>
<span data-ttu-id="79d2a-p194">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79d2a-p194">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





