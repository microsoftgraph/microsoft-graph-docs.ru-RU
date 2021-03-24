---
title: Создание windows81VpnConfiguration
description: Создайте новый объект Windows81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7118b29d7b18e36c20d9794af682ff9358d1b36c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147198"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="d5339-103">Создание windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5339-103">Create windows81VpnConfiguration</span></span>

<span data-ttu-id="d5339-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5339-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5339-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5339-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5339-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5339-107">Создайте [новый объект Windows81VpnConfiguration.](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5339-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5339-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5339-108">Prerequisites</span></span>
<span data-ttu-id="d5339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5339-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5339-111">Permission type</span></span>|<span data-ttu-id="d5339-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5339-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5339-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5339-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5339-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5339-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5339-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5339-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5339-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5339-116">Not supported.</span></span>|
|<span data-ttu-id="d5339-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5339-117">Application</span></span>|<span data-ttu-id="d5339-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5339-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5339-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5339-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5339-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5339-120">Request headers</span></span>
|<span data-ttu-id="d5339-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5339-121">Header</span></span>|<span data-ttu-id="d5339-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5339-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5339-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5339-123">Authorization</span></span>|<span data-ttu-id="d5339-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5339-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5339-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5339-125">Accept</span></span>|<span data-ttu-id="d5339-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5339-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5339-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5339-127">Request body</span></span>
<span data-ttu-id="d5339-128">В теле запроса поставляем представление JSON для объекта Windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d5339-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="d5339-129">В следующей таблице показаны свойства, необходимые при создании windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d5339-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="d5339-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5339-130">Property</span></span>|<span data-ttu-id="d5339-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d5339-131">Type</span></span>|<span data-ttu-id="d5339-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d5339-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5339-133">id</span><span class="sxs-lookup"><span data-stu-id="d5339-133">id</span></span>|<span data-ttu-id="d5339-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d5339-134">String</span></span>|<span data-ttu-id="d5339-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d5339-135">Key of the entity.</span></span> <span data-ttu-id="d5339-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5339-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d5339-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5339-138">DateTimeOffset</span></span>|<span data-ttu-id="d5339-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d5339-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d5339-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5339-141">roleScopeTagIds</span></span>|<span data-ttu-id="d5339-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d5339-142">String collection</span></span>|<span data-ttu-id="d5339-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="d5339-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5339-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d5339-145">supportsScopeTags</span></span>|<span data-ttu-id="d5339-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5339-146">Boolean</span></span>|<span data-ttu-id="d5339-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d5339-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d5339-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="d5339-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d5339-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d5339-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d5339-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5339-150">This property is read-only.</span></span> <span data-ttu-id="d5339-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d5339-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d5339-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d5339-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d5339-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d5339-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d5339-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d5339-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d5339-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d5339-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d5339-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d5339-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d5339-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d5339-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d5339-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d5339-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d5339-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d5339-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d5339-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5339-164">createdDateTime</span></span>|<span data-ttu-id="d5339-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5339-165">DateTimeOffset</span></span>|<span data-ttu-id="d5339-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d5339-166">DateTime the object was created.</span></span> <span data-ttu-id="d5339-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-168">description</span><span class="sxs-lookup"><span data-stu-id="d5339-168">description</span></span>|<span data-ttu-id="d5339-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d5339-169">String</span></span>|<span data-ttu-id="d5339-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d5339-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5339-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d5339-172">displayName</span></span>|<span data-ttu-id="d5339-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d5339-173">String</span></span>|<span data-ttu-id="d5339-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d5339-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5339-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-176">version</span><span class="sxs-lookup"><span data-stu-id="d5339-176">version</span></span>|<span data-ttu-id="d5339-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d5339-177">Int32</span></span>|<span data-ttu-id="d5339-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d5339-178">Version of the device configuration.</span></span> <span data-ttu-id="d5339-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5339-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="d5339-180">connectionName</span></span>|<span data-ttu-id="d5339-181">Строка</span><span class="sxs-lookup"><span data-stu-id="d5339-181">String</span></span>|<span data-ttu-id="d5339-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="d5339-182">Connection name displayed to the user.</span></span> <span data-ttu-id="d5339-183">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5339-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-184">серверы</span><span class="sxs-lookup"><span data-stu-id="d5339-184">servers</span></span>|<span data-ttu-id="d5339-185">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="d5339-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d5339-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="d5339-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="d5339-187">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="d5339-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d5339-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d5339-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d5339-189">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5339-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-190">customXml</span><span class="sxs-lookup"><span data-stu-id="d5339-190">customXml</span></span>|<span data-ttu-id="d5339-191">Binary</span><span class="sxs-lookup"><span data-stu-id="d5339-191">Binary</span></span>|<span data-ttu-id="d5339-192">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="d5339-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="d5339-193">(массив byte, закодированный UTF8) Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5339-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5339-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="d5339-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="d5339-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5339-195">Boolean</span></span>|<span data-ttu-id="d5339-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="d5339-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="d5339-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5339-197">This property is read-only.</span></span>|
|<span data-ttu-id="d5339-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="d5339-198">connectionType</span></span>|[<span data-ttu-id="d5339-199">WindowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d5339-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="d5339-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="d5339-200">Connection type.</span></span> <span data-ttu-id="d5339-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="d5339-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="d5339-202">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="d5339-202">loginGroupOrDomain</span></span>|<span data-ttu-id="d5339-203">Строка</span><span class="sxs-lookup"><span data-stu-id="d5339-203">String</span></span>|<span data-ttu-id="d5339-204">Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="d5339-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="d5339-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d5339-205">enableSplitTunneling</span></span>|<span data-ttu-id="d5339-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5339-206">Boolean</span></span>|<span data-ttu-id="d5339-207">Включить раздельный туннель для VPN.</span><span class="sxs-lookup"><span data-stu-id="d5339-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="d5339-208">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d5339-208">proxyServer</span></span>|[<span data-ttu-id="d5339-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d5339-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="d5339-210">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="d5339-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="d5339-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5339-211">Response</span></span>
<span data-ttu-id="d5339-212">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d5339-212">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5339-213">Пример</span><span class="sxs-lookup"><span data-stu-id="d5339-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5339-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5339-214">Request</span></span>
<span data-ttu-id="d5339-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5339-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="d5339-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5339-216">Response</span></span>
<span data-ttu-id="d5339-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5339-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```




