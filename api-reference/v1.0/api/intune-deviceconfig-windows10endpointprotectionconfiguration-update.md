---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b89084ba80cb2664056288dfae290186a7603c0a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760554"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="ced2c-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ced2c-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="ced2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ced2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ced2c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ced2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ced2c-106">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ced2c-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="ced2c-107">Prerequisites</span></span>
<span data-ttu-id="ced2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ced2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced2c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ced2c-110">Permission type</span></span>|<span data-ttu-id="ced2c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ced2c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ced2c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ced2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ced2c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced2c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ced2c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ced2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ced2c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ced2c-115">Not supported.</span></span>|
|<span data-ttu-id="ced2c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ced2c-116">Application</span></span>|<span data-ttu-id="ced2c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced2c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ced2c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ced2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ced2c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ced2c-119">Request headers</span></span>
|<span data-ttu-id="ced2c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ced2c-120">Header</span></span>|<span data-ttu-id="ced2c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ced2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ced2c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ced2c-122">Authorization</span></span>|<span data-ttu-id="ced2c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ced2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ced2c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ced2c-124">Accept</span></span>|<span data-ttu-id="ced2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ced2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ced2c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ced2c-126">Request body</span></span>
<span data-ttu-id="ced2c-127">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ced2c-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="ced2c-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="ced2c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ced2c-129">Property</span></span>|<span data-ttu-id="ced2c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ced2c-130">Type</span></span>|<span data-ttu-id="ced2c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ced2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced2c-132">id</span><span class="sxs-lookup"><span data-stu-id="ced2c-132">id</span></span>|<span data-ttu-id="ced2c-133">String</span><span class="sxs-lookup"><span data-stu-id="ced2c-133">String</span></span>|<span data-ttu-id="ced2c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ced2c-134">Key of the entity.</span></span> <span data-ttu-id="ced2c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ced2c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ced2c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ced2c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ced2c-137">DateTimeOffset</span></span>|<span data-ttu-id="ced2c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ced2c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ced2c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ced2c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ced2c-140">createdDateTime</span></span>|<span data-ttu-id="ced2c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ced2c-141">DateTimeOffset</span></span>|<span data-ttu-id="ced2c-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ced2c-142">DateTime the object was created.</span></span> <span data-ttu-id="ced2c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ced2c-144">description</span><span class="sxs-lookup"><span data-stu-id="ced2c-144">description</span></span>|<span data-ttu-id="ced2c-145">String</span><span class="sxs-lookup"><span data-stu-id="ced2c-145">String</span></span>|<span data-ttu-id="ced2c-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ced2c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ced2c-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ced2c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ced2c-148">displayName</span></span>|<span data-ttu-id="ced2c-149">String</span><span class="sxs-lookup"><span data-stu-id="ced2c-149">String</span></span>|<span data-ttu-id="ced2c-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ced2c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ced2c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ced2c-152">version</span><span class="sxs-lookup"><span data-stu-id="ced2c-152">version</span></span>|<span data-ttu-id="ced2c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ced2c-153">Int32</span></span>|<span data-ttu-id="ced2c-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ced2c-154">Version of the device configuration.</span></span> <span data-ttu-id="ced2c-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced2c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ced2c-156">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="ced2c-156">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="ced2c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-157">Boolean</span></span>|<span data-ttu-id="ced2c-158">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="ced2c-158">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="ced2c-159">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="ced2c-159">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="ced2c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ced2c-160">Int32</span></span>|<span data-ttu-id="ced2c-161">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="ced2c-161">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="ced2c-162">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="ced2c-162">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="ced2c-163">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="ced2c-163">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="ced2c-164">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="ced2c-164">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="ced2c-165">брандмауэрPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="ced2c-165">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="ced2c-166">Выберите кодику предварительного ключа, которая будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="ced2c-166">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="ced2c-167">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="ced2c-167">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="ced2c-168">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="ced2c-168">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="ced2c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-169">Boolean</span></span>|<span data-ttu-id="ced2c-170">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="ced2c-170">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="ced2c-171">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="ced2c-171">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="ced2c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-172">Boolean</span></span>|<span data-ttu-id="ced2c-173">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="ced2c-173">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="ced2c-174">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="ced2c-174">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="ced2c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-175">Boolean</span></span>|<span data-ttu-id="ced2c-176">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="ced2c-176">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="ced2c-177">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="ced2c-177">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="ced2c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-178">Boolean</span></span>|<span data-ttu-id="ced2c-179">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="ced2c-179">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="ced2c-180">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="ced2c-180">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="ced2c-181">брандмауэрCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="ced2c-181">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="ced2c-182">Укажите, как будет применяться список отзывов сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ced2c-182">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="ced2c-183">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="ced2c-183">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="ced2c-184">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="ced2c-184">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="ced2c-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-185">Boolean</span></span>|<span data-ttu-id="ced2c-186">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="ced2c-186">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="ced2c-187">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="ced2c-187">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="ced2c-188">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="ced2c-188">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="ced2c-189">Настраивает, как следует применять очереди пакетов в сценарии шлюза туннеля.</span><span class="sxs-lookup"><span data-stu-id="ced2c-189">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="ced2c-190">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="ced2c-190">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="ced2c-191">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="ced2c-191">firewallProfileDomain</span></span>|[<span data-ttu-id="ced2c-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ced2c-192">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="ced2c-193">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="ced2c-193">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="ced2c-194">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="ced2c-194">firewallProfilePublic</span></span>|[<span data-ttu-id="ced2c-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ced2c-195">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="ced2c-196">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="ced2c-196">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="ced2c-197">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="ced2c-197">firewallProfilePrivate</span></span>|[<span data-ttu-id="ced2c-198">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ced2c-198">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="ced2c-199">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="ced2c-199">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="ced2c-200">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="ced2c-200">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="ced2c-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ced2c-201">String collection</span></span>|<span data-ttu-id="ced2c-202">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="ced2c-202">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="ced2c-203">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="ced2c-203">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="ced2c-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ced2c-204">String collection</span></span>|<span data-ttu-id="ced2c-205">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="ced2c-205">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="ced2c-206">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="ced2c-206">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="ced2c-207">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ced2c-207">String collection</span></span>|<span data-ttu-id="ced2c-208">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="ced2c-208">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="ced2c-209">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="ced2c-209">defenderExploitProtectionXml</span></span>|<span data-ttu-id="ced2c-210">Binary</span><span class="sxs-lookup"><span data-stu-id="ced2c-210">Binary</span></span>|<span data-ttu-id="ced2c-211">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="ced2c-211">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="ced2c-212">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="ced2c-212">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="ced2c-213">String</span><span class="sxs-lookup"><span data-stu-id="ced2c-213">String</span></span>|<span data-ttu-id="ced2c-214">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="ced2c-214">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="ced2c-215">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="ced2c-215">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="ced2c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-216">Boolean</span></span>|<span data-ttu-id="ced2c-217">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="ced2c-217">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="ced2c-218">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="ced2c-218">appLockerApplicationControl</span></span>|[<span data-ttu-id="ced2c-219">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="ced2c-219">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="ced2c-220">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="ced2c-220">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="ced2c-221">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="ced2c-221">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="ced2c-222">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="ced2c-222">smartScreenEnableInShell</span></span>|<span data-ttu-id="ced2c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-223">Boolean</span></span>|<span data-ttu-id="ced2c-224">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="ced2c-224">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="ced2c-225">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="ced2c-225">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="ced2c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-226">Boolean</span></span>|<span data-ttu-id="ced2c-227">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="ced2c-227">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="ced2c-228">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="ced2c-228">applicationGuardEnabled</span></span>|<span data-ttu-id="ced2c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-229">Boolean</span></span>|<span data-ttu-id="ced2c-230">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="ced2c-230">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="ced2c-231">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="ced2c-231">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="ced2c-232">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="ced2c-232">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="ced2c-233">Блокировка буфера обмена для передачи файла изображений, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="ced2c-233">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="ced2c-234">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="ced2c-234">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="ced2c-235">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="ced2c-235">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="ced2c-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-236">Boolean</span></span>|<span data-ttu-id="ced2c-237">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="ced2c-237">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="ced2c-238">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="ced2c-238">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="ced2c-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-239">Boolean</span></span>|<span data-ttu-id="ced2c-240">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="ced2c-240">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="ced2c-241">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="ced2c-241">applicationGuardForceAuditing</span></span>|<span data-ttu-id="ced2c-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-242">Boolean</span></span>|<span data-ttu-id="ced2c-243">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="ced2c-243">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="ced2c-244">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="ced2c-244">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="ced2c-245">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="ced2c-245">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="ced2c-246">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="ced2c-246">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="ced2c-247">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="ced2c-247">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="ced2c-248">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="ced2c-248">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="ced2c-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-249">Boolean</span></span>|<span data-ttu-id="ced2c-250">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ced2c-250">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="ced2c-251">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="ced2c-251">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="ced2c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-252">Boolean</span></span>|<span data-ttu-id="ced2c-253">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ced2c-253">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="ced2c-254">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="ced2c-254">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="ced2c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-255">Boolean</span></span>|<span data-ttu-id="ced2c-256">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ced2c-256">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="ced2c-257">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="ced2c-257">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="ced2c-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-258">Boolean</span></span>|<span data-ttu-id="ced2c-259">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ced2c-259">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="ced2c-260">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="ced2c-260">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="ced2c-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-261">Boolean</span></span>|<span data-ttu-id="ced2c-262">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="ced2c-262">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="ced2c-263">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="ced2c-263">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="ced2c-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-264">Boolean</span></span>|<span data-ttu-id="ced2c-265">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ced2c-265">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="ced2c-266">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="ced2c-266">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="ced2c-267">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="ced2c-267">bitLockerEncryptDevice</span></span>|<span data-ttu-id="ced2c-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced2c-268">Boolean</span></span>|<span data-ttu-id="ced2c-269">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ced2c-269">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="ced2c-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ced2c-270">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="ced2c-271">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ced2c-271">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="ced2c-272">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="ced2c-272">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ced2c-273">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced2c-273">Response</span></span>
<span data-ttu-id="ced2c-274">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ced2c-274">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ced2c-275">Пример</span><span class="sxs-lookup"><span data-stu-id="ced2c-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="ced2c-276">Запрос</span><span class="sxs-lookup"><span data-stu-id="ced2c-276">Request</span></span>
<span data-ttu-id="ced2c-277">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ced2c-277">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4245

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="ced2c-278">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced2c-278">Response</span></span>
<span data-ttu-id="ced2c-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ced2c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```




