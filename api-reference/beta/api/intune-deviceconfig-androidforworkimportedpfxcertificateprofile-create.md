---
title: Создание androidForWorkImportedPFXCertificateProfile
description: Создание нового объекта androidForWorkImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb85e846645b5187e4f6feb8af78e2c624821a70
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414517"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="8ef5a-103">Создание androidForWorkImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8ef5a-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="8ef5a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ef5a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ef5a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ef5a-107">Создание нового объекта [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8ef5a-107">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ef5a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8ef5a-108">Prerequisites</span></span>
<span data-ttu-id="8ef5a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8ef5a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ef5a-111">Permission type</span></span>|<span data-ttu-id="8ef5a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ef5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ef5a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ef5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ef5a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ef5a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ef5a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ef5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ef5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-116">Not supported.</span></span>|
|<span data-ttu-id="8ef5a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ef5a-117">Application</span></span>|<span data-ttu-id="8ef5a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ef5a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ef5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ef5a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ef5a-120">Request headers</span></span>
|<span data-ttu-id="8ef5a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ef5a-121">Header</span></span>|<span data-ttu-id="8ef5a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ef5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ef5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ef5a-123">Authorization</span></span>|<span data-ttu-id="8ef5a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8ef5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ef5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ef5a-125">Accept</span></span>|<span data-ttu-id="8ef5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ef5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ef5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ef5a-127">Request body</span></span>
<span data-ttu-id="8ef5a-128">В тексте запроса укажите представление JSON для объекта androidForWorkImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-128">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="8ef5a-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-129">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="8ef5a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ef5a-130">Property</span></span>|<span data-ttu-id="8ef5a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ef5a-131">Type</span></span>|<span data-ttu-id="8ef5a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ef5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ef5a-133">id</span><span class="sxs-lookup"><span data-stu-id="8ef5a-133">id</span></span>|<span data-ttu-id="8ef5a-134">String</span><span class="sxs-lookup"><span data-stu-id="8ef5a-134">String</span></span>|<span data-ttu-id="8ef5a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-135">Key of the entity.</span></span> <span data-ttu-id="8ef5a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef5a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8ef5a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef5a-138">DateTimeOffset</span></span>|<span data-ttu-id="8ef5a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8ef5a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ef5a-141">roleScopeTagIds</span></span>|<span data-ttu-id="8ef5a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8ef5a-142">String collection</span></span>|<span data-ttu-id="8ef5a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ef5a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ef5a-145">supportsScopeTags</span></span>|<span data-ttu-id="8ef5a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8ef5a-146">Boolean</span></span>|<span data-ttu-id="8ef5a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ef5a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ef5a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ef5a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-150">This property is read-only.</span></span> <span data-ttu-id="8ef5a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef5a-152">createdDateTime</span></span>|<span data-ttu-id="8ef5a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef5a-153">DateTimeOffset</span></span>|<span data-ttu-id="8ef5a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-154">DateTime the object was created.</span></span> <span data-ttu-id="8ef5a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-156">description</span><span class="sxs-lookup"><span data-stu-id="8ef5a-156">description</span></span>|<span data-ttu-id="8ef5a-157">String</span><span class="sxs-lookup"><span data-stu-id="8ef5a-157">String</span></span>|<span data-ttu-id="8ef5a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ef5a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8ef5a-160">displayName</span></span>|<span data-ttu-id="8ef5a-161">String</span><span class="sxs-lookup"><span data-stu-id="8ef5a-161">String</span></span>|<span data-ttu-id="8ef5a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ef5a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-164">version</span><span class="sxs-lookup"><span data-stu-id="8ef5a-164">version</span></span>|<span data-ttu-id="8ef5a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef5a-165">Int32</span></span>|<span data-ttu-id="8ef5a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-166">Version of the device configuration.</span></span> <span data-ttu-id="8ef5a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ef5a-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8ef5a-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="8ef5a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef5a-169">Int32</span></span>|<span data-ttu-id="8ef5a-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8ef5a-171">Допустимые значения от 1 до 99 унаследованные от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8ef5a-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8ef5a-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8ef5a-172">subjectNameFormat</span></span>|[<span data-ttu-id="8ef5a-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8ef5a-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="8ef5a-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="8ef5a-175">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="8ef5a-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="8ef5a-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8ef5a-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8ef5a-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8ef5a-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8ef5a-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="8ef5a-180">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="8ef5a-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8ef5a-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8ef5a-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8ef5a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef5a-183">Int32</span></span>|<span data-ttu-id="8ef5a-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8ef5a-185">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8ef5a-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8ef5a-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8ef5a-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8ef5a-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8ef5a-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8ef5a-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8ef5a-189">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="8ef5a-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8ef5a-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="8ef5a-191">extendedKeyUsages</span></span>|<span data-ttu-id="8ef5a-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8ef5a-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8ef5a-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="8ef5a-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8ef5a-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8ef5a-195">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8ef5a-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8ef5a-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8ef5a-196">intendedPurpose</span></span>|[<span data-ttu-id="8ef5a-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8ef5a-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="8ef5a-198">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-198">Not yet documented.</span></span> <span data-ttu-id="8ef5a-199">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="8ef5a-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ef5a-200">Response</span></span>
<span data-ttu-id="8ef5a-201">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-201">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ef5a-202">Пример</span><span class="sxs-lookup"><span data-stu-id="8ef5a-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ef5a-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ef5a-203">Request</span></span>
<span data-ttu-id="8ef5a-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="8ef5a-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ef5a-205">Response</span></span>
<span data-ttu-id="8ef5a-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8ef5a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




