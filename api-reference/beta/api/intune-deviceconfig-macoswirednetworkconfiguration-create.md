---
title: Создание Макосвиреднетворкконфигуратион
description: Создание нового объекта Макосвиреднетворкконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cbbcb83492a6d3894530179728b010891bb2d28
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083552"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="4f392-103">Создание Макосвиреднетворкконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4f392-103">Create macOSWiredNetworkConfiguration</span></span>

> <span data-ttu-id="4f392-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f392-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f392-106">Создание нового объекта [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4f392-106">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f392-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f392-107">Prerequisites</span></span>
<span data-ttu-id="4f392-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f392-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f392-110">Permission type</span></span>|<span data-ttu-id="4f392-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f392-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f392-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f392-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f392-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f392-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f392-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f392-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f392-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f392-115">Not supported.</span></span>|
|<span data-ttu-id="4f392-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f392-116">Application</span></span>|<span data-ttu-id="4f392-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f392-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f392-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f392-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f392-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f392-119">Request headers</span></span>
|<span data-ttu-id="4f392-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f392-120">Header</span></span>|<span data-ttu-id="4f392-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f392-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f392-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f392-122">Authorization</span></span>|<span data-ttu-id="4f392-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f392-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f392-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f392-124">Accept</span></span>|<span data-ttu-id="4f392-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f392-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f392-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f392-126">Request body</span></span>
<span data-ttu-id="4f392-127">В тексте запроса добавьте представление объекта Макосвиреднетворкконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f392-127">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="4f392-128">В следующей таблице приведены свойства, необходимые при создании Макосвиреднетворкконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4f392-128">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="4f392-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f392-129">Property</span></span>|<span data-ttu-id="4f392-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4f392-130">Type</span></span>|<span data-ttu-id="4f392-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4f392-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f392-132">id</span><span class="sxs-lookup"><span data-stu-id="4f392-132">id</span></span>|<span data-ttu-id="4f392-133">String</span><span class="sxs-lookup"><span data-stu-id="4f392-133">String</span></span>|<span data-ttu-id="4f392-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f392-134">Key of the entity.</span></span> <span data-ttu-id="4f392-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f392-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4f392-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f392-137">DateTimeOffset</span></span>|<span data-ttu-id="4f392-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4f392-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4f392-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f392-140">roleScopeTagIds</span></span>|<span data-ttu-id="4f392-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f392-141">String collection</span></span>|<span data-ttu-id="4f392-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4f392-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f392-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4f392-144">supportsScopeTags</span></span>|<span data-ttu-id="4f392-145">Логический</span><span class="sxs-lookup"><span data-stu-id="4f392-145">Boolean</span></span>|<span data-ttu-id="4f392-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4f392-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4f392-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4f392-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4f392-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4f392-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4f392-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f392-149">This property is read-only.</span></span> <span data-ttu-id="4f392-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f392-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4f392-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f392-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4f392-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f392-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4f392-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f392-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4f392-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f392-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4f392-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f392-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4f392-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4f392-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4f392-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4f392-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4f392-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f392-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4f392-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f392-163">createdDateTime</span></span>|<span data-ttu-id="4f392-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f392-164">DateTimeOffset</span></span>|<span data-ttu-id="4f392-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4f392-165">DateTime the object was created.</span></span> <span data-ttu-id="4f392-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-167">description</span><span class="sxs-lookup"><span data-stu-id="4f392-167">description</span></span>|<span data-ttu-id="4f392-168">String</span><span class="sxs-lookup"><span data-stu-id="4f392-168">String</span></span>|<span data-ttu-id="4f392-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f392-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f392-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4f392-171">displayName</span></span>|<span data-ttu-id="4f392-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4f392-172">String</span></span>|<span data-ttu-id="4f392-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f392-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f392-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-175">version</span><span class="sxs-lookup"><span data-stu-id="4f392-175">version</span></span>|<span data-ttu-id="4f392-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4f392-176">Int32</span></span>|<span data-ttu-id="4f392-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f392-177">Version of the device configuration.</span></span> <span data-ttu-id="4f392-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f392-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f392-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="4f392-179">networkName</span></span>|<span data-ttu-id="4f392-180">String</span><span class="sxs-lookup"><span data-stu-id="4f392-180">String</span></span>|<span data-ttu-id="4f392-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="4f392-181">Network Name</span></span>|
|<span data-ttu-id="4f392-182">нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="4f392-182">networkInterface</span></span>|[<span data-ttu-id="4f392-183">виреднетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="4f392-183">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="4f392-184">Сетевой интерфейс.</span><span class="sxs-lookup"><span data-stu-id="4f392-184">Network interface.</span></span> <span data-ttu-id="4f392-185">Возможные значения: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="4f392-185">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="4f392-186">еаптипе</span><span class="sxs-lookup"><span data-stu-id="4f392-186">eapType</span></span>|[<span data-ttu-id="4f392-187">еаптипе</span><span class="sxs-lookup"><span data-stu-id="4f392-187">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="4f392-188">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="4f392-188">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="4f392-189">Указывает тип протокола EAP, установленный для проводной сети.</span><span class="sxs-lookup"><span data-stu-id="4f392-189">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="4f392-190">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="4f392-190">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="4f392-191">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4f392-191">eapFastConfiguration</span></span>|[<span data-ttu-id="4f392-192">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4f392-192">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="4f392-193">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="4f392-193">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="4f392-194">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="4f392-194">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="4f392-195">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="4f392-195">trustedServerCertificateNames</span></span>|<span data-ttu-id="4f392-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f392-196">String collection</span></span>|<span data-ttu-id="4f392-197">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="4f392-197">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="4f392-198">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="4f392-198">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="4f392-199">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой проводной сети.</span><span class="sxs-lookup"><span data-stu-id="4f392-199">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="4f392-200">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="4f392-200">authenticationMethod</span></span>|[<span data-ttu-id="4f392-201">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="4f392-201">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="4f392-202">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="4f392-202">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="4f392-203">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4f392-203">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4f392-204">Свойства noneapauthenticationmethodforeapttls</span><span class="sxs-lookup"><span data-stu-id="4f392-204">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="4f392-205">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="4f392-205">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="4f392-206">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="4f392-206">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="4f392-207">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="4f392-207">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="4f392-208">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="4f392-208">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="4f392-209">String</span><span class="sxs-lookup"><span data-stu-id="4f392-209">String</span></span>|<span data-ttu-id="4f392-210">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="4f392-210">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="4f392-211">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="4f392-211">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="4f392-212">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этой проводной сети, используют их реальное имя, отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="4f392-212">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="4f392-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f392-213">Response</span></span>
<span data-ttu-id="4f392-214">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f392-214">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f392-215">Пример</span><span class="sxs-lookup"><span data-stu-id="4f392-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f392-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f392-216">Request</span></span>
<span data-ttu-id="4f392-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f392-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f392-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f392-218">Response</span></span>
<span data-ttu-id="4f392-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f392-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






