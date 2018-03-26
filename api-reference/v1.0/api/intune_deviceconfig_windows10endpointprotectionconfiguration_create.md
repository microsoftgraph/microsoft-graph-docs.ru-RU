# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="7b3e9-101">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b3e9-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="7b3e9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b3e9-103">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b3e9-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b3e9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7b3e9-104">Prerequisites</span></span>
<span data-ttu-id="7b3e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b3e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b3e9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b3e9-107">Permission type</span></span>|<span data-ttu-id="7b3e9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b3e9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7b3e9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3e9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b3e9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b3e9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-112">Not supported.</span></span>|
|<span data-ttu-id="7b3e9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b3e9-113">Application</span></span>|<span data-ttu-id="7b3e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b3e9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b3e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b3e9-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b3e9-116">Request headers</span></span>
|<span data-ttu-id="7b3e9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b3e9-117">Header</span></span>|<span data-ttu-id="7b3e9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7b3e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b3e9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b3e9-119">Authorization</span></span>|<span data-ttu-id="7b3e9-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7b3e9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7b3e9-121">Accept</span></span>|<span data-ttu-id="7b3e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7b3e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b3e9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b3e9-123">Request body</span></span>
<span data-ttu-id="7b3e9-124">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="7b3e9-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7b3e9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b3e9-126">Property</span></span>|<span data-ttu-id="7b3e9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7b3e9-127">Type</span></span>|<span data-ttu-id="7b3e9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7b3e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b3e9-129">id</span><span class="sxs-lookup"><span data-stu-id="7b3e9-129">id</span></span>|<span data-ttu-id="7b3e9-130">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-130">String</span></span>|<span data-ttu-id="7b3e9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-131">Key of the setting.</span></span> <span data-ttu-id="7b3e9-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b3e9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b3e9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7b3e9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b3e9-134">DateTimeOffset</span></span>|<span data-ttu-id="7b3e9-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-135">DateTime the object was last modified.</span></span> <span data-ttu-id="7b3e9-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b3e9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b3e9-137">createdDateTime</span></span>|<span data-ttu-id="7b3e9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b3e9-138">DateTimeOffset</span></span>|<span data-ttu-id="7b3e9-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-139">DateTime the object was created.</span></span> <span data-ttu-id="7b3e9-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b3e9-141">description</span><span class="sxs-lookup"><span data-stu-id="7b3e9-141">description</span></span>|<span data-ttu-id="7b3e9-142">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-142">String</span></span>|<span data-ttu-id="7b3e9-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b3e9-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b3e9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7b3e9-145">displayName</span></span>|<span data-ttu-id="7b3e9-146">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-146">String</span></span>|<span data-ttu-id="7b3e9-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b3e9-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b3e9-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b3e9-149">version</span><span class="sxs-lookup"><span data-stu-id="7b3e9-149">version</span></span>|<span data-ttu-id="7b3e9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7b3e9-150">Int32</span></span>|<span data-ttu-id="7b3e9-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-151">Version of the device configuration.</span></span> <span data-ttu-id="7b3e9-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b3e9-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b3e9-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="7b3e9-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="7b3e9-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-154">Boolean</span></span>|<span data-ttu-id="7b3e9-155">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="7b3e9-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="7b3e9-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="7b3e9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7b3e9-157">Int32</span></span>|<span data-ttu-id="7b3e9-158">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="7b3e9-159">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="7b3e9-160">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="7b3e9-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="7b3e9-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="7b3e9-161">firewallPreSharedKeyEncodingMethod</span></span>|<span data-ttu-id="7b3e9-162">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-162">String</span></span>|<span data-ttu-id="7b3e9-163">Выберите кодировку с общим ключом, которую следует использовать. Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-163">Select the preshared key encoding to be used Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="7b3e9-164">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="7b3e9-164">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="7b3e9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-165">Boolean</span></span>|<span data-ttu-id="7b3e9-166">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-166">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="7b3e9-167">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="7b3e9-167">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="7b3e9-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-168">Boolean</span></span>|<span data-ttu-id="7b3e9-169">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="7b3e9-169">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="7b3e9-170">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="7b3e9-170">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="7b3e9-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-171">Boolean</span></span>|<span data-ttu-id="7b3e9-172">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-172">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="7b3e9-173">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="7b3e9-173">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="7b3e9-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-174">Boolean</span></span>|<span data-ttu-id="7b3e9-175">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="7b3e9-175">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="7b3e9-176">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="7b3e9-176">firewallCertificateRevocationListCheckMethod</span></span>|<span data-ttu-id="7b3e9-177">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-177">String</span></span>|<span data-ttu-id="7b3e9-178">Укажите, как следует применять список отзыва сертификатов. Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-178">Specify how the certificate revocation list is to be enforced Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="7b3e9-179">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="7b3e9-179">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="7b3e9-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-180">Boolean</span></span>|<span data-ttu-id="7b3e9-181">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="7b3e9-181">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="7b3e9-182">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="7b3e9-182">firewallPacketQueueingMethod</span></span>|<span data-ttu-id="7b3e9-183">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-183">String</span></span>|<span data-ttu-id="7b3e9-184">Настраивает организацию очереди пакетов в сценарии туннельного шлюза. Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-184">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="7b3e9-185">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="7b3e9-185">firewallProfileDomain</span></span>|[<span data-ttu-id="7b3e9-186">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7b3e9-186">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="7b3e9-187">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="7b3e9-187">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="7b3e9-188">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="7b3e9-188">firewallProfilePublic</span></span>|[<span data-ttu-id="7b3e9-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7b3e9-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="7b3e9-190">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="7b3e9-190">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="7b3e9-191">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="7b3e9-191">firewallProfilePrivate</span></span>|[<span data-ttu-id="7b3e9-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7b3e9-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="7b3e9-193">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="7b3e9-193">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="7b3e9-194">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="7b3e9-194">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="7b3e9-195">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b3e9-195">String collection</span></span>|<span data-ttu-id="7b3e9-196">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="7b3e9-196">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="7b3e9-197">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="7b3e9-197">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="7b3e9-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b3e9-198">String collection</span></span>|<span data-ttu-id="7b3e9-199">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="7b3e9-199">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="7b3e9-200">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="7b3e9-200">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="7b3e9-201">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b3e9-201">String collection</span></span>|<span data-ttu-id="7b3e9-202">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="7b3e9-202">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="7b3e9-203">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="7b3e9-203">defenderExploitProtectionXml</span></span>|<span data-ttu-id="7b3e9-204">Binary</span><span class="sxs-lookup"><span data-stu-id="7b3e9-204">Binary</span></span>|<span data-ttu-id="7b3e9-205">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-205">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="7b3e9-206">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="7b3e9-206">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="7b3e9-207">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-207">String</span></span>|<span data-ttu-id="7b3e9-208">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-208">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="7b3e9-209">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="7b3e9-209">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="7b3e9-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-210">Boolean</span></span>|<span data-ttu-id="7b3e9-211">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-211">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="7b3e9-212">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="7b3e9-212">appLockerApplicationControl</span></span>|<span data-ttu-id="7b3e9-213">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-213">String</span></span>|<span data-ttu-id="7b3e9-214">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-214">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="7b3e9-215">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-215">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="7b3e9-216">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="7b3e9-216">smartScreenEnableInShell</span></span>|<span data-ttu-id="7b3e9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-217">Boolean</span></span>|<span data-ttu-id="7b3e9-218">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-218">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="7b3e9-219">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="7b3e9-219">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="7b3e9-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-220">Boolean</span></span>|<span data-ttu-id="7b3e9-221">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-221">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="7b3e9-222">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="7b3e9-222">applicationGuardEnabled</span></span>|<span data-ttu-id="7b3e9-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-223">Boolean</span></span>|<span data-ttu-id="7b3e9-224">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="7b3e9-224">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="7b3e9-225">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="7b3e9-225">applicationGuardBlockFileTransfer</span></span>|<span data-ttu-id="7b3e9-226">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-226">String</span></span>|<span data-ttu-id="7b3e9-227">Позволяет заблокировать передачу изображений и текстовых файлов через буфер обмена. Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-227">Block clipboard to transfer image file, text file or neither of them Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="7b3e9-228">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="7b3e9-228">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="7b3e9-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-229">Boolean</span></span>|<span data-ttu-id="7b3e9-230">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-230">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="7b3e9-231">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="7b3e9-231">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="7b3e9-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-232">Boolean</span></span>|<span data-ttu-id="7b3e9-233">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="7b3e9-233">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="7b3e9-234">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="7b3e9-234">applicationGuardForceAuditing</span></span>|<span data-ttu-id="7b3e9-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-235">Boolean</span></span>|<span data-ttu-id="7b3e9-236">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-236">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="7b3e9-237">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="7b3e9-237">applicationGuardBlockClipboardSharing</span></span>|<span data-ttu-id="7b3e9-238">String</span><span class="sxs-lookup"><span data-stu-id="7b3e9-238">String</span></span>|<span data-ttu-id="7b3e9-239">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-239">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="7b3e9-240">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-240">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="7b3e9-241">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="7b3e9-241">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="7b3e9-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-242">Boolean</span></span>|<span data-ttu-id="7b3e9-243">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-243">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="7b3e9-244">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="7b3e9-244">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="7b3e9-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-245">Boolean</span></span>|<span data-ttu-id="7b3e9-246">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-246">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="7b3e9-247">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="7b3e9-247">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="7b3e9-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-248">Boolean</span></span>|<span data-ttu-id="7b3e9-249">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-249">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="7b3e9-250">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="7b3e9-250">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="7b3e9-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-251">Boolean</span></span>|<span data-ttu-id="7b3e9-252">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-252">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="7b3e9-253">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="7b3e9-253">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="7b3e9-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-254">Boolean</span></span>|<span data-ttu-id="7b3e9-255">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-255">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="7b3e9-256">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="7b3e9-256">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="7b3e9-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-257">Boolean</span></span>|<span data-ttu-id="7b3e9-258">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-258">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="7b3e9-259">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-259">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="7b3e9-260">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="7b3e9-260">bitLockerEncryptDevice</span></span>|<span data-ttu-id="7b3e9-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b3e9-261">Boolean</span></span>|<span data-ttu-id="7b3e9-262">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="7b3e9-263">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="7b3e9-263">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="7b3e9-264">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="7b3e9-264">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="7b3e9-265">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-265">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="7b3e9-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b3e9-266">Response</span></span>
<span data-ttu-id="7b3e9-267">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-267">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b3e9-268">Пример</span><span class="sxs-lookup"><span data-stu-id="7b3e9-268">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b3e9-269">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b3e9-269">Request</span></span>
<span data-ttu-id="7b3e9-270">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-270">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4309

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="7b3e9-271">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b3e9-271">Response</span></span>
<span data-ttu-id="7b3e9-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b3e9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



