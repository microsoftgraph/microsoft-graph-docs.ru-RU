---
title: Обновление Андроидфорворкимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Андроидфорворкимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26c759049e0a7e2224f0c554a64de8a68a70ec9a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933517"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="b24ee-103">Обновление Андроидфорворкимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="b24ee-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="b24ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b24ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b24ee-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b24ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b24ee-106">Обновление свойств объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b24ee-106">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b24ee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b24ee-107">Prerequisites</span></span>
<span data-ttu-id="b24ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b24ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b24ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b24ee-110">Permission type</span></span>|<span data-ttu-id="b24ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b24ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b24ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b24ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b24ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b24ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b24ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b24ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b24ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b24ee-115">Not supported.</span></span>|
|<span data-ttu-id="b24ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b24ee-116">Application</span></span>|<span data-ttu-id="b24ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b24ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b24ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b24ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b24ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b24ee-119">Request headers</span></span>
|<span data-ttu-id="b24ee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b24ee-120">Header</span></span>|<span data-ttu-id="b24ee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b24ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b24ee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b24ee-122">Authorization</span></span>|<span data-ttu-id="b24ee-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b24ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b24ee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b24ee-124">Accept</span></span>|<span data-ttu-id="b24ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b24ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b24ee-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b24ee-126">Request body</span></span>
<span data-ttu-id="b24ee-127">В тексте запроса добавьте представление объекта [Андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b24ee-127">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="b24ee-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-128">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="b24ee-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b24ee-129">Property</span></span>|<span data-ttu-id="b24ee-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b24ee-130">Type</span></span>|<span data-ttu-id="b24ee-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b24ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b24ee-132">id</span><span class="sxs-lookup"><span data-stu-id="b24ee-132">id</span></span>|<span data-ttu-id="b24ee-133">String</span><span class="sxs-lookup"><span data-stu-id="b24ee-133">String</span></span>|<span data-ttu-id="b24ee-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b24ee-134">Key of the entity.</span></span> <span data-ttu-id="b24ee-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b24ee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b24ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b24ee-137">DateTimeOffset</span></span>|<span data-ttu-id="b24ee-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b24ee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b24ee-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b24ee-140">roleScopeTagIds</span></span>|<span data-ttu-id="b24ee-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b24ee-141">String collection</span></span>|<span data-ttu-id="b24ee-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b24ee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b24ee-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b24ee-144">supportsScopeTags</span></span>|<span data-ttu-id="b24ee-145">Логический</span><span class="sxs-lookup"><span data-stu-id="b24ee-145">Boolean</span></span>|<span data-ttu-id="b24ee-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b24ee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b24ee-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b24ee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b24ee-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b24ee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b24ee-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b24ee-149">This property is read-only.</span></span> <span data-ttu-id="b24ee-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b24ee-151">createdDateTime</span></span>|<span data-ttu-id="b24ee-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b24ee-152">DateTimeOffset</span></span>|<span data-ttu-id="b24ee-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b24ee-153">DateTime the object was created.</span></span> <span data-ttu-id="b24ee-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-155">description</span><span class="sxs-lookup"><span data-stu-id="b24ee-155">description</span></span>|<span data-ttu-id="b24ee-156">String</span><span class="sxs-lookup"><span data-stu-id="b24ee-156">String</span></span>|<span data-ttu-id="b24ee-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b24ee-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b24ee-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b24ee-159">displayName</span></span>|<span data-ttu-id="b24ee-160">Строка</span><span class="sxs-lookup"><span data-stu-id="b24ee-160">String</span></span>|<span data-ttu-id="b24ee-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b24ee-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b24ee-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-163">version</span><span class="sxs-lookup"><span data-stu-id="b24ee-163">version</span></span>|<span data-ttu-id="b24ee-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b24ee-164">Int32</span></span>|<span data-ttu-id="b24ee-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b24ee-165">Version of the device configuration.</span></span> <span data-ttu-id="b24ee-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b24ee-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="b24ee-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="b24ee-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b24ee-168">Int32</span></span>|<span data-ttu-id="b24ee-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="b24ee-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b24ee-170">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b24ee-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b24ee-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b24ee-171">subjectNameFormat</span></span>|[<span data-ttu-id="b24ee-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b24ee-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b24ee-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b24ee-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="b24ee-174">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b24ee-175">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b24ee-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b24ee-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b24ee-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b24ee-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b24ee-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b24ee-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b24ee-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b24ee-179">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b24ee-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b24ee-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b24ee-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b24ee-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b24ee-182">Int32</span><span class="sxs-lookup"><span data-stu-id="b24ee-182">Int32</span></span>|<span data-ttu-id="b24ee-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b24ee-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b24ee-184">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b24ee-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b24ee-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b24ee-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b24ee-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b24ee-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b24ee-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b24ee-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b24ee-188">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b24ee-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="b24ee-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b24ee-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b24ee-190">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="b24ee-190">extendedKeyUsages</span></span>|<span data-ttu-id="b24ee-191">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b24ee-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b24ee-192">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="b24ee-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b24ee-193">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b24ee-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b24ee-194">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b24ee-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b24ee-195">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="b24ee-195">intendedPurpose</span></span>|[<span data-ttu-id="b24ee-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="b24ee-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="b24ee-197">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b24ee-197">Not yet documented.</span></span> <span data-ttu-id="b24ee-198">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="b24ee-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="b24ee-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="b24ee-199">Response</span></span>
<span data-ttu-id="b24ee-200">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b24ee-200">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b24ee-201">Пример</span><span class="sxs-lookup"><span data-stu-id="b24ee-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="b24ee-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="b24ee-202">Request</span></span>
<span data-ttu-id="b24ee-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b24ee-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="b24ee-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="b24ee-204">Response</span></span>
<span data-ttu-id="b24ee-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b24ee-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 898

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "intendedPurpose": "smimeEncryption"
}
```




