# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="33ac2-101">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="33ac2-101">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="33ac2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="33ac2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33ac2-103">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-103">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33ac2-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="33ac2-104">Prerequisites</span></span>
<span data-ttu-id="33ac2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="33ac2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33ac2-107">Permission type</span></span>|<span data-ttu-id="33ac2-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33ac2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33ac2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33ac2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="33ac2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ac2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33ac2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33ac2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33ac2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33ac2-112">Not supported.</span></span>|
|<span data-ttu-id="33ac2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33ac2-113">Application</span></span>|<span data-ttu-id="33ac2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33ac2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33ac2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33ac2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33ac2-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33ac2-116">Request headers</span></span>
|<span data-ttu-id="33ac2-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33ac2-117">Header</span></span>|<span data-ttu-id="33ac2-118">Значение</span><span class="sxs-lookup"><span data-stu-id="33ac2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33ac2-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33ac2-119">Authorization</span></span>|<span data-ttu-id="33ac2-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="33ac2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33ac2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="33ac2-121">Accept</span></span>|<span data-ttu-id="33ac2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="33ac2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33ac2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33ac2-123">Request body</span></span>
<span data-ttu-id="33ac2-124">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33ac2-124">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="33ac2-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-125">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="33ac2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="33ac2-126">Property</span></span>|<span data-ttu-id="33ac2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="33ac2-127">Type</span></span>|<span data-ttu-id="33ac2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="33ac2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33ac2-129">id</span><span class="sxs-lookup"><span data-stu-id="33ac2-129">id</span></span>|<span data-ttu-id="33ac2-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="33ac2-130">String</span></span>|<span data-ttu-id="33ac2-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33ac2-131">Key of the entity.</span></span> <span data-ttu-id="33ac2-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33ac2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33ac2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="33ac2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ac2-134">DateTimeOffset</span></span>|<span data-ttu-id="33ac2-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33ac2-135">DateTime the object was last modified.</span></span> <span data-ttu-id="33ac2-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33ac2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33ac2-137">createdDateTime</span></span>|<span data-ttu-id="33ac2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ac2-138">DateTimeOffset</span></span>|<span data-ttu-id="33ac2-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33ac2-139">DateTime the object was created.</span></span> <span data-ttu-id="33ac2-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33ac2-141">description</span><span class="sxs-lookup"><span data-stu-id="33ac2-141">description</span></span>|<span data-ttu-id="33ac2-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="33ac2-142">String</span></span>|<span data-ttu-id="33ac2-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33ac2-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33ac2-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33ac2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="33ac2-145">displayName</span></span>|<span data-ttu-id="33ac2-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="33ac2-146">String</span></span>|<span data-ttu-id="33ac2-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33ac2-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33ac2-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33ac2-149">version</span><span class="sxs-lookup"><span data-stu-id="33ac2-149">version</span></span>|<span data-ttu-id="33ac2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="33ac2-150">Int32</span></span>|<span data-ttu-id="33ac2-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33ac2-151">Version of the device configuration.</span></span> <span data-ttu-id="33ac2-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33ac2-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33ac2-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="33ac2-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="33ac2-154">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-154">Boolean</span></span>|<span data-ttu-id="33ac2-155">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="33ac2-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="33ac2-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="33ac2-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="33ac2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="33ac2-157">Int32</span></span>|<span data-ttu-id="33ac2-158">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="33ac2-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="33ac2-159">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="33ac2-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="33ac2-160">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="33ac2-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="33ac2-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="33ac2-161">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="33ac2-162">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="33ac2-162">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="33ac2-163">Выберите предварительную кодировку ключа, которая будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="33ac2-163">Select the preshared key encoding to be used Possible values are: , , .</span></span> <span data-ttu-id="33ac2-164">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="33ac2-164">The possible values are `deviceDefault`, `none`, `utF8`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="33ac2-165">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="33ac2-165">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="33ac2-166">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-166">Boolean</span></span>|<span data-ttu-id="33ac2-167">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="33ac2-167">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="33ac2-168">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="33ac2-168">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="33ac2-169">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-169">Boolean</span></span>|<span data-ttu-id="33ac2-170">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="33ac2-170">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="33ac2-171">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="33ac2-171">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="33ac2-172">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-172">Boolean</span></span>|<span data-ttu-id="33ac2-173">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="33ac2-173">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="33ac2-174">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="33ac2-174">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="33ac2-175">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-175">Boolean</span></span>|<span data-ttu-id="33ac2-176">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="33ac2-176">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="33ac2-177">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="33ac2-177">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="33ac2-178">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="33ac2-178">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="33ac2-179">Укажите способ принудительного отзыва списка сертификатов.</span><span class="sxs-lookup"><span data-stu-id="33ac2-179">Specify how the certificate revocation list is to be enforced Possible values are: , , , .</span></span> <span data-ttu-id="33ac2-180">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="33ac2-180">The possible values are `deviceDefault`, `none`, `attempt`, `require`, , , , , , , , or .</span></span>|
|<span data-ttu-id="33ac2-181">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="33ac2-181">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="33ac2-182">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-182">Boolean</span></span>|<span data-ttu-id="33ac2-183">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="33ac2-183">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="33ac2-184">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="33ac2-184">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="33ac2-185">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="33ac2-185">firewallPacketQueueingMethodType</span></span>](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|<span data-ttu-id="33ac2-186">Настраивает организацию очереди пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="33ac2-186">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: , , , , .</span></span> <span data-ttu-id="33ac2-187">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="33ac2-187">The possible values are `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`, , , , , , , or .</span></span>|
|<span data-ttu-id="33ac2-188">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="33ac2-188">firewallProfileDomain</span></span>|[<span data-ttu-id="33ac2-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="33ac2-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="33ac2-190">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="33ac2-190">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="33ac2-191">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="33ac2-191">firewallProfilePublic</span></span>|[<span data-ttu-id="33ac2-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="33ac2-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="33ac2-193">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="33ac2-193">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="33ac2-194">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="33ac2-194">firewallProfilePrivate</span></span>|[<span data-ttu-id="33ac2-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="33ac2-195">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="33ac2-196">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="33ac2-196">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="33ac2-197">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="33ac2-197">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="33ac2-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="33ac2-198">String collection</span></span>|<span data-ttu-id="33ac2-199">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="33ac2-199">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="33ac2-200">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="33ac2-200">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="33ac2-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="33ac2-201">String collection</span></span>|<span data-ttu-id="33ac2-202">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="33ac2-202">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="33ac2-203">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="33ac2-203">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="33ac2-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="33ac2-204">String collection</span></span>|<span data-ttu-id="33ac2-205">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="33ac2-205">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="33ac2-206">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="33ac2-206">defenderExploitProtectionXml</span></span>|<span data-ttu-id="33ac2-207">Binary</span><span class="sxs-lookup"><span data-stu-id="33ac2-207">Binary</span></span>|<span data-ttu-id="33ac2-208">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="33ac2-208">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="33ac2-209">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="33ac2-209">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="33ac2-210">String (строка)</span><span class="sxs-lookup"><span data-stu-id="33ac2-210">String</span></span>|<span data-ttu-id="33ac2-211">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="33ac2-211">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="33ac2-212">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="33ac2-212">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="33ac2-213">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-213">Boolean</span></span>|<span data-ttu-id="33ac2-214">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="33ac2-214">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="33ac2-215">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="33ac2-215">appLockerApplicationControl</span></span>|[<span data-ttu-id="33ac2-216">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="33ac2-216">appLockerApplicationControlType</span></span>](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|<span data-ttu-id="33ac2-217">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="33ac2-217">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="33ac2-218">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="33ac2-218">The possible values are `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`, , , , , , , or .</span></span>|
|<span data-ttu-id="33ac2-219">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="33ac2-219">smartScreenEnableInShell</span></span>|<span data-ttu-id="33ac2-220">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-220">Boolean</span></span>|<span data-ttu-id="33ac2-221">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="33ac2-221">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="33ac2-222">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="33ac2-222">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="33ac2-223">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-223">Boolean</span></span>|<span data-ttu-id="33ac2-224">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="33ac2-224">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="33ac2-225">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="33ac2-225">applicationGuardEnabled</span></span>|<span data-ttu-id="33ac2-226">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-226">Boolean</span></span>|<span data-ttu-id="33ac2-227">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="33ac2-227">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="33ac2-228">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="33ac2-228">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="33ac2-229">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="33ac2-229">applicationGuardBlockFileTransferType</span></span>](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|<span data-ttu-id="33ac2-230">Позволяет заблокировать передачу изображений, текстовых файлов или и того, и другого через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="33ac2-230">Block clipboard to transfer image file, text file or neither of them Possible values are: , , , , .</span></span> <span data-ttu-id="33ac2-231">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="33ac2-231">The possible values are `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`, , , , , , , or .</span></span>|
|<span data-ttu-id="33ac2-232">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="33ac2-232">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="33ac2-233">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-233">Boolean</span></span>|<span data-ttu-id="33ac2-234">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="33ac2-234">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="33ac2-235">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="33ac2-235">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="33ac2-236">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-236">Boolean</span></span>|<span data-ttu-id="33ac2-237">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="33ac2-237">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="33ac2-238">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="33ac2-238">applicationGuardForceAuditing</span></span>|<span data-ttu-id="33ac2-239">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-239">Boolean</span></span>|<span data-ttu-id="33ac2-240">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="33ac2-240">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="33ac2-241">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="33ac2-241">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="33ac2-242">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="33ac2-242">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="33ac2-243">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="33ac2-243">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="33ac2-244">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="33ac2-244">The possible values are `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`, , , , , , , or .</span></span>|
|<span data-ttu-id="33ac2-245">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="33ac2-245">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="33ac2-246">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-246">Boolean</span></span>|<span data-ttu-id="33ac2-247">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="33ac2-247">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="33ac2-248">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="33ac2-248">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="33ac2-249">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-249">Boolean</span></span>|<span data-ttu-id="33ac2-250">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="33ac2-250">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="33ac2-251">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="33ac2-251">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="33ac2-252">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-252">Boolean</span></span>|<span data-ttu-id="33ac2-253">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="33ac2-253">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="33ac2-254">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="33ac2-254">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="33ac2-255">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-255">Boolean</span></span>|<span data-ttu-id="33ac2-256">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="33ac2-256">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="33ac2-257">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="33ac2-257">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="33ac2-258">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-258">Boolean</span></span>|<span data-ttu-id="33ac2-259">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="33ac2-259">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="33ac2-260">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="33ac2-260">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="33ac2-261">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-261">Boolean</span></span>|<span data-ttu-id="33ac2-262">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="33ac2-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="33ac2-263">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="33ac2-263">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="33ac2-264">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="33ac2-264">bitLockerEncryptDevice</span></span>|<span data-ttu-id="33ac2-265">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="33ac2-265">Boolean</span></span>|<span data-ttu-id="33ac2-266">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="33ac2-266">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="33ac2-267">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="33ac2-267">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="33ac2-268">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="33ac2-268">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="33ac2-269">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="33ac2-269">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="33ac2-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="33ac2-270">Response</span></span>
<span data-ttu-id="33ac2-271">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="33ac2-271">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33ac2-272">Пример</span><span class="sxs-lookup"><span data-stu-id="33ac2-272">Example</span></span>
### <a name="request"></a><span data-ttu-id="33ac2-273">Запрос</span><span class="sxs-lookup"><span data-stu-id="33ac2-273">Request</span></span>
<span data-ttu-id="33ac2-274">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33ac2-274">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4230

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="33ac2-275">Ответ</span><span class="sxs-lookup"><span data-stu-id="33ac2-275">Response</span></span>
<span data-ttu-id="33ac2-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33ac2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



