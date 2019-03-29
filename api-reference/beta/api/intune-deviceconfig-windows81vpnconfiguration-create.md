---
title: Создание windows81VpnConfiguration
description: Создание нового объекта windows81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98724226d8ca109b30e586760a402702cbb12128
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971299"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="2ad6a-103">Создание windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ad6a-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="2ad6a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ad6a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad6a-106">Создание нового объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2ad6a-106">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ad6a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ad6a-107">Prerequisites</span></span>
<span data-ttu-id="2ad6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ad6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ad6a-110">Permission type</span></span>|<span data-ttu-id="2ad6a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ad6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ad6a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ad6a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ad6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ad6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-115">Not supported.</span></span>|
|<span data-ttu-id="2ad6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ad6a-116">Application</span></span>|<span data-ttu-id="2ad6a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ad6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ad6a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2ad6a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ad6a-119">Request headers</span></span>
|<span data-ttu-id="2ad6a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ad6a-120">Header</span></span>|<span data-ttu-id="2ad6a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2ad6a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ad6a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ad6a-122">Authorization</span></span>|<span data-ttu-id="2ad6a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ad6a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2ad6a-124">Accept</span></span>|<span data-ttu-id="2ad6a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ad6a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ad6a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ad6a-126">Request body</span></span>
<span data-ttu-id="2ad6a-127">В тексте запроса добавьте представление объекта windows81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-127">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="2ad6a-128">В следующей таблице приведены свойства, необходимые при создании windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-128">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="2ad6a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ad6a-129">Property</span></span>|<span data-ttu-id="2ad6a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad6a-130">Type</span></span>|<span data-ttu-id="2ad6a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad6a-132">id</span><span class="sxs-lookup"><span data-stu-id="2ad6a-132">id</span></span>|<span data-ttu-id="2ad6a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2ad6a-133">String</span></span>|<span data-ttu-id="2ad6a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-134">Key of the entity.</span></span> <span data-ttu-id="2ad6a-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad6a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2ad6a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad6a-137">DateTimeOffset</span></span>|<span data-ttu-id="2ad6a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2ad6a-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ad6a-140">roleScopeTagIds</span></span>|<span data-ttu-id="2ad6a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ad6a-141">String collection</span></span>|<span data-ttu-id="2ad6a-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2ad6a-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2ad6a-144">supportsScopeTags</span></span>|<span data-ttu-id="2ad6a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad6a-145">Boolean</span></span>|<span data-ttu-id="2ad6a-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2ad6a-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2ad6a-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2ad6a-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-149">This property is read-only.</span></span> <span data-ttu-id="2ad6a-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad6a-151">createdDateTime</span></span>|<span data-ttu-id="2ad6a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad6a-152">DateTimeOffset</span></span>|<span data-ttu-id="2ad6a-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-153">DateTime the object was created.</span></span> <span data-ttu-id="2ad6a-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-155">description</span><span class="sxs-lookup"><span data-stu-id="2ad6a-155">description</span></span>|<span data-ttu-id="2ad6a-156">String</span><span class="sxs-lookup"><span data-stu-id="2ad6a-156">String</span></span>|<span data-ttu-id="2ad6a-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ad6a-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2ad6a-159">displayName</span></span>|<span data-ttu-id="2ad6a-160">String</span><span class="sxs-lookup"><span data-stu-id="2ad6a-160">String</span></span>|<span data-ttu-id="2ad6a-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ad6a-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-163">version</span><span class="sxs-lookup"><span data-stu-id="2ad6a-163">version</span></span>|<span data-ttu-id="2ad6a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad6a-164">Int32</span></span>|<span data-ttu-id="2ad6a-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-165">Version of the device configuration.</span></span> <span data-ttu-id="2ad6a-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad6a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="2ad6a-167">connectionName</span></span>|<span data-ttu-id="2ad6a-168">String</span><span class="sxs-lookup"><span data-stu-id="2ad6a-168">String</span></span>|<span data-ttu-id="2ad6a-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-169">Connection name displayed to the user.</span></span> <span data-ttu-id="2ad6a-170">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-171">серверами</span><span class="sxs-lookup"><span data-stu-id="2ad6a-171">servers</span></span>|<span data-ttu-id="2ad6a-172">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="2ad6a-173">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="2ad6a-174">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="2ad6a-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2ad6a-176">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-177">customXml</span><span class="sxs-lookup"><span data-stu-id="2ad6a-177">customXml</span></span>|<span data-ttu-id="2ad6a-178">Binary</span><span class="sxs-lookup"><span data-stu-id="2ad6a-178">Binary</span></span>|<span data-ttu-id="2ad6a-179">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="2ad6a-180">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad6a-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ad6a-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="2ad6a-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="2ad6a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad6a-182">Boolean</span></span>|<span data-ttu-id="2ad6a-183">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="2ad6a-184">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-184">This property is read-only.</span></span>|
|<span data-ttu-id="2ad6a-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="2ad6a-185">connectionType</span></span>|[<span data-ttu-id="2ad6a-186">Виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="2ad6a-186">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="2ad6a-187">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-187">Connection type.</span></span> <span data-ttu-id="2ad6a-188">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="2ad6a-189">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="2ad6a-189">loginGroupOrDomain</span></span>|<span data-ttu-id="2ad6a-190">String</span><span class="sxs-lookup"><span data-stu-id="2ad6a-190">String</span></span>|<span data-ttu-id="2ad6a-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="2ad6a-192">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="2ad6a-192">enableSplitTunneling</span></span>|<span data-ttu-id="2ad6a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad6a-193">Boolean</span></span>|<span data-ttu-id="2ad6a-194">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-194">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="2ad6a-195">проксисервер</span><span class="sxs-lookup"><span data-stu-id="2ad6a-195">proxyServer</span></span>|[<span data-ttu-id="2ad6a-196">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2ad6a-196">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="2ad6a-197">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-197">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="2ad6a-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ad6a-198">Response</span></span>
<span data-ttu-id="2ad6a-199">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-199">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ad6a-200">Пример</span><span class="sxs-lookup"><span data-stu-id="2ad6a-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ad6a-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ad6a-201">Request</span></span>
<span data-ttu-id="2ad6a-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1015

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="2ad6a-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ad6a-203">Response</span></span>
<span data-ttu-id="2ad6a-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ad6a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1187

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




