---
title: Создание windowsWifiEnterpriseEAPConfiguration
description: Создание нового объекта windowsWifiEnterpriseEAPConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f3ab25f8d74546bd75d4fdc65cc5306fd4c48d25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413481"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="a7638-103">Создание windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7638-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="a7638-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7638-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7638-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7638-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7638-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7638-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7638-107">Создание нового объекта [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7638-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7638-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a7638-108">Prerequisites</span></span>
<span data-ttu-id="a7638-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7638-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7638-111">Permission type</span></span>|<span data-ttu-id="a7638-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7638-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7638-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7638-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7638-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7638-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7638-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7638-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7638-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7638-116">Not supported.</span></span>|
|<span data-ttu-id="a7638-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7638-117">Application</span></span>|<span data-ttu-id="a7638-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7638-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7638-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7638-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a7638-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7638-120">Request headers</span></span>
|<span data-ttu-id="a7638-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7638-121">Header</span></span>|<span data-ttu-id="a7638-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7638-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7638-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7638-123">Authorization</span></span>|<span data-ttu-id="a7638-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a7638-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7638-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7638-125">Accept</span></span>|<span data-ttu-id="a7638-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7638-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7638-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7638-127">Request body</span></span>
<span data-ttu-id="a7638-128">В тексте запроса укажите представление JSON для объекта windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7638-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="a7638-129">В следующей таблице показаны свойства, которые необходимы для создания windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7638-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="a7638-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7638-130">Property</span></span>|<span data-ttu-id="a7638-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a7638-131">Type</span></span>|<span data-ttu-id="a7638-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a7638-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7638-133">id</span><span class="sxs-lookup"><span data-stu-id="a7638-133">id</span></span>|<span data-ttu-id="a7638-134">String</span><span class="sxs-lookup"><span data-stu-id="a7638-134">String</span></span>|<span data-ttu-id="a7638-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7638-135">Key of the entity.</span></span> <span data-ttu-id="a7638-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7638-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a7638-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7638-138">DateTimeOffset</span></span>|<span data-ttu-id="a7638-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a7638-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a7638-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7638-141">roleScopeTagIds</span></span>|<span data-ttu-id="a7638-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a7638-142">String collection</span></span>|<span data-ttu-id="a7638-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a7638-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7638-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7638-145">supportsScopeTags</span></span>|<span data-ttu-id="a7638-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-146">Boolean</span></span>|<span data-ttu-id="a7638-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="a7638-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7638-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="a7638-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7638-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a7638-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7638-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7638-150">This property is read-only.</span></span> <span data-ttu-id="a7638-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7638-152">createdDateTime</span></span>|<span data-ttu-id="a7638-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7638-153">DateTimeOffset</span></span>|<span data-ttu-id="a7638-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a7638-154">DateTime the object was created.</span></span> <span data-ttu-id="a7638-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-156">description</span><span class="sxs-lookup"><span data-stu-id="a7638-156">description</span></span>|<span data-ttu-id="a7638-157">String</span><span class="sxs-lookup"><span data-stu-id="a7638-157">String</span></span>|<span data-ttu-id="a7638-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7638-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7638-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a7638-160">displayName</span></span>|<span data-ttu-id="a7638-161">String</span><span class="sxs-lookup"><span data-stu-id="a7638-161">String</span></span>|<span data-ttu-id="a7638-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7638-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7638-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-164">version</span><span class="sxs-lookup"><span data-stu-id="a7638-164">version</span></span>|<span data-ttu-id="a7638-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a7638-165">Int32</span></span>|<span data-ttu-id="a7638-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7638-166">Version of the device configuration.</span></span> <span data-ttu-id="a7638-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7638-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a7638-168">preSharedKey</span></span>|<span data-ttu-id="a7638-169">String</span><span class="sxs-lookup"><span data-stu-id="a7638-169">String</span></span>|<span data-ttu-id="a7638-170">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a7638-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="a7638-171">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-171">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-172">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a7638-172">wifiSecurityType</span></span>|[<span data-ttu-id="a7638-173">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a7638-173">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="a7638-174">Укажите тип безопасности Wifi.</span><span class="sxs-lookup"><span data-stu-id="a7638-174">Specify the Wifi Security Type.</span></span> <span data-ttu-id="a7638-175">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-175">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="a7638-176">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="a7638-176">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="a7638-177">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="a7638-177">meteredConnectionLimit</span></span>|[<span data-ttu-id="a7638-178">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="a7638-178">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="a7638-179">Задать тип ограничение лимитным тарифным планом подключения для Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a7638-179">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="a7638-180">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7638-180">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="a7638-181">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="a7638-181">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="a7638-182">SSID</span><span class="sxs-lookup"><span data-stu-id="a7638-182">ssid</span></span>|<span data-ttu-id="a7638-183">String</span><span class="sxs-lookup"><span data-stu-id="a7638-183">String</span></span>|<span data-ttu-id="a7638-184">Укажите SSID Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a7638-184">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="a7638-185">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-185">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-186">networkName</span><span class="sxs-lookup"><span data-stu-id="a7638-186">networkName</span></span>|<span data-ttu-id="a7638-187">String</span><span class="sxs-lookup"><span data-stu-id="a7638-187">String</span></span>|<span data-ttu-id="a7638-188">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="a7638-188">Specify the network configuration name.</span></span> <span data-ttu-id="a7638-189">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-189">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-190">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a7638-190">connectAutomatically</span></span>|<span data-ttu-id="a7638-191">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-191">Boolean</span></span>|<span data-ttu-id="a7638-192">Укажите, будет ли Wi-Fi следует автоматически подключаться при работе в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="a7638-192">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="a7638-193">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-193">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-194">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="a7638-194">connectToPreferredNetwork</span></span>|<span data-ttu-id="a7638-195">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-195">Boolean</span></span>|<span data-ttu-id="a7638-196">Укажите, должны ли Wi-Fi подключаться к более подходящей сети, если уже подключен этой.</span><span class="sxs-lookup"><span data-stu-id="a7638-196">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="a7638-197">Требуется ConnectAutomatically значение true.</span><span class="sxs-lookup"><span data-stu-id="a7638-197">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="a7638-198">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-198">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-199">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a7638-199">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a7638-200">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-200">Boolean</span></span>|<span data-ttu-id="a7638-201">Укажите, автоматически подключения Wi-Fi даже когда не передают SSID.</span><span class="sxs-lookup"><span data-stu-id="a7638-201">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="a7638-202">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-202">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-203">proxySetting</span><span class="sxs-lookup"><span data-stu-id="a7638-203">proxySetting</span></span>|[<span data-ttu-id="a7638-204">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="a7638-204">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="a7638-205">Укажите параметры для конфигурации Wi-Fi унаследованные от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a7638-205">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="a7638-206">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="a7638-206">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="a7638-207">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="a7638-207">proxyManualAddress</span></span>|<span data-ttu-id="a7638-208">String</span><span class="sxs-lookup"><span data-stu-id="a7638-208">String</span></span>|<span data-ttu-id="a7638-209">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a7638-209">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="a7638-210">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-211">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="a7638-211">proxyManualPort</span></span>|<span data-ttu-id="a7638-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a7638-212">Int32</span></span>|<span data-ttu-id="a7638-213">Указание порта для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a7638-213">Specify the port for the proxy server.</span></span> <span data-ttu-id="a7638-214">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-215">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="a7638-215">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="a7638-216">String</span><span class="sxs-lookup"><span data-stu-id="a7638-216">String</span></span>|<span data-ttu-id="a7638-217">Укажите URL-адрес для сценария настройки сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a7638-217">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="a7638-218">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-218">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="a7638-219">forceFIPSCompliance</span></span>|<span data-ttu-id="a7638-220">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-220">Boolean</span></span>|<span data-ttu-id="a7638-221">Укажите необходимость проверки соответствия требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="a7638-221">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="a7638-222">Наследуется от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7638-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="a7638-223">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="a7638-223">networkSingleSignOn</span></span>|[<span data-ttu-id="a7638-224">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="a7638-224">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="a7638-225">Укажите на тип сети единого входа.</span><span class="sxs-lookup"><span data-stu-id="a7638-225">Specify the network single sign on type.</span></span> <span data-ttu-id="a7638-226">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="a7638-226">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="a7638-227">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="a7638-227">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="a7638-228">Int32</span><span class="sxs-lookup"><span data-stu-id="a7638-228">Int32</span></span>|<span data-ttu-id="a7638-229">Укажите проверки подлинности на максимальное время ожидания (в секундах).</span><span class="sxs-lookup"><span data-stu-id="a7638-229">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="a7638-230">Допустимые значения: 1-120</span><span class="sxs-lookup"><span data-stu-id="a7638-230">Valid range: 1-120</span></span>|
|<span data-ttu-id="a7638-231">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="a7638-231">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="a7638-232">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-232">Boolean</span></span>|<span data-ttu-id="a7638-233">Укажите, следует ли Wi-Fi запрашивать дополнительную проверку подлинности учетных данных.</span><span class="sxs-lookup"><span data-stu-id="a7638-233">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="a7638-234">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="a7638-234">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="a7638-235">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-235">Boolean</span></span>|<span data-ttu-id="a7638-236">Укажите, следует ли Wi-Fi включить кэширование парных главных ключей.</span><span class="sxs-lookup"><span data-stu-id="a7638-236">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="a7638-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a7638-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="a7638-238">Int32</span><span class="sxs-lookup"><span data-stu-id="a7638-238">Int32</span></span>|<span data-ttu-id="a7638-239">Укажите максимальный парных главный ключ кэша времени (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a7638-239">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="a7638-240">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="a7638-240">Valid range: 5-1440</span></span>|
|<span data-ttu-id="a7638-241">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="a7638-241">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="a7638-242">Int32</span><span class="sxs-lookup"><span data-stu-id="a7638-242">Int32</span></span>|<span data-ttu-id="a7638-243">Укажите максимальное число парных главных ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="a7638-243">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="a7638-244">Допустимые значения: 1-255</span><span class="sxs-lookup"><span data-stu-id="a7638-244">Valid range: 1-255</span></span>|
|<span data-ttu-id="a7638-245">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="a7638-245">enablePreAuthentication</span></span>|<span data-ttu-id="a7638-246">Логический</span><span class="sxs-lookup"><span data-stu-id="a7638-246">Boolean</span></span>|<span data-ttu-id="a7638-247">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="a7638-247">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="a7638-248">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="a7638-248">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="a7638-249">Int32</span><span class="sxs-lookup"><span data-stu-id="a7638-249">Int32</span></span>|<span data-ttu-id="a7638-250">Укажите максимальный попыток предварительной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a7638-250">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="a7638-251">Допустимые значения: 1-16</span><span class="sxs-lookup"><span data-stu-id="a7638-251">Valid range: 1-16</span></span>|
|<span data-ttu-id="a7638-252">eapType</span><span class="sxs-lookup"><span data-stu-id="a7638-252">eapType</span></span>|[<span data-ttu-id="a7638-253">eapType</span><span class="sxs-lookup"><span data-stu-id="a7638-253">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="a7638-254">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="a7638-254">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="a7638-255">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="a7638-255">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="a7638-256">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="a7638-256">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="a7638-257">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="a7638-257">trustedServerCertificateNames</span></span>|<span data-ttu-id="a7638-258">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a7638-258">String collection</span></span>|<span data-ttu-id="a7638-259">Укажите имена сертификат доверенного сервера.</span><span class="sxs-lookup"><span data-stu-id="a7638-259">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="a7638-260">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a7638-260">authenticationMethod</span></span>|[<span data-ttu-id="a7638-261">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a7638-261">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="a7638-262">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a7638-262">Specify the authentication method.</span></span> <span data-ttu-id="a7638-263">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="a7638-263">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="a7638-264">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="a7638-264">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="a7638-265">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="a7638-265">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="a7638-266">Укажите внутренний протокол EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="a7638-266">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="a7638-267">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="a7638-267">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="a7638-268">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="a7638-268">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="a7638-269">String</span><span class="sxs-lookup"><span data-stu-id="a7638-269">String</span></span>|<span data-ttu-id="a7638-270">Укажите строку, которую нужно заменить имена пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="a7638-270">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="a7638-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7638-271">Response</span></span>
<span data-ttu-id="a7638-272">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7638-272">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7638-273">Пример</span><span class="sxs-lookup"><span data-stu-id="a7638-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7638-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7638-274">Request</span></span>
<span data-ttu-id="a7638-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7638-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="a7638-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7638-276">Response</span></span>
<span data-ttu-id="a7638-p132">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7638-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




