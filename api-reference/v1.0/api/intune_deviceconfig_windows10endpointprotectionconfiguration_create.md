# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="d23f5-101">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d23f5-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="d23f5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d23f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d23f5-103">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-103">Create a new [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d23f5-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d23f5-104">Prerequisites</span></span>
<span data-ttu-id="d23f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d23f5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d23f5-107">Permission type</span></span>|<span data-ttu-id="d23f5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d23f5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d23f5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d23f5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d23f5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23f5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d23f5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d23f5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d23f5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d23f5-112">Not supported.</span></span>|
|<span data-ttu-id="d23f5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d23f5-113">Application</span></span>|<span data-ttu-id="d23f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d23f5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d23f5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d23f5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d23f5-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d23f5-116">Request headers</span></span>
|<span data-ttu-id="d23f5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d23f5-117">Header</span></span>|<span data-ttu-id="d23f5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d23f5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d23f5-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d23f5-119">Authorization</span></span>|<span data-ttu-id="d23f5-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="d23f5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d23f5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d23f5-121">Accept</span></span>|<span data-ttu-id="d23f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d23f5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d23f5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d23f5-123">Request body</span></span>
<span data-ttu-id="d23f5-124">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d23f5-124">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="d23f5-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d23f5-125">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="d23f5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d23f5-126">Property</span></span>|<span data-ttu-id="d23f5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d23f5-127">Type</span></span>|<span data-ttu-id="d23f5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d23f5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d23f5-129">id</span><span class="sxs-lookup"><span data-stu-id="d23f5-129">id</span></span>|<span data-ttu-id="d23f5-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d23f5-130">String</span></span>|<span data-ttu-id="d23f5-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d23f5-131">Key of the entity.</span></span> <span data-ttu-id="d23f5-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d23f5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d23f5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d23f5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d23f5-134">DateTimeOffset</span></span>|<span data-ttu-id="d23f5-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d23f5-135">DateTime the object was last modified.</span></span> <span data-ttu-id="d23f5-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d23f5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d23f5-137">createdDateTime</span></span>|<span data-ttu-id="d23f5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d23f5-138">DateTimeOffset</span></span>|<span data-ttu-id="d23f5-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d23f5-139">DateTime the object was created.</span></span> <span data-ttu-id="d23f5-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d23f5-141">description</span><span class="sxs-lookup"><span data-stu-id="d23f5-141">description</span></span>|<span data-ttu-id="d23f5-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d23f5-142">String</span></span>|<span data-ttu-id="d23f5-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d23f5-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d23f5-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d23f5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d23f5-145">displayName</span></span>|<span data-ttu-id="d23f5-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d23f5-146">String</span></span>|<span data-ttu-id="d23f5-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d23f5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d23f5-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d23f5-149">version</span><span class="sxs-lookup"><span data-stu-id="d23f5-149">version</span></span>|<span data-ttu-id="d23f5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d23f5-150">Int32</span></span>|<span data-ttu-id="d23f5-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d23f5-151">Version of the device configuration.</span></span> <span data-ttu-id="d23f5-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d23f5-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d23f5-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="d23f5-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="d23f5-154">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-154">Boolean</span></span>|<span data-ttu-id="d23f5-155">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="d23f5-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="d23f5-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d23f5-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="d23f5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d23f5-157">Int32</span></span>|<span data-ttu-id="d23f5-158">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="d23f5-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="d23f5-159">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="d23f5-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="d23f5-160">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="d23f5-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="d23f5-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d23f5-161">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="d23f5-162">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d23f5-162">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="d23f5-p109">Выберите кодировку с общим ключом, которую следует использовать. Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p109">Select the preshared key encoding to be used Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="d23f5-165">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="d23f5-165">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="d23f5-166">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-166">Boolean</span></span>|<span data-ttu-id="d23f5-167">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="d23f5-167">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d23f5-168">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="d23f5-168">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="d23f5-169">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-169">Boolean</span></span>|<span data-ttu-id="d23f5-170">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="d23f5-170">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="d23f5-171">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="d23f5-171">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="d23f5-172">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-172">Boolean</span></span>|<span data-ttu-id="d23f5-173">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="d23f5-173">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d23f5-174">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="d23f5-174">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="d23f5-175">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-175">Boolean</span></span>|<span data-ttu-id="d23f5-176">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="d23f5-176">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="d23f5-177">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d23f5-177">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="d23f5-178">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="d23f5-178">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="d23f5-p110">Укажите, как будет применяться список отзыва сертификатов. Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p110">Specify how the certificate revocation list is to be enforced Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="d23f5-181">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="d23f5-181">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="d23f5-182">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-182">Boolean</span></span>|<span data-ttu-id="d23f5-183">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="d23f5-183">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="d23f5-184">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d23f5-184">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="d23f5-185">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d23f5-185">firewallPacketQueueingMethodType</span></span>](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|<span data-ttu-id="d23f5-p111">Настраивает, как будет применяться пакетная очередность в сценарии туннельного шлюза. Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p111">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="d23f5-188">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="d23f5-188">firewallProfileDomain</span></span>|[<span data-ttu-id="d23f5-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d23f5-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="d23f5-190">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="d23f5-190">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="d23f5-191">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="d23f5-191">firewallProfilePublic</span></span>|[<span data-ttu-id="d23f5-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d23f5-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="d23f5-193">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="d23f5-193">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="d23f5-194">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="d23f5-194">firewallProfilePrivate</span></span>|[<span data-ttu-id="d23f5-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d23f5-195">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="d23f5-196">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="d23f5-196">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="d23f5-197">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="d23f5-197">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="d23f5-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d23f5-198">String collection</span></span>|<span data-ttu-id="d23f5-199">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="d23f5-199">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="d23f5-200">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="d23f5-200">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="d23f5-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d23f5-201">String collection</span></span>|<span data-ttu-id="d23f5-202">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="d23f5-202">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="d23f5-203">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="d23f5-203">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="d23f5-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d23f5-204">String collection</span></span>|<span data-ttu-id="d23f5-205">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="d23f5-205">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="d23f5-206">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="d23f5-206">defenderExploitProtectionXml</span></span>|<span data-ttu-id="d23f5-207">Binary</span><span class="sxs-lookup"><span data-stu-id="d23f5-207">Binary</span></span>|<span data-ttu-id="d23f5-208">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="d23f5-208">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="d23f5-209">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="d23f5-209">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="d23f5-210">String (строка)</span><span class="sxs-lookup"><span data-stu-id="d23f5-210">String</span></span>|<span data-ttu-id="d23f5-211">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="d23f5-211">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="d23f5-212">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="d23f5-212">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="d23f5-213">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-213">Boolean</span></span>|<span data-ttu-id="d23f5-214">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="d23f5-214">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="d23f5-215">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="d23f5-215">appLockerApplicationControl</span></span>|[<span data-ttu-id="d23f5-216">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="d23f5-216">appLockerApplicationControlType</span></span>](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|<span data-ttu-id="d23f5-p112">Позволяет администратору выбрать, какие типы приложений разрешены на устройствах. Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p112">Enables the Admin to choose what types of app to allow on devices. The possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="d23f5-219">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="d23f5-219">smartScreenEnableInShell</span></span>|<span data-ttu-id="d23f5-220">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-220">Boolean</span></span>|<span data-ttu-id="d23f5-221">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="d23f5-221">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="d23f5-222">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="d23f5-222">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="d23f5-223">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-223">Boolean</span></span>|<span data-ttu-id="d23f5-224">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="d23f5-224">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="d23f5-225">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="d23f5-225">applicationGuardEnabled</span></span>|<span data-ttu-id="d23f5-226">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-226">Boolean</span></span>|<span data-ttu-id="d23f5-227">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="d23f5-227">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="d23f5-228">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="d23f5-228">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="d23f5-229">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="d23f5-229">applicationGuardBlockFileTransferType</span></span>](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|<span data-ttu-id="d23f5-p113">Позволяет заблокировать передачу изображений и текстовых файлов через буфер обмена. Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p113">Block clipboard to transfer image file, text file or neither of them Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="d23f5-232">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="d23f5-232">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="d23f5-233">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-233">Boolean</span></span>|<span data-ttu-id="d23f5-234">Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="d23f5-234">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="d23f5-235">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="d23f5-235">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="d23f5-236">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-236">Boolean</span></span>|<span data-ttu-id="d23f5-237">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="d23f5-237">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="d23f5-238">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="d23f5-238">applicationGuardForceAuditing</span></span>|<span data-ttu-id="d23f5-239">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-239">Boolean</span></span>|<span data-ttu-id="d23f5-240">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="d23f5-240">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="d23f5-241">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d23f5-241">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="d23f5-242">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d23f5-242">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="d23f5-p114">Позволяет заблокировать обмен данными от основного приложения к контейнеру или в обратном направлении через буфер обмена. Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p114">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways. The possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="d23f5-245">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="d23f5-245">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="d23f5-246">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-246">Boolean</span></span>|<span data-ttu-id="d23f5-247">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d23f5-247">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="d23f5-248">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="d23f5-248">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="d23f5-249">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-249">Boolean</span></span>|<span data-ttu-id="d23f5-250">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d23f5-250">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="d23f5-251">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="d23f5-251">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="d23f5-252">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-252">Boolean</span></span>|<span data-ttu-id="d23f5-253">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d23f5-253">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="d23f5-254">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="d23f5-254">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="d23f5-255">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-255">Boolean</span></span>|<span data-ttu-id="d23f5-256">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d23f5-256">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="d23f5-257">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="d23f5-257">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="d23f5-258">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-258">Boolean</span></span>|<span data-ttu-id="d23f5-259">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="d23f5-259">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="d23f5-260">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="d23f5-260">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="d23f5-261">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-261">Boolean</span></span>|<span data-ttu-id="d23f5-262">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d23f5-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="d23f5-263">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="d23f5-263">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="d23f5-264">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="d23f5-264">bitLockerEncryptDevice</span></span>|<span data-ttu-id="d23f5-265">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d23f5-265">Boolean</span></span>|<span data-ttu-id="d23f5-266">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d23f5-266">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="d23f5-267">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d23f5-267">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="d23f5-268">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d23f5-268">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="d23f5-269">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="d23f5-269">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d23f5-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="d23f5-270">Response</span></span>
<span data-ttu-id="d23f5-271">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d23f5-271">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d23f5-272">Пример</span><span class="sxs-lookup"><span data-stu-id="d23f5-272">Example</span></span>
### <a name="request"></a><span data-ttu-id="d23f5-273">Запрос</span><span class="sxs-lookup"><span data-stu-id="d23f5-273">Request</span></span>
<span data-ttu-id="d23f5-274">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d23f5-274">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d23f5-275">Ответ</span><span class="sxs-lookup"><span data-stu-id="d23f5-275">Response</span></span>
<span data-ttu-id="d23f5-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d23f5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








