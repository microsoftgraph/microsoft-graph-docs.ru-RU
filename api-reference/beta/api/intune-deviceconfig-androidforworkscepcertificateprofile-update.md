---
title: Обновление androidForWorkScepCertificateProfile
description: Обновление свойства объекта androidForWorkScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e034b7c4dde6a6dbbfc1de41a2d5ea25c7d8f49f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946723"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="c5a3f-103">Обновление androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c5a3f-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="c5a3f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5a3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5a3f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5a3f-107">Обновление свойства объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c5a3f-107">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5a3f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5a3f-108">Prerequisites</span></span>
<span data-ttu-id="c5a3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5a3f-111">Permission type</span></span>|<span data-ttu-id="c5a3f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5a3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5a3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a3f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a3f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5a3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-116">Not supported.</span></span>|
|<span data-ttu-id="c5a3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5a3f-117">Application</span></span>|<span data-ttu-id="c5a3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5a3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c5a3f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5a3f-120">Request headers</span></span>
|<span data-ttu-id="c5a3f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5a3f-121">Header</span></span>|<span data-ttu-id="c5a3f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5a3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a3f-123">Authorization</span></span>|<span data-ttu-id="c5a3f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5a3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a3f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5a3f-125">Accept</span></span>|<span data-ttu-id="c5a3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a3f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5a3f-127">Request body</span></span>
<span data-ttu-id="c5a3f-128">В тексте запроса укажите представление JSON для объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c5a3f-128">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="c5a3f-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-129">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="c5a3f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5a3f-130">Property</span></span>|<span data-ttu-id="c5a3f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5a3f-131">Type</span></span>|<span data-ttu-id="c5a3f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a3f-133">id</span><span class="sxs-lookup"><span data-stu-id="c5a3f-133">id</span></span>|<span data-ttu-id="c5a3f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c5a3f-134">String</span></span>|<span data-ttu-id="c5a3f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-135">Key of the entity.</span></span> <span data-ttu-id="c5a3f-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a3f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c5a3f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a3f-138">DateTimeOffset</span></span>|<span data-ttu-id="c5a3f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c5a3f-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5a3f-141">roleScopeTagIds</span></span>|<span data-ttu-id="c5a3f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c5a3f-142">String collection</span></span>|<span data-ttu-id="c5a3f-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5a3f-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5a3f-145">supportsScopeTags</span></span>|<span data-ttu-id="c5a3f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c5a3f-146">Boolean</span></span>|<span data-ttu-id="c5a3f-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5a3f-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5a3f-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5a3f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-150">This property is read-only.</span></span> <span data-ttu-id="c5a3f-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a3f-152">createdDateTime</span></span>|<span data-ttu-id="c5a3f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a3f-153">DateTimeOffset</span></span>|<span data-ttu-id="c5a3f-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-154">DateTime the object was created.</span></span> <span data-ttu-id="c5a3f-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-156">описание</span><span class="sxs-lookup"><span data-stu-id="c5a3f-156">description</span></span>|<span data-ttu-id="c5a3f-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c5a3f-157">String</span></span>|<span data-ttu-id="c5a3f-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5a3f-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c5a3f-160">displayName</span></span>|<span data-ttu-id="c5a3f-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c5a3f-161">String</span></span>|<span data-ttu-id="c5a3f-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5a3f-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-164">version</span><span class="sxs-lookup"><span data-stu-id="c5a3f-164">version</span></span>|<span data-ttu-id="c5a3f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a3f-165">Int32</span></span>|<span data-ttu-id="c5a3f-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-166">Version of the device configuration.</span></span> <span data-ttu-id="c5a3f-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a3f-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c5a3f-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="c5a3f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a3f-169">Int32</span></span>|<span data-ttu-id="c5a3f-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c5a3f-171">Допустимые значения от 1 до 99 унаследованные от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c5a3f-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c5a3f-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c5a3f-172">subjectNameFormat</span></span>|[<span data-ttu-id="c5a3f-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c5a3f-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c5a3f-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="c5a3f-175">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c5a3f-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c5a3f-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c5a3f-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c5a3f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a3f-178">Int32</span></span>|<span data-ttu-id="c5a3f-179">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c5a3f-180">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c5a3f-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c5a3f-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c5a3f-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c5a3f-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c5a3f-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c5a3f-183">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c5a3f-184">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c5a3f-185">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c5a3f-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c5a3f-186">extendedKeyUsages</span></span>|<span data-ttu-id="c5a3f-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c5a3f-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c5a3f-188">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c5a3f-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c5a3f-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c5a3f-190">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c5a3f-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c5a3f-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c5a3f-191">scepServerUrls</span></span>|<span data-ttu-id="c5a3f-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c5a3f-192">String collection</span></span>|<span data-ttu-id="c5a3f-193">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="c5a3f-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="c5a3f-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c5a3f-194">subjectNameFormatString</span></span>|<span data-ttu-id="c5a3f-195">Строка</span><span class="sxs-lookup"><span data-stu-id="c5a3f-195">String</span></span>|<span data-ttu-id="c5a3f-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c5a3f-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="c5a3f-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c5a3f-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="c5a3f-198">keyUsage</span></span>|[<span data-ttu-id="c5a3f-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="c5a3f-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c5a3f-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-200">SCEP Key Usage.</span></span> <span data-ttu-id="c5a3f-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c5a3f-202">keySize</span><span class="sxs-lookup"><span data-stu-id="c5a3f-202">keySize</span></span>|[<span data-ttu-id="c5a3f-203">keySize</span><span class="sxs-lookup"><span data-stu-id="c5a3f-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c5a3f-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-204">SCEP Key Size.</span></span> <span data-ttu-id="c5a3f-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c5a3f-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c5a3f-206">hashAlgorithm</span></span>|[<span data-ttu-id="c5a3f-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="c5a3f-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="c5a3f-208">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c5a3f-209">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c5a3f-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c5a3f-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c5a3f-211">Строка</span><span class="sxs-lookup"><span data-stu-id="c5a3f-211">String</span></span>|<span data-ttu-id="c5a3f-212">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c5a3f-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c5a3f-213">certificateStore</span></span>|[<span data-ttu-id="c5a3f-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c5a3f-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="c5a3f-215">Целевой хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-215">Target store certificate.</span></span> <span data-ttu-id="c5a3f-216">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c5a3f-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="c5a3f-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="c5a3f-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c5a3f-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="c5a3f-219">Параметры Alterantive имя настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="c5a3f-220">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c5a3f-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c5a3f-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c5a3f-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c5a3f-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c5a3f-223">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c5a3f-224">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="c5a3f-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5a3f-225">Response</span></span>
<span data-ttu-id="c5a3f-226">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-226">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a3f-227">Пример</span><span class="sxs-lookup"><span data-stu-id="c5a3f-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5a3f-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5a3f-228">Request</span></span>
<span data-ttu-id="c5a3f-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1194

{
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

### <a name="response"></a><span data-ttu-id="c5a3f-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5a3f-230">Response</span></span>
<span data-ttu-id="c5a3f-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5a3f-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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





