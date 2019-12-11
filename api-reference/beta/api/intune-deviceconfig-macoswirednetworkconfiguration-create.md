---
title: Создание Макосвиреднетворкконфигуратион
description: Создание нового объекта Макосвиреднетворкконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51644540e8026e310c76810b5cc3f16d6697c3bc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948032"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="7b917-103">Создание Макосвиреднетворкконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7b917-103">Create macOSWiredNetworkConfiguration</span></span>

> <span data-ttu-id="7b917-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b917-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b917-106">Создание нового объекта [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7b917-106">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b917-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b917-107">Prerequisites</span></span>
<span data-ttu-id="7b917-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b917-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b917-110">Permission type</span></span>|<span data-ttu-id="7b917-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b917-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b917-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b917-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b917-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b917-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b917-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b917-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b917-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b917-115">Not supported.</span></span>|
|<span data-ttu-id="7b917-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b917-116">Application</span></span>|<span data-ttu-id="7b917-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b917-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b917-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b917-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b917-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b917-119">Request headers</span></span>
|<span data-ttu-id="7b917-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b917-120">Header</span></span>|<span data-ttu-id="7b917-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7b917-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b917-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b917-122">Authorization</span></span>|<span data-ttu-id="7b917-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b917-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b917-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7b917-124">Accept</span></span>|<span data-ttu-id="7b917-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b917-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b917-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b917-126">Request body</span></span>
<span data-ttu-id="7b917-127">В тексте запроса добавьте представление объекта Макосвиреднетворкконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b917-127">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="7b917-128">В следующей таблице приведены свойства, необходимые при создании Макосвиреднетворкконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="7b917-128">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="7b917-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b917-129">Property</span></span>|<span data-ttu-id="7b917-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7b917-130">Type</span></span>|<span data-ttu-id="7b917-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7b917-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b917-132">id</span><span class="sxs-lookup"><span data-stu-id="7b917-132">id</span></span>|<span data-ttu-id="7b917-133">String</span><span class="sxs-lookup"><span data-stu-id="7b917-133">String</span></span>|<span data-ttu-id="7b917-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b917-134">Key of the entity.</span></span> <span data-ttu-id="7b917-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b917-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7b917-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b917-137">DateTimeOffset</span></span>|<span data-ttu-id="7b917-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7b917-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7b917-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b917-140">roleScopeTagIds</span></span>|<span data-ttu-id="7b917-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b917-141">String collection</span></span>|<span data-ttu-id="7b917-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7b917-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b917-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7b917-144">supportsScopeTags</span></span>|<span data-ttu-id="7b917-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b917-145">Boolean</span></span>|<span data-ttu-id="7b917-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7b917-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b917-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7b917-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b917-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7b917-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b917-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7b917-149">This property is read-only.</span></span> <span data-ttu-id="7b917-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7b917-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7b917-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7b917-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7b917-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7b917-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7b917-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7b917-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7b917-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7b917-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7b917-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7b917-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7b917-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7b917-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7b917-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7b917-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7b917-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7b917-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7b917-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b917-163">createdDateTime</span></span>|<span data-ttu-id="7b917-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b917-164">DateTimeOffset</span></span>|<span data-ttu-id="7b917-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7b917-165">DateTime the object was created.</span></span> <span data-ttu-id="7b917-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-167">description</span><span class="sxs-lookup"><span data-stu-id="7b917-167">description</span></span>|<span data-ttu-id="7b917-168">String</span><span class="sxs-lookup"><span data-stu-id="7b917-168">String</span></span>|<span data-ttu-id="7b917-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b917-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b917-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7b917-171">displayName</span></span>|<span data-ttu-id="7b917-172">Строка</span><span class="sxs-lookup"><span data-stu-id="7b917-172">String</span></span>|<span data-ttu-id="7b917-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b917-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b917-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-175">version</span><span class="sxs-lookup"><span data-stu-id="7b917-175">version</span></span>|<span data-ttu-id="7b917-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7b917-176">Int32</span></span>|<span data-ttu-id="7b917-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b917-177">Version of the device configuration.</span></span> <span data-ttu-id="7b917-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b917-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b917-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="7b917-179">networkName</span></span>|<span data-ttu-id="7b917-180">Строка</span><span class="sxs-lookup"><span data-stu-id="7b917-180">String</span></span>|<span data-ttu-id="7b917-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="7b917-181">Network Name</span></span>|
|<span data-ttu-id="7b917-182">нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="7b917-182">networkInterface</span></span>|[<span data-ttu-id="7b917-183">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="7b917-183">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="7b917-184">Сетевой интерфейс.</span><span class="sxs-lookup"><span data-stu-id="7b917-184">Network interface.</span></span> <span data-ttu-id="7b917-185">Возможные значения: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="7b917-185">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="7b917-186">еаптипе</span><span class="sxs-lookup"><span data-stu-id="7b917-186">eapType</span></span>|[<span data-ttu-id="7b917-187">еаптипе</span><span class="sxs-lookup"><span data-stu-id="7b917-187">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="7b917-188">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="7b917-188">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="7b917-189">Указывает тип протокола EAP, установленный для проводной сети.</span><span class="sxs-lookup"><span data-stu-id="7b917-189">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="7b917-190">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="7b917-190">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="7b917-191">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7b917-191">eapFastConfiguration</span></span>|[<span data-ttu-id="7b917-192">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7b917-192">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="7b917-193">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="7b917-193">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="7b917-194">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="7b917-194">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="7b917-195">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="7b917-195">trustedServerCertificateNames</span></span>|<span data-ttu-id="7b917-196">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b917-196">String collection</span></span>|<span data-ttu-id="7b917-197">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="7b917-197">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="7b917-198">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="7b917-198">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="7b917-199">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой проводной сети.</span><span class="sxs-lookup"><span data-stu-id="7b917-199">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="7b917-200">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="7b917-200">authenticationMethod</span></span>|[<span data-ttu-id="7b917-201">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="7b917-201">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="7b917-202">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="7b917-202">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="7b917-203">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7b917-203">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7b917-204">Свойства noneapauthenticationmethodforeapttls</span><span class="sxs-lookup"><span data-stu-id="7b917-204">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="7b917-205">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="7b917-205">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="7b917-206">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="7b917-206">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="7b917-207">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="7b917-207">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="7b917-208">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="7b917-208">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="7b917-209">Строка</span><span class="sxs-lookup"><span data-stu-id="7b917-209">String</span></span>|<span data-ttu-id="7b917-210">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="7b917-210">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="7b917-211">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="7b917-211">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="7b917-212">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этой проводной сети, используют их реальное имя, отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="7b917-212">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="7b917-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b917-213">Response</span></span>
<span data-ttu-id="7b917-214">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b917-214">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b917-215">Пример</span><span class="sxs-lookup"><span data-stu-id="7b917-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b917-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b917-216">Request</span></span>
<span data-ttu-id="7b917-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b917-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
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
  "networkName": "Network Name value",
  "networkInterface": "firstActiveEthernet",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
}
```

### <a name="response"></a><span data-ttu-id="7b917-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b917-218">Response</span></span>
<span data-ttu-id="7b917-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b917-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
  "id": "e5a57519-7519-e5a5-1975-a5e51975a5e5",
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
  "networkName": "Network Name value",
  "networkInterface": "firstActiveEthernet",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
}
```





