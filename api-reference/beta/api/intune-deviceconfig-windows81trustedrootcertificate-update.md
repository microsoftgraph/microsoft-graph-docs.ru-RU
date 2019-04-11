---
title: Обновление windows81TrustedRootCertificate
description: Обновление свойств объекта windows81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f8a60362ce178a9aa42c92e9c469b58577096c8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774458"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="ed5a9-103">Обновление windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ed5a9-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="ed5a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed5a9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed5a9-106">Обновление свойств объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ed5a9-106">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed5a9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed5a9-107">Prerequisites</span></span>
<span data-ttu-id="ed5a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed5a9-110">Permission type</span></span>|<span data-ttu-id="ed5a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed5a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed5a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed5a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed5a9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed5a9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed5a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed5a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed5a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-115">Not supported.</span></span>|
|<span data-ttu-id="ed5a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed5a9-116">Application</span></span>|<span data-ttu-id="ed5a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed5a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed5a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="ed5a9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed5a9-119">Request headers</span></span>
|<span data-ttu-id="ed5a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed5a9-120">Header</span></span>|<span data-ttu-id="ed5a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ed5a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed5a9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed5a9-122">Authorization</span></span>|<span data-ttu-id="ed5a9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed5a9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ed5a9-124">Accept</span></span>|<span data-ttu-id="ed5a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed5a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed5a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed5a9-126">Request body</span></span>
<span data-ttu-id="ed5a9-127">В тексте запроса добавьте представление объекта [Windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-127">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="ed5a9-128">В следующей таблице приведены свойства, необходимые при создании [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-128">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="ed5a9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed5a9-129">Property</span></span>|<span data-ttu-id="ed5a9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ed5a9-130">Type</span></span>|<span data-ttu-id="ed5a9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ed5a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed5a9-132">id</span><span class="sxs-lookup"><span data-stu-id="ed5a9-132">id</span></span>|<span data-ttu-id="ed5a9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ed5a9-133">String</span></span>|<span data-ttu-id="ed5a9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-134">Key of the entity.</span></span> <span data-ttu-id="ed5a9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed5a9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ed5a9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed5a9-137">DateTimeOffset</span></span>|<span data-ttu-id="ed5a9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ed5a9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed5a9-140">roleScopeTagIds</span></span>|<span data-ttu-id="ed5a9-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ed5a9-141">String collection</span></span>|<span data-ttu-id="ed5a9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ed5a9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ed5a9-144">supportsScopeTags</span></span>|<span data-ttu-id="ed5a9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed5a9-145">Boolean</span></span>|<span data-ttu-id="ed5a9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ed5a9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ed5a9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ed5a9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-149">This property is read-only.</span></span> <span data-ttu-id="ed5a9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed5a9-151">createdDateTime</span></span>|<span data-ttu-id="ed5a9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed5a9-152">DateTimeOffset</span></span>|<span data-ttu-id="ed5a9-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-153">DateTime the object was created.</span></span> <span data-ttu-id="ed5a9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-155">description</span><span class="sxs-lookup"><span data-stu-id="ed5a9-155">description</span></span>|<span data-ttu-id="ed5a9-156">String</span><span class="sxs-lookup"><span data-stu-id="ed5a9-156">String</span></span>|<span data-ttu-id="ed5a9-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed5a9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ed5a9-159">displayName</span></span>|<span data-ttu-id="ed5a9-160">String</span><span class="sxs-lookup"><span data-stu-id="ed5a9-160">String</span></span>|<span data-ttu-id="ed5a9-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed5a9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-163">version</span><span class="sxs-lookup"><span data-stu-id="ed5a9-163">version</span></span>|<span data-ttu-id="ed5a9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ed5a9-164">Int32</span></span>|<span data-ttu-id="ed5a9-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-165">Version of the device configuration.</span></span> <span data-ttu-id="ed5a9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed5a9-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ed5a9-167">trustedRootCertificate</span></span>|<span data-ttu-id="ed5a9-168">Binary</span><span class="sxs-lookup"><span data-stu-id="ed5a9-168">Binary</span></span>|<span data-ttu-id="ed5a9-169">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="ed5a9-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="ed5a9-170">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="ed5a9-170">certFileName</span></span>|<span data-ttu-id="ed5a9-171">String</span><span class="sxs-lookup"><span data-stu-id="ed5a9-171">String</span></span>|<span data-ttu-id="ed5a9-172">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-172">File name to display in UI.</span></span>|
|<span data-ttu-id="ed5a9-173">Дестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="ed5a9-173">destinationStore</span></span>|[<span data-ttu-id="ed5a9-174">Цертификатедестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="ed5a9-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="ed5a9-175">Расположение хранилища назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="ed5a9-176">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="ed5a9-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed5a9-177">Response</span></span>
<span data-ttu-id="ed5a9-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-178">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed5a9-179">Пример</span><span class="sxs-lookup"><span data-stu-id="ed5a9-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed5a9-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed5a9-180">Request</span></span>
<span data-ttu-id="ed5a9-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="ed5a9-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed5a9-182">Response</span></span>
<span data-ttu-id="ed5a9-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed5a9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```





