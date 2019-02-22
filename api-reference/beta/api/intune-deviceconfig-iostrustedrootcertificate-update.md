---
title: Обновление Иострустедрутцертификате
description: Обновление свойств объекта Иострустедрутцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2436cd551e2e84e128b620d4ff2d06a28a0670a4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165641"
---
# <a name="update-iostrustedrootcertificate"></a><span data-ttu-id="aaa05-103">Обновление Иострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="aaa05-103">Update iosTrustedRootCertificate</span></span>

> <span data-ttu-id="aaa05-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaa05-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aaa05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaa05-106">Обновление свойств объекта [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="aaa05-106">Update the properties of a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaa05-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aaa05-107">Prerequisites</span></span>
<span data-ttu-id="aaa05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aaa05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa05-110">Permission type</span></span>|<span data-ttu-id="aaa05-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaa05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaa05-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaa05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aaa05-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaa05-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aaa05-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaa05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaa05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa05-115">Not supported.</span></span>|
|<span data-ttu-id="aaa05-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaa05-116">Application</span></span>|<span data-ttu-id="aaa05-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaa05-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaa05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="aaa05-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaa05-119">Request headers</span></span>
|<span data-ttu-id="aaa05-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aaa05-120">Header</span></span>|<span data-ttu-id="aaa05-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aaa05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaa05-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaa05-122">Authorization</span></span>|<span data-ttu-id="aaa05-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aaa05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaa05-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aaa05-124">Accept</span></span>|<span data-ttu-id="aaa05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aaa05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaa05-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaa05-126">Request body</span></span>
<span data-ttu-id="aaa05-127">В тексте запроса добавьте представление объекта [Иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaa05-127">In the request body, supply a JSON representation for the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="aaa05-128">В следующей таблице приведены свойства, необходимые при создании [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-128">The following table shows the properties that are required when you create the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="aaa05-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaa05-129">Property</span></span>|<span data-ttu-id="aaa05-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aaa05-130">Type</span></span>|<span data-ttu-id="aaa05-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaa05-132">id</span><span class="sxs-lookup"><span data-stu-id="aaa05-132">id</span></span>|<span data-ttu-id="aaa05-133">String</span><span class="sxs-lookup"><span data-stu-id="aaa05-133">String</span></span>|<span data-ttu-id="aaa05-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aaa05-134">Key of the entity.</span></span> <span data-ttu-id="aaa05-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaa05-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aaa05-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaa05-137">DateTimeOffset</span></span>|<span data-ttu-id="aaa05-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aaa05-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aaa05-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aaa05-140">roleScopeTagIds</span></span>|<span data-ttu-id="aaa05-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aaa05-141">String collection</span></span>|<span data-ttu-id="aaa05-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="aaa05-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aaa05-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="aaa05-144">supportsScopeTags</span></span>|<span data-ttu-id="aaa05-145">Логический</span><span class="sxs-lookup"><span data-stu-id="aaa05-145">Boolean</span></span>|<span data-ttu-id="aaa05-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="aaa05-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aaa05-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="aaa05-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aaa05-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="aaa05-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aaa05-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aaa05-149">This property is read-only.</span></span> <span data-ttu-id="aaa05-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaa05-151">createdDateTime</span></span>|<span data-ttu-id="aaa05-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaa05-152">DateTimeOffset</span></span>|<span data-ttu-id="aaa05-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aaa05-153">DateTime the object was created.</span></span> <span data-ttu-id="aaa05-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-155">description</span><span class="sxs-lookup"><span data-stu-id="aaa05-155">description</span></span>|<span data-ttu-id="aaa05-156">String</span><span class="sxs-lookup"><span data-stu-id="aaa05-156">String</span></span>|<span data-ttu-id="aaa05-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aaa05-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aaa05-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-159">displayName</span><span class="sxs-lookup"><span data-stu-id="aaa05-159">displayName</span></span>|<span data-ttu-id="aaa05-160">String</span><span class="sxs-lookup"><span data-stu-id="aaa05-160">String</span></span>|<span data-ttu-id="aaa05-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aaa05-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aaa05-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-163">version</span><span class="sxs-lookup"><span data-stu-id="aaa05-163">version</span></span>|<span data-ttu-id="aaa05-164">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa05-164">Int32</span></span>|<span data-ttu-id="aaa05-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aaa05-165">Version of the device configuration.</span></span> <span data-ttu-id="aaa05-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaa05-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aaa05-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="aaa05-167">trustedRootCertificate</span></span>|<span data-ttu-id="aaa05-168">Binary</span><span class="sxs-lookup"><span data-stu-id="aaa05-168">Binary</span></span>|<span data-ttu-id="aaa05-169">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="aaa05-169">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="aaa05-170">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="aaa05-170">certFileName</span></span>|<span data-ttu-id="aaa05-171">String</span><span class="sxs-lookup"><span data-stu-id="aaa05-171">String</span></span>|<span data-ttu-id="aaa05-172">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="aaa05-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="aaa05-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa05-173">Response</span></span>
<span data-ttu-id="aaa05-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaa05-174">If successful, this method returns a `200 OK` response code and an updated [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaa05-175">Пример</span><span class="sxs-lookup"><span data-stu-id="aaa05-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaa05-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaa05-176">Request</span></span>
<span data-ttu-id="aaa05-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaa05-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="aaa05-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa05-178">Response</span></span>
<span data-ttu-id="aaa05-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaa05-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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




