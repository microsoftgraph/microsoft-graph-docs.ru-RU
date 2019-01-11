---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a4391676ad9620210f0cb80339ac986b5229e856
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859383"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="82c1f-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="82c1f-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="82c1f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82c1f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82c1f-105">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-105">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82c1f-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="82c1f-106">Prerequisites</span></span>
<span data-ttu-id="82c1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82c1f-109">Permission type</span></span>|<span data-ttu-id="82c1f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82c1f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82c1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82c1f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82c1f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c1f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82c1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82c1f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82c1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c1f-114">Not supported.</span></span>|
|<span data-ttu-id="82c1f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82c1f-115">Application</span></span>|<span data-ttu-id="82c1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c1f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82c1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82c1f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82c1f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82c1f-118">Request headers</span></span>
|<span data-ttu-id="82c1f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82c1f-119">Header</span></span>|<span data-ttu-id="82c1f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="82c1f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82c1f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82c1f-121">Authorization</span></span>|<span data-ttu-id="82c1f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82c1f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82c1f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="82c1f-123">Accept</span></span>|<span data-ttu-id="82c1f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82c1f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82c1f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82c1f-125">Request body</span></span>
<span data-ttu-id="82c1f-126">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82c1f-126">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="82c1f-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-127">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="82c1f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="82c1f-128">Property</span></span>|<span data-ttu-id="82c1f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="82c1f-129">Type</span></span>|<span data-ttu-id="82c1f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="82c1f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c1f-131">id</span><span class="sxs-lookup"><span data-stu-id="82c1f-131">id</span></span>|<span data-ttu-id="82c1f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="82c1f-132">String</span></span>|<span data-ttu-id="82c1f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82c1f-133">Key of the entity.</span></span> <span data-ttu-id="82c1f-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c1f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82c1f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="82c1f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82c1f-136">DateTimeOffset</span></span>|<span data-ttu-id="82c1f-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82c1f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="82c1f-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c1f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82c1f-139">createdDateTime</span></span>|<span data-ttu-id="82c1f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82c1f-140">DateTimeOffset</span></span>|<span data-ttu-id="82c1f-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="82c1f-141">DateTime the object was created.</span></span> <span data-ttu-id="82c1f-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c1f-143">описание</span><span class="sxs-lookup"><span data-stu-id="82c1f-143">description</span></span>|<span data-ttu-id="82c1f-144">Строка</span><span class="sxs-lookup"><span data-stu-id="82c1f-144">String</span></span>|<span data-ttu-id="82c1f-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82c1f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82c1f-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c1f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="82c1f-147">displayName</span></span>|<span data-ttu-id="82c1f-148">Строка</span><span class="sxs-lookup"><span data-stu-id="82c1f-148">String</span></span>|<span data-ttu-id="82c1f-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82c1f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82c1f-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c1f-151">version</span><span class="sxs-lookup"><span data-stu-id="82c1f-151">version</span></span>|<span data-ttu-id="82c1f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="82c1f-152">Int32</span></span>|<span data-ttu-id="82c1f-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82c1f-153">Version of the device configuration.</span></span> <span data-ttu-id="82c1f-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82c1f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82c1f-155">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="82c1f-155">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="82c1f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-156">Boolean</span></span>|<span data-ttu-id="82c1f-157">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="82c1f-157">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="82c1f-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="82c1f-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="82c1f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="82c1f-159">Int32</span></span>|<span data-ttu-id="82c1f-160">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="82c1f-160">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="82c1f-161">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="82c1f-161">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="82c1f-162">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="82c1f-162">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="82c1f-163">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="82c1f-163">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="82c1f-164">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="82c1f-164">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="82c1f-165">Выберите предварительный ключ, кодировка для использования.</span><span class="sxs-lookup"><span data-stu-id="82c1f-165">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="82c1f-166">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="82c1f-166">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="82c1f-167">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="82c1f-167">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="82c1f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-168">Boolean</span></span>|<span data-ttu-id="82c1f-169">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="82c1f-169">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="82c1f-170">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="82c1f-170">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="82c1f-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-171">Boolean</span></span>|<span data-ttu-id="82c1f-172">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="82c1f-172">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="82c1f-173">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="82c1f-173">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="82c1f-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-174">Boolean</span></span>|<span data-ttu-id="82c1f-175">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="82c1f-175">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="82c1f-176">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="82c1f-176">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="82c1f-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-177">Boolean</span></span>|<span data-ttu-id="82c1f-178">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="82c1f-178">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="82c1f-179">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="82c1f-179">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="82c1f-180">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="82c1f-180">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="82c1f-181">Укажите, как быть реализовано списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82c1f-181">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="82c1f-182">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="82c1f-182">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="82c1f-183">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="82c1f-183">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="82c1f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-184">Boolean</span></span>|<span data-ttu-id="82c1f-185">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="82c1f-185">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="82c1f-186">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="82c1f-186">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="82c1f-187">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="82c1f-187">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="82c1f-188">Настраивает применения пакетов очередей в сценарии туннель шлюза.</span><span class="sxs-lookup"><span data-stu-id="82c1f-188">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="82c1f-189">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="82c1f-189">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="82c1f-190">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="82c1f-190">firewallProfileDomain</span></span>|[<span data-ttu-id="82c1f-191">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="82c1f-191">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="82c1f-192">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="82c1f-192">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="82c1f-193">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="82c1f-193">firewallProfilePublic</span></span>|[<span data-ttu-id="82c1f-194">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="82c1f-194">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="82c1f-195">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="82c1f-195">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="82c1f-196">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="82c1f-196">firewallProfilePrivate</span></span>|[<span data-ttu-id="82c1f-197">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="82c1f-197">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="82c1f-198">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="82c1f-198">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="82c1f-199">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="82c1f-199">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="82c1f-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82c1f-200">String collection</span></span>|<span data-ttu-id="82c1f-201">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="82c1f-201">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="82c1f-202">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="82c1f-202">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="82c1f-203">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82c1f-203">String collection</span></span>|<span data-ttu-id="82c1f-204">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="82c1f-204">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="82c1f-205">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="82c1f-205">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="82c1f-206">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82c1f-206">String collection</span></span>|<span data-ttu-id="82c1f-207">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="82c1f-207">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="82c1f-208">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="82c1f-208">defenderExploitProtectionXml</span></span>|<span data-ttu-id="82c1f-209">Binary</span><span class="sxs-lookup"><span data-stu-id="82c1f-209">Binary</span></span>|<span data-ttu-id="82c1f-210">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="82c1f-210">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="82c1f-211">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="82c1f-211">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="82c1f-212">String</span><span class="sxs-lookup"><span data-stu-id="82c1f-212">String</span></span>|<span data-ttu-id="82c1f-213">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="82c1f-213">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="82c1f-214">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="82c1f-214">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="82c1f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-215">Boolean</span></span>|<span data-ttu-id="82c1f-216">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="82c1f-216">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="82c1f-217">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="82c1f-217">appLockerApplicationControl</span></span>|[<span data-ttu-id="82c1f-218">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="82c1f-218">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="82c1f-219">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="82c1f-219">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="82c1f-220">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="82c1f-220">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="82c1f-221">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="82c1f-221">smartScreenEnableInShell</span></span>|<span data-ttu-id="82c1f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-222">Boolean</span></span>|<span data-ttu-id="82c1f-223">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="82c1f-223">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="82c1f-224">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="82c1f-224">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="82c1f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-225">Boolean</span></span>|<span data-ttu-id="82c1f-226">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="82c1f-226">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="82c1f-227">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="82c1f-227">applicationGuardEnabled</span></span>|<span data-ttu-id="82c1f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-228">Boolean</span></span>|<span data-ttu-id="82c1f-229">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="82c1f-229">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="82c1f-230">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="82c1f-230">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="82c1f-231">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="82c1f-231">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="82c1f-232">Блокировать буфера обмена передача файла изображения, текстовый файл или ни один из них.</span><span class="sxs-lookup"><span data-stu-id="82c1f-232">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="82c1f-233">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="82c1f-233">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="82c1f-234">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="82c1f-234">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="82c1f-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-235">Boolean</span></span>|<span data-ttu-id="82c1f-236">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="82c1f-236">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="82c1f-237">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="82c1f-237">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="82c1f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-238">Boolean</span></span>|<span data-ttu-id="82c1f-239">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="82c1f-239">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="82c1f-240">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="82c1f-240">applicationGuardForceAuditing</span></span>|<span data-ttu-id="82c1f-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-241">Boolean</span></span>|<span data-ttu-id="82c1f-242">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="82c1f-242">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="82c1f-243">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="82c1f-243">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="82c1f-244">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="82c1f-244">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="82c1f-245">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="82c1f-245">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="82c1f-246">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="82c1f-246">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="82c1f-247">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="82c1f-247">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="82c1f-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-248">Boolean</span></span>|<span data-ttu-id="82c1f-249">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="82c1f-249">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="82c1f-250">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="82c1f-250">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="82c1f-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-251">Boolean</span></span>|<span data-ttu-id="82c1f-252">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="82c1f-252">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="82c1f-253">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="82c1f-253">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="82c1f-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-254">Boolean</span></span>|<span data-ttu-id="82c1f-255">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="82c1f-255">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="82c1f-256">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="82c1f-256">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="82c1f-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-257">Boolean</span></span>|<span data-ttu-id="82c1f-258">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="82c1f-258">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="82c1f-259">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="82c1f-259">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="82c1f-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-260">Boolean</span></span>|<span data-ttu-id="82c1f-261">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="82c1f-261">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="82c1f-262">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="82c1f-262">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="82c1f-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-263">Boolean</span></span>|<span data-ttu-id="82c1f-264">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="82c1f-264">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="82c1f-265">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="82c1f-265">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="82c1f-266">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="82c1f-266">bitLockerEncryptDevice</span></span>|<span data-ttu-id="82c1f-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c1f-267">Boolean</span></span>|<span data-ttu-id="82c1f-268">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="82c1f-268">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="82c1f-269">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="82c1f-269">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="82c1f-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="82c1f-270">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="82c1f-271">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="82c1f-271">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="82c1f-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c1f-272">Response</span></span>
<span data-ttu-id="82c1f-273">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="82c1f-273">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82c1f-274">Пример</span><span class="sxs-lookup"><span data-stu-id="82c1f-274">Example</span></span>
### <a name="request"></a><span data-ttu-id="82c1f-275">Запрос</span><span class="sxs-lookup"><span data-stu-id="82c1f-275">Request</span></span>
<span data-ttu-id="82c1f-276">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82c1f-276">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82c1f-277">Ответ</span><span class="sxs-lookup"><span data-stu-id="82c1f-277">Response</span></span>
<span data-ttu-id="82c1f-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="82c1f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



