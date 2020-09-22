---
title: Создание Макосвиреднетворкконфигуратион
description: Создание нового объекта Макосвиреднетворкконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4f2943f07362e7bb3a72baf8cd50aee6e6e5da2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017754"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="bdcba-103">Создание Макосвиреднетворкконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bdcba-103">Create macOSWiredNetworkConfiguration</span></span>

<span data-ttu-id="bdcba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdcba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdcba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdcba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdcba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdcba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdcba-107">Создание нового объекта [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bdcba-107">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdcba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bdcba-108">Prerequisites</span></span>
<span data-ttu-id="bdcba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdcba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdcba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdcba-111">Permission type</span></span>|<span data-ttu-id="bdcba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdcba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdcba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdcba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdcba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdcba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdcba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdcba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdcba-116">Not supported.</span></span>|
|<span data-ttu-id="bdcba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdcba-117">Application</span></span>|<span data-ttu-id="bdcba-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcba-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdcba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdcba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bdcba-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bdcba-120">Request headers</span></span>
|<span data-ttu-id="bdcba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdcba-121">Header</span></span>|<span data-ttu-id="bdcba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdcba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdcba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdcba-123">Authorization</span></span>|<span data-ttu-id="bdcba-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdcba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdcba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdcba-125">Accept</span></span>|<span data-ttu-id="bdcba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdcba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdcba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdcba-127">Request body</span></span>
<span data-ttu-id="bdcba-128">В тексте запроса добавьте представление объекта Макосвиреднетворкконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdcba-128">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="bdcba-129">В следующей таблице приведены свойства, необходимые при создании Макосвиреднетворкконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="bdcba-129">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="bdcba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdcba-130">Property</span></span>|<span data-ttu-id="bdcba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bdcba-131">Type</span></span>|<span data-ttu-id="bdcba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bdcba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdcba-133">id</span><span class="sxs-lookup"><span data-stu-id="bdcba-133">id</span></span>|<span data-ttu-id="bdcba-134">String</span><span class="sxs-lookup"><span data-stu-id="bdcba-134">String</span></span>|<span data-ttu-id="bdcba-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bdcba-135">Key of the entity.</span></span> <span data-ttu-id="bdcba-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdcba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bdcba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdcba-138">DateTimeOffset</span></span>|<span data-ttu-id="bdcba-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bdcba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bdcba-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bdcba-141">roleScopeTagIds</span></span>|<span data-ttu-id="bdcba-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bdcba-142">String collection</span></span>|<span data-ttu-id="bdcba-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bdcba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bdcba-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bdcba-145">supportsScopeTags</span></span>|<span data-ttu-id="bdcba-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdcba-146">Boolean</span></span>|<span data-ttu-id="bdcba-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bdcba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bdcba-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bdcba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bdcba-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bdcba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bdcba-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdcba-150">This property is read-only.</span></span> <span data-ttu-id="bdcba-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bdcba-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bdcba-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bdcba-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bdcba-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bdcba-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bdcba-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bdcba-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bdcba-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bdcba-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bdcba-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bdcba-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bdcba-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bdcba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bdcba-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bdcba-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bdcba-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bdcba-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bdcba-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdcba-164">createdDateTime</span></span>|<span data-ttu-id="bdcba-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdcba-165">DateTimeOffset</span></span>|<span data-ttu-id="bdcba-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bdcba-166">DateTime the object was created.</span></span> <span data-ttu-id="bdcba-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-168">description</span><span class="sxs-lookup"><span data-stu-id="bdcba-168">description</span></span>|<span data-ttu-id="bdcba-169">String</span><span class="sxs-lookup"><span data-stu-id="bdcba-169">String</span></span>|<span data-ttu-id="bdcba-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdcba-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bdcba-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bdcba-172">displayName</span></span>|<span data-ttu-id="bdcba-173">String</span><span class="sxs-lookup"><span data-stu-id="bdcba-173">String</span></span>|<span data-ttu-id="bdcba-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdcba-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bdcba-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-176">version</span><span class="sxs-lookup"><span data-stu-id="bdcba-176">version</span></span>|<span data-ttu-id="bdcba-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bdcba-177">Int32</span></span>|<span data-ttu-id="bdcba-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdcba-178">Version of the device configuration.</span></span> <span data-ttu-id="bdcba-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdcba-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdcba-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="bdcba-180">networkName</span></span>|<span data-ttu-id="bdcba-181">String</span><span class="sxs-lookup"><span data-stu-id="bdcba-181">String</span></span>|<span data-ttu-id="bdcba-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="bdcba-182">Network Name</span></span>|
|<span data-ttu-id="bdcba-183">нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="bdcba-183">networkInterface</span></span>|[<span data-ttu-id="bdcba-184">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="bdcba-184">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="bdcba-185">Сетевой интерфейс.</span><span class="sxs-lookup"><span data-stu-id="bdcba-185">Network interface.</span></span> <span data-ttu-id="bdcba-186">Возможные значения: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span><span class="sxs-lookup"><span data-stu-id="bdcba-186">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="bdcba-187">еаптипе</span><span class="sxs-lookup"><span data-stu-id="bdcba-187">eapType</span></span>|[<span data-ttu-id="bdcba-188">еаптипе</span><span class="sxs-lookup"><span data-stu-id="bdcba-188">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="bdcba-189">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="bdcba-189">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="bdcba-190">Указывает тип протокола EAP, установленный для проводной сети.</span><span class="sxs-lookup"><span data-stu-id="bdcba-190">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="bdcba-191">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="bdcba-191">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="bdcba-192">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bdcba-192">eapFastConfiguration</span></span>|[<span data-ttu-id="bdcba-193">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bdcba-193">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="bdcba-194">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="bdcba-194">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="bdcba-195">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="bdcba-195">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="bdcba-196">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="bdcba-196">trustedServerCertificateNames</span></span>|<span data-ttu-id="bdcba-197">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bdcba-197">String collection</span></span>|<span data-ttu-id="bdcba-198">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="bdcba-198">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="bdcba-199">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="bdcba-199">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="bdcba-200">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой проводной сети.</span><span class="sxs-lookup"><span data-stu-id="bdcba-200">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="bdcba-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="bdcba-201">authenticationMethod</span></span>|[<span data-ttu-id="bdcba-202">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="bdcba-202">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="bdcba-203">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="bdcba-203">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="bdcba-204">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="bdcba-204">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="bdcba-205">Свойства noneapauthenticationmethodforeapttls</span><span class="sxs-lookup"><span data-stu-id="bdcba-205">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="bdcba-206">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="bdcba-206">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="bdcba-207">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="bdcba-207">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="bdcba-208">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="bdcba-208">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="bdcba-209">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="bdcba-209">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="bdcba-210">String</span><span class="sxs-lookup"><span data-stu-id="bdcba-210">String</span></span>|<span data-ttu-id="bdcba-211">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="bdcba-211">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="bdcba-212">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="bdcba-212">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="bdcba-213">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этой проводной сети, используют их реальное имя, отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="bdcba-213">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="bdcba-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdcba-214">Response</span></span>
<span data-ttu-id="bdcba-215">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвиреднетворкконфигуратион](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdcba-215">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdcba-216">Пример</span><span class="sxs-lookup"><span data-stu-id="bdcba-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdcba-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdcba-217">Request</span></span>
<span data-ttu-id="bdcba-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdcba-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bdcba-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdcba-219">Response</span></span>
<span data-ttu-id="bdcba-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdcba-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






