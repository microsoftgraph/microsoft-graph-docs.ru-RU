---
title: Создание windows81TrustedRootCertificate
description: Создание нового объекта windows81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d3c0c6bc0fda2623e2cfd5fbdf96c275dd1e47b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776208"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="5ae8d-103">Создание windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5ae8d-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="5ae8d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ae8d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ae8d-106">Создание нового объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="5ae8d-106">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ae8d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ae8d-107">Prerequisites</span></span>
<span data-ttu-id="5ae8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae8d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ae8d-110">Permission type</span></span>|<span data-ttu-id="5ae8d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ae8d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae8d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ae8d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae8d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae8d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae8d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ae8d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-115">Not supported.</span></span>|
|<span data-ttu-id="5ae8d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ae8d-116">Application</span></span>|<span data-ttu-id="5ae8d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae8d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ae8d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="5ae8d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ae8d-119">Request headers</span></span>
|<span data-ttu-id="5ae8d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ae8d-120">Header</span></span>|<span data-ttu-id="5ae8d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5ae8d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ae8d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ae8d-122">Authorization</span></span>|<span data-ttu-id="5ae8d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ae8d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5ae8d-124">Accept</span></span>|<span data-ttu-id="5ae8d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae8d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae8d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ae8d-126">Request body</span></span>
<span data-ttu-id="5ae8d-127">В тексте запроса добавьте представление объекта windows81TrustedRootCertificate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-127">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="5ae8d-128">В следующей таблице приведены свойства, необходимые при создании windows81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-128">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="5ae8d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ae8d-129">Property</span></span>|<span data-ttu-id="5ae8d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5ae8d-130">Type</span></span>|<span data-ttu-id="5ae8d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5ae8d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae8d-132">id</span><span class="sxs-lookup"><span data-stu-id="5ae8d-132">id</span></span>|<span data-ttu-id="5ae8d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5ae8d-133">String</span></span>|<span data-ttu-id="5ae8d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-134">Key of the entity.</span></span> <span data-ttu-id="5ae8d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae8d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ae8d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae8d-137">DateTimeOffset</span></span>|<span data-ttu-id="5ae8d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ae8d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ae8d-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ae8d-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5ae8d-141">String collection</span></span>|<span data-ttu-id="5ae8d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ae8d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5ae8d-144">supportsScopeTags</span></span>|<span data-ttu-id="5ae8d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ae8d-145">Boolean</span></span>|<span data-ttu-id="5ae8d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ae8d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ae8d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ae8d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-149">This property is read-only.</span></span> <span data-ttu-id="5ae8d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae8d-151">createdDateTime</span></span>|<span data-ttu-id="5ae8d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae8d-152">DateTimeOffset</span></span>|<span data-ttu-id="5ae8d-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-153">DateTime the object was created.</span></span> <span data-ttu-id="5ae8d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-155">description</span><span class="sxs-lookup"><span data-stu-id="5ae8d-155">description</span></span>|<span data-ttu-id="5ae8d-156">String</span><span class="sxs-lookup"><span data-stu-id="5ae8d-156">String</span></span>|<span data-ttu-id="5ae8d-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ae8d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5ae8d-159">displayName</span></span>|<span data-ttu-id="5ae8d-160">String</span><span class="sxs-lookup"><span data-stu-id="5ae8d-160">String</span></span>|<span data-ttu-id="5ae8d-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ae8d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-163">version</span><span class="sxs-lookup"><span data-stu-id="5ae8d-163">version</span></span>|<span data-ttu-id="5ae8d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae8d-164">Int32</span></span>|<span data-ttu-id="5ae8d-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-165">Version of the device configuration.</span></span> <span data-ttu-id="5ae8d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ae8d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ae8d-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5ae8d-167">trustedRootCertificate</span></span>|<span data-ttu-id="5ae8d-168">Binary</span><span class="sxs-lookup"><span data-stu-id="5ae8d-168">Binary</span></span>|<span data-ttu-id="5ae8d-169">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="5ae8d-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="5ae8d-170">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="5ae8d-170">certFileName</span></span>|<span data-ttu-id="5ae8d-171">String</span><span class="sxs-lookup"><span data-stu-id="5ae8d-171">String</span></span>|<span data-ttu-id="5ae8d-172">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-172">File name to display in UI.</span></span>|
|<span data-ttu-id="5ae8d-173">Дестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="5ae8d-173">destinationStore</span></span>|[<span data-ttu-id="5ae8d-174">Цертификатедестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="5ae8d-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="5ae8d-175">Расположение хранилища назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="5ae8d-176">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="5ae8d-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae8d-177">Response</span></span>
<span data-ttu-id="5ae8d-178">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-178">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ae8d-179">Пример</span><span class="sxs-lookup"><span data-stu-id="5ae8d-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ae8d-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ae8d-180">Request</span></span>
<span data-ttu-id="5ae8d-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="5ae8d-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae8d-182">Response</span></span>
<span data-ttu-id="5ae8d-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ae8d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





