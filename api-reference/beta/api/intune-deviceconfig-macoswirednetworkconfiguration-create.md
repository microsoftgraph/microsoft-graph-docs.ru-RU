---
title: Создание macOSWiredNetworkConfiguration
description: Создайте новый объект macOSWiredNetworkConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91003cdb7b48da0271dcf83651628b4a3b5dde47
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131206"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="376e5-103">Создание macOSWiredNetworkConfiguration</span><span class="sxs-lookup"><span data-stu-id="376e5-103">Create macOSWiredNetworkConfiguration</span></span>

<span data-ttu-id="376e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="376e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="376e5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="376e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="376e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="376e5-107">Создайте [новый объект macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="376e5-107">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="376e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="376e5-108">Prerequisites</span></span>
<span data-ttu-id="376e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="376e5-111">Permission type</span></span>|<span data-ttu-id="376e5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="376e5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376e5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="376e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="376e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="376e5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="376e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376e5-116">Not supported.</span></span>|
|<span data-ttu-id="376e5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="376e5-117">Application</span></span>|<span data-ttu-id="376e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="376e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="376e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="376e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="376e5-120">Request headers</span></span>
|<span data-ttu-id="376e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="376e5-121">Header</span></span>|<span data-ttu-id="376e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="376e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="376e5-123">Authorization</span></span>|<span data-ttu-id="376e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="376e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="376e5-125">Accept</span></span>|<span data-ttu-id="376e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="376e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="376e5-127">Request body</span></span>
<span data-ttu-id="376e5-128">В теле запроса предоставляем представление JSON для объекта macOSWiredNetworkConfiguration.</span><span class="sxs-lookup"><span data-stu-id="376e5-128">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="376e5-129">В следующей таблице показаны свойства, необходимые при создании macOSWiredNetworkConfiguration.</span><span class="sxs-lookup"><span data-stu-id="376e5-129">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="376e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="376e5-130">Property</span></span>|<span data-ttu-id="376e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="376e5-131">Type</span></span>|<span data-ttu-id="376e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="376e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376e5-133">id</span><span class="sxs-lookup"><span data-stu-id="376e5-133">id</span></span>|<span data-ttu-id="376e5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="376e5-134">String</span></span>|<span data-ttu-id="376e5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="376e5-135">Key of the entity.</span></span> <span data-ttu-id="376e5-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="376e5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="376e5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376e5-138">DateTimeOffset</span></span>|<span data-ttu-id="376e5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="376e5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="376e5-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="376e5-141">roleScopeTagIds</span></span>|<span data-ttu-id="376e5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="376e5-142">String collection</span></span>|<span data-ttu-id="376e5-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="376e5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="376e5-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="376e5-145">supportsScopeTags</span></span>|<span data-ttu-id="376e5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="376e5-146">Boolean</span></span>|<span data-ttu-id="376e5-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="376e5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="376e5-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="376e5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="376e5-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="376e5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="376e5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="376e5-150">This property is read-only.</span></span> <span data-ttu-id="376e5-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="376e5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="376e5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="376e5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="376e5-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="376e5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="376e5-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="376e5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="376e5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="376e5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="376e5-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="376e5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="376e5-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="376e5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="376e5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="376e5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="376e5-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="376e5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="376e5-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="376e5-164">createdDateTime</span></span>|<span data-ttu-id="376e5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376e5-165">DateTimeOffset</span></span>|<span data-ttu-id="376e5-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="376e5-166">DateTime the object was created.</span></span> <span data-ttu-id="376e5-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-168">description</span><span class="sxs-lookup"><span data-stu-id="376e5-168">description</span></span>|<span data-ttu-id="376e5-169">Строка</span><span class="sxs-lookup"><span data-stu-id="376e5-169">String</span></span>|<span data-ttu-id="376e5-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="376e5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="376e5-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="376e5-172">displayName</span></span>|<span data-ttu-id="376e5-173">Строка</span><span class="sxs-lookup"><span data-stu-id="376e5-173">String</span></span>|<span data-ttu-id="376e5-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="376e5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="376e5-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-176">version</span><span class="sxs-lookup"><span data-stu-id="376e5-176">version</span></span>|<span data-ttu-id="376e5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="376e5-177">Int32</span></span>|<span data-ttu-id="376e5-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="376e5-178">Version of the device configuration.</span></span> <span data-ttu-id="376e5-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="376e5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376e5-180">networkName</span><span class="sxs-lookup"><span data-stu-id="376e5-180">networkName</span></span>|<span data-ttu-id="376e5-181">Строка</span><span class="sxs-lookup"><span data-stu-id="376e5-181">String</span></span>|<span data-ttu-id="376e5-182">Имя сети</span><span class="sxs-lookup"><span data-stu-id="376e5-182">Network Name</span></span>|
|<span data-ttu-id="376e5-183">networkInterface</span><span class="sxs-lookup"><span data-stu-id="376e5-183">networkInterface</span></span>|[<span data-ttu-id="376e5-184">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="376e5-184">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="376e5-185">Сетевой интерфейс.</span><span class="sxs-lookup"><span data-stu-id="376e5-185">Network interface.</span></span> <span data-ttu-id="376e5-186">Возможные значения: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="376e5-186">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="376e5-187">eapType</span><span class="sxs-lookup"><span data-stu-id="376e5-187">eapType</span></span>|[<span data-ttu-id="376e5-188">eapType</span><span class="sxs-lookup"><span data-stu-id="376e5-188">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="376e5-189">Extensible Authentication Protocol (EAP).</span><span class="sxs-lookup"><span data-stu-id="376e5-189">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="376e5-190">Указывает тип протокола EAP, задаваемого в проводной сети.</span><span class="sxs-lookup"><span data-stu-id="376e5-190">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="376e5-191">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="376e5-191">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="376e5-192">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="376e5-192">eapFastConfiguration</span></span>|[<span data-ttu-id="376e5-193">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="376e5-193">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="376e5-194">Параметр конфигурации EAP-FAST, когда EAP-FAST является выбранным типом EAP.</span><span class="sxs-lookup"><span data-stu-id="376e5-194">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="376e5-195">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="376e5-195">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="376e5-196">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="376e5-196">trustedServerCertificateNames</span></span>|<span data-ttu-id="376e5-197">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="376e5-197">String collection</span></span>|<span data-ttu-id="376e5-198">Доверенные имена сертификатов сервера при настройке типа EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="376e5-198">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="376e5-199">Это общее имя, используемая в сертификатах, выдаванных доверенным органом сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="376e5-199">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="376e5-200">Если вы предоставите эту информацию, можно обойти динамический диалог доверия, отображаемый на устройствах конечных пользователей при подключении к этой проводной сети.</span><span class="sxs-lookup"><span data-stu-id="376e5-200">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="376e5-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="376e5-201">authenticationMethod</span></span>|[<span data-ttu-id="376e5-202">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="376e5-202">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="376e5-203">Метод проверки подлинности при настройке типа EAP на PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="376e5-203">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="376e5-204">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="376e5-204">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="376e5-205">nonEapAuthenticationMethodForEapTtls</span><span class="sxs-lookup"><span data-stu-id="376e5-205">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="376e5-206">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="376e5-206">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="376e5-207">Метод без EAP для проверки подлинности (внутренняя идентичность), когда тип EAP EAP-TTLS и authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="376e5-207">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="376e5-208">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="376e5-208">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="376e5-209">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="376e5-209">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="376e5-210">Строка</span><span class="sxs-lookup"><span data-stu-id="376e5-210">String</span></span>|<span data-ttu-id="376e5-211">Введите конфиденциальность удостоверений (внешний идентификатор), если тип EAP настроен на EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="376e5-211">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="376e5-212">Это свойство маскирует имена пользователей с вводимым текстом.</span><span class="sxs-lookup"><span data-stu-id="376e5-212">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="376e5-213">Например, если вы используете "анонимный", каждый пользователь, который аутентификация с помощью этой проводной сети с помощью их реального имени пользователя отображается как "анонимный".</span><span class="sxs-lookup"><span data-stu-id="376e5-213">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="376e5-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="376e5-214">Response</span></span>
<span data-ttu-id="376e5-215">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="376e5-215">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376e5-216">Пример</span><span class="sxs-lookup"><span data-stu-id="376e5-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="376e5-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="376e5-217">Request</span></span>
<span data-ttu-id="376e5-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="376e5-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="376e5-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="376e5-219">Response</span></span>
<span data-ttu-id="376e5-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="376e5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




