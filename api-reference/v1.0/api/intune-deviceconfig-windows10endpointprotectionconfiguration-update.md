---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58b37fa4f7eb83f4f86fe36b2be90c2fac376a11
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365518"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="b811b-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b811b-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="b811b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b811b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b811b-105">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-105">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b811b-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="b811b-106">Prerequisites</span></span>
<span data-ttu-id="b811b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b811b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b811b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b811b-109">Permission type</span></span>|<span data-ttu-id="b811b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b811b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b811b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b811b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b811b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b811b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b811b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b811b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b811b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b811b-114">Not supported.</span></span>|
|<span data-ttu-id="b811b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b811b-115">Application</span></span>|<span data-ttu-id="b811b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b811b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b811b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b811b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b811b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b811b-118">Request headers</span></span>
|<span data-ttu-id="b811b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b811b-119">Header</span></span>|<span data-ttu-id="b811b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b811b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b811b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b811b-121">Authorization</span></span>|<span data-ttu-id="b811b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b811b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b811b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b811b-123">Accept</span></span>|<span data-ttu-id="b811b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b811b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b811b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b811b-125">Request body</span></span>
<span data-ttu-id="b811b-126">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b811b-126">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="b811b-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-127">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="b811b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b811b-128">Property</span></span>|<span data-ttu-id="b811b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b811b-129">Type</span></span>|<span data-ttu-id="b811b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b811b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b811b-131">id</span><span class="sxs-lookup"><span data-stu-id="b811b-131">id</span></span>|<span data-ttu-id="b811b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b811b-132">String</span></span>|<span data-ttu-id="b811b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b811b-133">Key of the entity.</span></span> <span data-ttu-id="b811b-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b811b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b811b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b811b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b811b-136">DateTimeOffset</span></span>|<span data-ttu-id="b811b-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b811b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b811b-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b811b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b811b-139">createdDateTime</span></span>|<span data-ttu-id="b811b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b811b-140">DateTimeOffset</span></span>|<span data-ttu-id="b811b-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b811b-141">DateTime the object was created.</span></span> <span data-ttu-id="b811b-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b811b-143">description</span><span class="sxs-lookup"><span data-stu-id="b811b-143">description</span></span>|<span data-ttu-id="b811b-144">String</span><span class="sxs-lookup"><span data-stu-id="b811b-144">String</span></span>|<span data-ttu-id="b811b-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b811b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b811b-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b811b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b811b-147">displayName</span></span>|<span data-ttu-id="b811b-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b811b-148">String</span></span>|<span data-ttu-id="b811b-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b811b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b811b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b811b-151">version</span><span class="sxs-lookup"><span data-stu-id="b811b-151">version</span></span>|<span data-ttu-id="b811b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b811b-152">Int32</span></span>|<span data-ttu-id="b811b-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b811b-153">Version of the device configuration.</span></span> <span data-ttu-id="b811b-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b811b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b811b-155">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="b811b-155">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="b811b-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-156">Boolean</span></span>|<span data-ttu-id="b811b-157">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="b811b-157">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="b811b-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="b811b-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="b811b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b811b-159">Int32</span></span>|<span data-ttu-id="b811b-160">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="b811b-160">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="b811b-161">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="b811b-161">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="b811b-162">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="b811b-162">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="b811b-163">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="b811b-163">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="b811b-164">фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="b811b-164">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="b811b-165">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="b811b-165">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="b811b-166">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="b811b-166">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="b811b-167">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="b811b-167">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="b811b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-168">Boolean</span></span>|<span data-ttu-id="b811b-169">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="b811b-169">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="b811b-170">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="b811b-170">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="b811b-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-171">Boolean</span></span>|<span data-ttu-id="b811b-172">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="b811b-172">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="b811b-173">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="b811b-173">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="b811b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-174">Boolean</span></span>|<span data-ttu-id="b811b-175">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="b811b-175">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="b811b-176">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="b811b-176">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="b811b-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-177">Boolean</span></span>|<span data-ttu-id="b811b-178">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="b811b-178">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="b811b-179">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="b811b-179">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="b811b-180">фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="b811b-180">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="b811b-181">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="b811b-181">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="b811b-182">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="b811b-182">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="b811b-183">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="b811b-183">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="b811b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-184">Boolean</span></span>|<span data-ttu-id="b811b-185">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="b811b-185">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="b811b-186">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b811b-186">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="b811b-187">фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="b811b-187">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="b811b-188">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="b811b-188">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="b811b-189">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="b811b-189">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="b811b-190">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="b811b-190">firewallProfileDomain</span></span>|[<span data-ttu-id="b811b-191">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b811b-191">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b811b-192">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="b811b-192">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="b811b-193">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="b811b-193">firewallProfilePublic</span></span>|[<span data-ttu-id="b811b-194">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b811b-194">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b811b-195">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="b811b-195">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="b811b-196">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="b811b-196">firewallProfilePrivate</span></span>|[<span data-ttu-id="b811b-197">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b811b-197">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b811b-198">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="b811b-198">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="b811b-199">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="b811b-199">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="b811b-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b811b-200">String collection</span></span>|<span data-ttu-id="b811b-201">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="b811b-201">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="b811b-202">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="b811b-202">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="b811b-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b811b-203">String collection</span></span>|<span data-ttu-id="b811b-204">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="b811b-204">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="b811b-205">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="b811b-205">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="b811b-206">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b811b-206">String collection</span></span>|<span data-ttu-id="b811b-207">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="b811b-207">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="b811b-208">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="b811b-208">defenderExploitProtectionXml</span></span>|<span data-ttu-id="b811b-209">Binary</span><span class="sxs-lookup"><span data-stu-id="b811b-209">Binary</span></span>|<span data-ttu-id="b811b-210">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="b811b-210">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="b811b-211">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="b811b-211">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="b811b-212">String</span><span class="sxs-lookup"><span data-stu-id="b811b-212">String</span></span>|<span data-ttu-id="b811b-213">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="b811b-213">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="b811b-214">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="b811b-214">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="b811b-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-215">Boolean</span></span>|<span data-ttu-id="b811b-216">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="b811b-216">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="b811b-217">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="b811b-217">appLockerApplicationControl</span></span>|[<span data-ttu-id="b811b-218">апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="b811b-218">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="b811b-219">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="b811b-219">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="b811b-220">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="b811b-220">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="b811b-221">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="b811b-221">smartScreenEnableInShell</span></span>|<span data-ttu-id="b811b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-222">Boolean</span></span>|<span data-ttu-id="b811b-223">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="b811b-223">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="b811b-224">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="b811b-224">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="b811b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-225">Boolean</span></span>|<span data-ttu-id="b811b-226">Позволяет ИТ – администраторам контролировать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="b811b-226">Allows IT Admins to control whether users can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="b811b-227">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="b811b-227">applicationGuardEnabled</span></span>|<span data-ttu-id="b811b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-228">Boolean</span></span>|<span data-ttu-id="b811b-229">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="b811b-229">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="b811b-230">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="b811b-230">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="b811b-231">аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="b811b-231">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="b811b-232">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="b811b-232">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="b811b-233">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="b811b-233">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="b811b-234">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="b811b-234">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="b811b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-235">Boolean</span></span>|<span data-ttu-id="b811b-236">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="b811b-236">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="b811b-237">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="b811b-237">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="b811b-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-238">Boolean</span></span>|<span data-ttu-id="b811b-239">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="b811b-239">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="b811b-240">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="b811b-240">applicationGuardForceAuditing</span></span>|<span data-ttu-id="b811b-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-241">Boolean</span></span>|<span data-ttu-id="b811b-242">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="b811b-242">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="b811b-243">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="b811b-243">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="b811b-244">аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="b811b-244">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="b811b-245">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="b811b-245">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="b811b-246">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="b811b-246">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="b811b-247">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="b811b-247">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="b811b-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-248">Boolean</span></span>|<span data-ttu-id="b811b-249">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="b811b-249">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="b811b-250">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="b811b-250">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="b811b-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-251">Boolean</span></span>|<span data-ttu-id="b811b-252">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="b811b-252">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="b811b-253">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="b811b-253">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="b811b-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-254">Boolean</span></span>|<span data-ttu-id="b811b-255">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="b811b-255">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="b811b-256">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="b811b-256">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="b811b-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-257">Boolean</span></span>|<span data-ttu-id="b811b-258">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="b811b-258">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="b811b-259">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="b811b-259">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="b811b-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-260">Boolean</span></span>|<span data-ttu-id="b811b-261">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="b811b-261">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="b811b-262">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="b811b-262">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="b811b-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-263">Boolean</span></span>|<span data-ttu-id="b811b-264">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="b811b-264">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="b811b-265">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="b811b-265">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="b811b-266">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="b811b-266">bitLockerEncryptDevice</span></span>|<span data-ttu-id="b811b-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b811b-267">Boolean</span></span>|<span data-ttu-id="b811b-268">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="b811b-268">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="b811b-269">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b811b-269">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="b811b-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b811b-270">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="b811b-271">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="b811b-271">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="b811b-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="b811b-272">Response</span></span>
<span data-ttu-id="b811b-273">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b811b-273">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b811b-274">Пример</span><span class="sxs-lookup"><span data-stu-id="b811b-274">Example</span></span>

### <a name="request"></a><span data-ttu-id="b811b-275">Запрос</span><span class="sxs-lookup"><span data-stu-id="b811b-275">Request</span></span>
<span data-ttu-id="b811b-276">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b811b-276">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b811b-277">Отклик</span><span class="sxs-lookup"><span data-stu-id="b811b-277">Response</span></span>
<span data-ttu-id="b811b-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b811b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




