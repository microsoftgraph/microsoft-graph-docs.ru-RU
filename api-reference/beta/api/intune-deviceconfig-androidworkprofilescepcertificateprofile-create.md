---
title: Создание Андроидворкпрофилесцепцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилесцепцертификатепрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df81fe793fcbcbd6cb269010651ee7618168fd42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140119"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="bd12b-103">Создание Андроидворкпрофилесцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="bd12b-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="bd12b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd12b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd12b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd12b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd12b-106">Создание нового объекта [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bd12b-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd12b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd12b-107">Prerequisites</span></span>
<span data-ttu-id="bd12b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd12b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd12b-110">Permission type</span></span>|<span data-ttu-id="bd12b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd12b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd12b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd12b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd12b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd12b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd12b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd12b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd12b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd12b-115">Not supported.</span></span>|
|<span data-ttu-id="bd12b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd12b-116">Application</span></span>|<span data-ttu-id="bd12b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd12b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd12b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd12b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd12b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd12b-119">Request headers</span></span>
|<span data-ttu-id="bd12b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd12b-120">Header</span></span>|<span data-ttu-id="bd12b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bd12b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd12b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd12b-122">Authorization</span></span>|<span data-ttu-id="bd12b-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bd12b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd12b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bd12b-124">Accept</span></span>|<span data-ttu-id="bd12b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd12b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd12b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd12b-126">Request body</span></span>
<span data-ttu-id="bd12b-127">В тексте запроса добавьте представление объекта Андроидворкпрофилесцепцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd12b-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="bd12b-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилесцепцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="bd12b-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="bd12b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd12b-129">Property</span></span>|<span data-ttu-id="bd12b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bd12b-130">Type</span></span>|<span data-ttu-id="bd12b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bd12b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd12b-132">id</span><span class="sxs-lookup"><span data-stu-id="bd12b-132">id</span></span>|<span data-ttu-id="bd12b-133">String</span><span class="sxs-lookup"><span data-stu-id="bd12b-133">String</span></span>|<span data-ttu-id="bd12b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd12b-134">Key of the entity.</span></span> <span data-ttu-id="bd12b-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd12b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bd12b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd12b-137">DateTimeOffset</span></span>|<span data-ttu-id="bd12b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bd12b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bd12b-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd12b-140">roleScopeTagIds</span></span>|<span data-ttu-id="bd12b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd12b-141">String collection</span></span>|<span data-ttu-id="bd12b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bd12b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd12b-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bd12b-144">supportsScopeTags</span></span>|<span data-ttu-id="bd12b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="bd12b-145">Boolean</span></span>|<span data-ttu-id="bd12b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bd12b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bd12b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bd12b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bd12b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bd12b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bd12b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd12b-149">This property is read-only.</span></span> <span data-ttu-id="bd12b-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd12b-151">createdDateTime</span></span>|<span data-ttu-id="bd12b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd12b-152">DateTimeOffset</span></span>|<span data-ttu-id="bd12b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bd12b-153">DateTime the object was created.</span></span> <span data-ttu-id="bd12b-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-155">description</span><span class="sxs-lookup"><span data-stu-id="bd12b-155">description</span></span>|<span data-ttu-id="bd12b-156">String</span><span class="sxs-lookup"><span data-stu-id="bd12b-156">String</span></span>|<span data-ttu-id="bd12b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd12b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd12b-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bd12b-159">displayName</span></span>|<span data-ttu-id="bd12b-160">String</span><span class="sxs-lookup"><span data-stu-id="bd12b-160">String</span></span>|<span data-ttu-id="bd12b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd12b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd12b-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-163">version</span><span class="sxs-lookup"><span data-stu-id="bd12b-163">version</span></span>|<span data-ttu-id="bd12b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bd12b-164">Int32</span></span>|<span data-ttu-id="bd12b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd12b-165">Version of the device configuration.</span></span> <span data-ttu-id="bd12b-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd12b-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="bd12b-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="bd12b-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bd12b-168">Int32</span></span>|<span data-ttu-id="bd12b-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd12b-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bd12b-170">Допустимые значения — от 1 до 99, наСледуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd12b-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bd12b-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bd12b-171">subjectNameFormat</span></span>|[<span data-ttu-id="bd12b-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bd12b-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="bd12b-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd12b-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="bd12b-174">НаСледуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="bd12b-175">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="bd12b-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bd12b-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bd12b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bd12b-177">Int32</span></span>|<span data-ttu-id="bd12b-178">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd12b-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="bd12b-179">НаСледуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd12b-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bd12b-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bd12b-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bd12b-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bd12b-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bd12b-182">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd12b-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="bd12b-183">НаСледуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bd12b-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="bd12b-184">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bd12b-185">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="bd12b-185">extendedKeyUsages</span></span>|<span data-ttu-id="bd12b-186">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="bd12b-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bd12b-187">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="bd12b-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bd12b-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bd12b-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bd12b-189">НаСледуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd12b-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bd12b-190">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="bd12b-190">scepServerUrls</span></span>|<span data-ttu-id="bd12b-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd12b-191">String collection</span></span>|<span data-ttu-id="bd12b-192">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="bd12b-192">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="bd12b-193">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="bd12b-193">subjectNameFormatString</span></span>|<span data-ttu-id="bd12b-194">String</span><span class="sxs-lookup"><span data-stu-id="bd12b-194">String</span></span>|<span data-ttu-id="bd12b-195">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="bd12b-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="bd12b-196">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="bd12b-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="bd12b-197">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="bd12b-197">keyUsage</span></span>|[<span data-ttu-id="bd12b-198">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="bd12b-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="bd12b-199">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="bd12b-199">SCEP Key Usage.</span></span> <span data-ttu-id="bd12b-200">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="bd12b-201">keySize</span><span class="sxs-lookup"><span data-stu-id="bd12b-201">keySize</span></span>|[<span data-ttu-id="bd12b-202">keySize</span><span class="sxs-lookup"><span data-stu-id="bd12b-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="bd12b-203">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="bd12b-203">SCEP Key Size.</span></span> <span data-ttu-id="bd12b-204">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="bd12b-205">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="bd12b-205">hashAlgorithm</span></span>|[<span data-ttu-id="bd12b-206">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="bd12b-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="bd12b-207">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="bd12b-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="bd12b-208">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="bd12b-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bd12b-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bd12b-210">String</span><span class="sxs-lookup"><span data-stu-id="bd12b-210">String</span></span>|<span data-ttu-id="bd12b-211">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="bd12b-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="bd12b-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bd12b-212">certificateStore</span></span>|[<span data-ttu-id="bd12b-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bd12b-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="bd12b-214">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="bd12b-214">Target store certificate.</span></span> <span data-ttu-id="bd12b-215">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="bd12b-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="bd12b-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="bd12b-217">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="bd12b-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="bd12b-218">Настраиваемые параметры имени субъекта Алтерантиве.</span><span class="sxs-lookup"><span data-stu-id="bd12b-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="bd12b-219">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bd12b-219">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bd12b-220">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bd12b-220">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bd12b-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bd12b-221">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bd12b-222">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd12b-222">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="bd12b-223">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="bd12b-223">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="bd12b-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd12b-224">Response</span></span>
<span data-ttu-id="bd12b-225">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd12b-225">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd12b-226">Пример</span><span class="sxs-lookup"><span data-stu-id="bd12b-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd12b-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd12b-227">Request</span></span>
<span data-ttu-id="bd12b-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd12b-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="bd12b-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd12b-229">Response</span></span>
<span data-ttu-id="bd12b-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd12b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```




