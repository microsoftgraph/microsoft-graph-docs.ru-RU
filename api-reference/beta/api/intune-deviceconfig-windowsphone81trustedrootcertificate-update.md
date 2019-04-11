---
title: Обновление windowsPhone81TrustedRootCertificate
description: Обновление свойств объекта windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0acc47bd427a61e9009db8ecb7cb16f65f0f2d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803523"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="10caf-103">Обновление windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="10caf-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="10caf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10caf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10caf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10caf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10caf-106">Обновление свойств объекта [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="10caf-106">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10caf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10caf-107">Prerequisites</span></span>
<span data-ttu-id="10caf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10caf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10caf-110">Permission type</span></span>|<span data-ttu-id="10caf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10caf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10caf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10caf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10caf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10caf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10caf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10caf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10caf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10caf-115">Not supported.</span></span>|
|<span data-ttu-id="10caf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10caf-116">Application</span></span>|<span data-ttu-id="10caf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10caf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10caf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10caf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="10caf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10caf-119">Request headers</span></span>
|<span data-ttu-id="10caf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10caf-120">Header</span></span>|<span data-ttu-id="10caf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10caf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10caf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10caf-122">Authorization</span></span>|<span data-ttu-id="10caf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10caf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10caf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10caf-124">Accept</span></span>|<span data-ttu-id="10caf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10caf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10caf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10caf-126">Request body</span></span>
<span data-ttu-id="10caf-127">В тексте запроса добавьте представление объекта [WindowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10caf-127">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="10caf-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-128">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="10caf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10caf-129">Property</span></span>|<span data-ttu-id="10caf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10caf-130">Type</span></span>|<span data-ttu-id="10caf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10caf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10caf-132">id</span><span class="sxs-lookup"><span data-stu-id="10caf-132">id</span></span>|<span data-ttu-id="10caf-133">Строка</span><span class="sxs-lookup"><span data-stu-id="10caf-133">String</span></span>|<span data-ttu-id="10caf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="10caf-134">Key of the entity.</span></span> <span data-ttu-id="10caf-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10caf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="10caf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10caf-137">DateTimeOffset</span></span>|<span data-ttu-id="10caf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="10caf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="10caf-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10caf-140">roleScopeTagIds</span></span>|<span data-ttu-id="10caf-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="10caf-141">String collection</span></span>|<span data-ttu-id="10caf-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="10caf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="10caf-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="10caf-144">supportsScopeTags</span></span>|<span data-ttu-id="10caf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="10caf-145">Boolean</span></span>|<span data-ttu-id="10caf-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="10caf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="10caf-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="10caf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="10caf-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="10caf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="10caf-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="10caf-149">This property is read-only.</span></span> <span data-ttu-id="10caf-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10caf-151">createdDateTime</span></span>|<span data-ttu-id="10caf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10caf-152">DateTimeOffset</span></span>|<span data-ttu-id="10caf-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="10caf-153">DateTime the object was created.</span></span> <span data-ttu-id="10caf-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-155">description</span><span class="sxs-lookup"><span data-stu-id="10caf-155">description</span></span>|<span data-ttu-id="10caf-156">String</span><span class="sxs-lookup"><span data-stu-id="10caf-156">String</span></span>|<span data-ttu-id="10caf-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="10caf-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="10caf-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="10caf-159">displayName</span></span>|<span data-ttu-id="10caf-160">String</span><span class="sxs-lookup"><span data-stu-id="10caf-160">String</span></span>|<span data-ttu-id="10caf-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="10caf-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="10caf-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-163">version</span><span class="sxs-lookup"><span data-stu-id="10caf-163">version</span></span>|<span data-ttu-id="10caf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="10caf-164">Int32</span></span>|<span data-ttu-id="10caf-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="10caf-165">Version of the device configuration.</span></span> <span data-ttu-id="10caf-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10caf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10caf-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="10caf-167">trustedRootCertificate</span></span>|<span data-ttu-id="10caf-168">Binary</span><span class="sxs-lookup"><span data-stu-id="10caf-168">Binary</span></span>|<span data-ttu-id="10caf-169">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="10caf-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="10caf-170">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="10caf-170">certFileName</span></span>|<span data-ttu-id="10caf-171">String</span><span class="sxs-lookup"><span data-stu-id="10caf-171">String</span></span>|<span data-ttu-id="10caf-172">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="10caf-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="10caf-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="10caf-173">Response</span></span>
<span data-ttu-id="10caf-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10caf-174">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10caf-175">Пример</span><span class="sxs-lookup"><span data-stu-id="10caf-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="10caf-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="10caf-176">Request</span></span>
<span data-ttu-id="10caf-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10caf-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="10caf-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="10caf-178">Response</span></span>
<span data-ttu-id="10caf-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10caf-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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
  "certFileName": "Cert File Name value"
}
```





