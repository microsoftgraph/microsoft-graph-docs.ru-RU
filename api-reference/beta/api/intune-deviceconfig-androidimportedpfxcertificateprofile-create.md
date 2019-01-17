---
title: Создание androidImportedPFXCertificateProfile
description: Создание нового объекта androidImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d988490fb6dc2ab06a9b94b372b32642bb2e87b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963607"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="1cee8-103">Создание androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="1cee8-103">Create androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="1cee8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cee8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cee8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cee8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cee8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1cee8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cee8-107">Создание нового объекта [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1cee8-107">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cee8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="1cee8-108">Prerequisites</span></span>
<span data-ttu-id="1cee8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cee8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cee8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cee8-111">Permission type</span></span>|<span data-ttu-id="1cee8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cee8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cee8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cee8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cee8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cee8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cee8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cee8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cee8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cee8-116">Not supported.</span></span>|
|<span data-ttu-id="1cee8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cee8-117">Application</span></span>|<span data-ttu-id="1cee8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cee8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cee8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cee8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1cee8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cee8-120">Request headers</span></span>
|<span data-ttu-id="1cee8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cee8-121">Header</span></span>|<span data-ttu-id="1cee8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cee8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cee8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cee8-123">Authorization</span></span>|<span data-ttu-id="1cee8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1cee8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cee8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cee8-125">Accept</span></span>|<span data-ttu-id="1cee8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cee8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cee8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cee8-127">Request body</span></span>
<span data-ttu-id="1cee8-128">В тексте запроса укажите представление JSON для объекта androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1cee8-128">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="1cee8-129">В следующей таблице показаны свойства, которые необходимы для создания androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1cee8-129">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="1cee8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cee8-130">Property</span></span>|<span data-ttu-id="1cee8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cee8-131">Type</span></span>|<span data-ttu-id="1cee8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cee8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cee8-133">id</span><span class="sxs-lookup"><span data-stu-id="1cee8-133">id</span></span>|<span data-ttu-id="1cee8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1cee8-134">String</span></span>|<span data-ttu-id="1cee8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1cee8-135">Key of the entity.</span></span> <span data-ttu-id="1cee8-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cee8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1cee8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cee8-138">DateTimeOffset</span></span>|<span data-ttu-id="1cee8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1cee8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1cee8-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1cee8-141">roleScopeTagIds</span></span>|<span data-ttu-id="1cee8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1cee8-142">String collection</span></span>|<span data-ttu-id="1cee8-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1cee8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1cee8-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1cee8-145">supportsScopeTags</span></span>|<span data-ttu-id="1cee8-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1cee8-146">Boolean</span></span>|<span data-ttu-id="1cee8-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="1cee8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1cee8-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="1cee8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1cee8-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1cee8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1cee8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cee8-150">This property is read-only.</span></span> <span data-ttu-id="1cee8-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cee8-152">createdDateTime</span></span>|<span data-ttu-id="1cee8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cee8-153">DateTimeOffset</span></span>|<span data-ttu-id="1cee8-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1cee8-154">DateTime the object was created.</span></span> <span data-ttu-id="1cee8-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-156">описание</span><span class="sxs-lookup"><span data-stu-id="1cee8-156">description</span></span>|<span data-ttu-id="1cee8-157">Строка</span><span class="sxs-lookup"><span data-stu-id="1cee8-157">String</span></span>|<span data-ttu-id="1cee8-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cee8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1cee8-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1cee8-160">displayName</span></span>|<span data-ttu-id="1cee8-161">Строка</span><span class="sxs-lookup"><span data-stu-id="1cee8-161">String</span></span>|<span data-ttu-id="1cee8-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cee8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1cee8-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-164">version</span><span class="sxs-lookup"><span data-stu-id="1cee8-164">version</span></span>|<span data-ttu-id="1cee8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1cee8-165">Int32</span></span>|<span data-ttu-id="1cee8-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cee8-166">Version of the device configuration.</span></span> <span data-ttu-id="1cee8-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cee8-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1cee8-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="1cee8-169">Int32</span><span class="sxs-lookup"><span data-stu-id="1cee8-169">Int32</span></span>|<span data-ttu-id="1cee8-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cee8-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1cee8-171">Допустимые значения от 1 до 99 унаследованные от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1cee8-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1cee8-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1cee8-172">subjectNameFormat</span></span>|[<span data-ttu-id="1cee8-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1cee8-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1cee8-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cee8-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="1cee8-175">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1cee8-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="1cee8-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1cee8-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1cee8-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1cee8-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1cee8-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1cee8-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cee8-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="1cee8-180">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1cee8-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="1cee8-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1cee8-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1cee8-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1cee8-183">Int32</span><span class="sxs-lookup"><span data-stu-id="1cee8-183">Int32</span></span>|<span data-ttu-id="1cee8-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cee8-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="1cee8-185">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1cee8-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1cee8-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1cee8-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1cee8-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1cee8-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1cee8-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cee8-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1cee8-189">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cee8-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1cee8-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="1cee8-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1cee8-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1cee8-191">extendedKeyUsages</span></span>|<span data-ttu-id="1cee8-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1cee8-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="1cee8-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="1cee8-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="1cee8-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1cee8-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1cee8-195">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1cee8-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1cee8-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1cee8-196">intendedPurpose</span></span>|[<span data-ttu-id="1cee8-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1cee8-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="1cee8-198">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="1cee8-198">Not yet documented.</span></span> <span data-ttu-id="1cee8-199">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="1cee8-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="1cee8-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cee8-200">Response</span></span>
<span data-ttu-id="1cee8-201">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1cee8-201">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cee8-202">Пример</span><span class="sxs-lookup"><span data-stu-id="1cee8-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cee8-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cee8-203">Request</span></span>
<span data-ttu-id="1cee8-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cee8-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 783

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="1cee8-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cee8-205">Response</span></span>
<span data-ttu-id="1cee8-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1cee8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 891

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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





