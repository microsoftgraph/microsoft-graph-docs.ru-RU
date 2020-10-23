---
title: Создание Макосвиреднетворкконфигуратион
description: Создание нового объекта Макосвиреднетворкконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d58a3e27c084a942ac7bcc5f1de62156973ea885
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708377"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="31445-103">Создание Макосвиреднетворкконфигуратион</span><span class="sxs-lookup"><span data-stu-id="31445-103">Create macOSWiredNetworkConfiguration</span></span>

<span data-ttu-id="31445-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31445-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31445-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31445-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31445-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31445-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31445-107">Создание нового объекта [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="31445-107">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31445-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31445-108">Prerequisites</span></span>
<span data-ttu-id="31445-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31445-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31445-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31445-111">Permission type</span></span>|<span data-ttu-id="31445-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31445-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31445-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31445-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31445-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31445-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31445-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31445-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31445-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31445-116">Not supported.</span></span>|
|<span data-ttu-id="31445-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31445-117">Application</span></span>|<span data-ttu-id="31445-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31445-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31445-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31445-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31445-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31445-120">Request headers</span></span>
|<span data-ttu-id="31445-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31445-121">Header</span></span>|<span data-ttu-id="31445-122">Значение</span><span class="sxs-lookup"><span data-stu-id="31445-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31445-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31445-123">Authorization</span></span>|<span data-ttu-id="31445-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31445-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31445-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31445-125">Accept</span></span>|<span data-ttu-id="31445-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31445-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31445-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31445-127">Request body</span></span>
<span data-ttu-id="31445-128">В тексте запроса добавьте представление объекта Макосвиреднетворкконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31445-128">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="31445-129">В следующей таблице приведены свойства, необходимые при создании Макосвиреднетворкконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="31445-129">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="31445-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="31445-130">Property</span></span>|<span data-ttu-id="31445-131">Тип</span><span class="sxs-lookup"><span data-stu-id="31445-131">Type</span></span>|<span data-ttu-id="31445-132">Описание</span><span class="sxs-lookup"><span data-stu-id="31445-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31445-133">id</span><span class="sxs-lookup"><span data-stu-id="31445-133">id</span></span>|<span data-ttu-id="31445-134">Строка</span><span class="sxs-lookup"><span data-stu-id="31445-134">String</span></span>|<span data-ttu-id="31445-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31445-135">Key of the entity.</span></span> <span data-ttu-id="31445-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31445-137">lastModifiedDateTime</span></span>|<span data-ttu-id="31445-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31445-138">DateTimeOffset</span></span>|<span data-ttu-id="31445-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="31445-139">DateTime the object was last modified.</span></span> <span data-ttu-id="31445-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31445-141">roleScopeTagIds</span></span>|<span data-ttu-id="31445-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="31445-142">String collection</span></span>|<span data-ttu-id="31445-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="31445-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31445-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="31445-145">supportsScopeTags</span></span>|<span data-ttu-id="31445-146">Логический</span><span class="sxs-lookup"><span data-stu-id="31445-146">Boolean</span></span>|<span data-ttu-id="31445-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="31445-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31445-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="31445-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31445-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="31445-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31445-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31445-150">This property is read-only.</span></span> <span data-ttu-id="31445-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31445-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="31445-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31445-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="31445-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="31445-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="31445-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="31445-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="31445-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="31445-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="31445-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="31445-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="31445-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="31445-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="31445-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="31445-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="31445-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="31445-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="31445-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31445-164">createdDateTime</span></span>|<span data-ttu-id="31445-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31445-165">DateTimeOffset</span></span>|<span data-ttu-id="31445-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="31445-166">DateTime the object was created.</span></span> <span data-ttu-id="31445-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-168">description</span><span class="sxs-lookup"><span data-stu-id="31445-168">description</span></span>|<span data-ttu-id="31445-169">Строка</span><span class="sxs-lookup"><span data-stu-id="31445-169">String</span></span>|<span data-ttu-id="31445-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31445-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31445-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-172">displayName</span><span class="sxs-lookup"><span data-stu-id="31445-172">displayName</span></span>|<span data-ttu-id="31445-173">Строка</span><span class="sxs-lookup"><span data-stu-id="31445-173">String</span></span>|<span data-ttu-id="31445-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31445-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31445-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-176">version</span><span class="sxs-lookup"><span data-stu-id="31445-176">version</span></span>|<span data-ttu-id="31445-177">Int32</span><span class="sxs-lookup"><span data-stu-id="31445-177">Int32</span></span>|<span data-ttu-id="31445-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31445-178">Version of the device configuration.</span></span> <span data-ttu-id="31445-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31445-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31445-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="31445-180">networkName</span></span>|<span data-ttu-id="31445-181">Строка</span><span class="sxs-lookup"><span data-stu-id="31445-181">String</span></span>|<span data-ttu-id="31445-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="31445-182">Network Name</span></span>|
|<span data-ttu-id="31445-183">нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="31445-183">networkInterface</span></span>|[<span data-ttu-id="31445-184">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="31445-184">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="31445-185">Сетевой интерфейс.</span><span class="sxs-lookup"><span data-stu-id="31445-185">Network interface.</span></span> <span data-ttu-id="31445-186">Возможные значения: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="31445-186">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="31445-187">еаптипе</span><span class="sxs-lookup"><span data-stu-id="31445-187">eapType</span></span>|[<span data-ttu-id="31445-188">еаптипе</span><span class="sxs-lookup"><span data-stu-id="31445-188">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="31445-189">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="31445-189">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="31445-190">Указывает тип протокола EAP, установленный для проводной сети.</span><span class="sxs-lookup"><span data-stu-id="31445-190">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="31445-191">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="31445-191">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="31445-192">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="31445-192">eapFastConfiguration</span></span>|[<span data-ttu-id="31445-193">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="31445-193">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="31445-194">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="31445-194">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="31445-195">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="31445-195">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="31445-196">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="31445-196">trustedServerCertificateNames</span></span>|<span data-ttu-id="31445-197">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="31445-197">String collection</span></span>|<span data-ttu-id="31445-198">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="31445-198">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="31445-199">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="31445-199">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="31445-200">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой проводной сети.</span><span class="sxs-lookup"><span data-stu-id="31445-200">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="31445-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="31445-201">authenticationMethod</span></span>|[<span data-ttu-id="31445-202">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="31445-202">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="31445-203">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="31445-203">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="31445-204">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="31445-204">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="31445-205">Свойства noneapauthenticationmethodforeapttls</span><span class="sxs-lookup"><span data-stu-id="31445-205">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="31445-206">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="31445-206">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="31445-207">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="31445-207">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="31445-208">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="31445-208">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="31445-209">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="31445-209">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="31445-210">Строка</span><span class="sxs-lookup"><span data-stu-id="31445-210">String</span></span>|<span data-ttu-id="31445-211">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="31445-211">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="31445-212">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="31445-212">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="31445-213">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этой проводной сети, используют их реальное имя, отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="31445-213">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="31445-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="31445-214">Response</span></span>
<span data-ttu-id="31445-215">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31445-215">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31445-216">Пример</span><span class="sxs-lookup"><span data-stu-id="31445-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="31445-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="31445-217">Request</span></span>
<span data-ttu-id="31445-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31445-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31445-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="31445-219">Response</span></span>
<span data-ttu-id="31445-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31445-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





