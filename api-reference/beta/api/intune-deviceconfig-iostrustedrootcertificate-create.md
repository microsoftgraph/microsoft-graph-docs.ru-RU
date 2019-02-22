---
title: Создание Иострустедрутцертификате
description: Создание нового объекта Иострустедрутцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f021e9a7d64589456cbbe48f87ef1434f6225a8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171843"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="ad8ea-103">Создание Иострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="ad8ea-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="ad8ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad8ea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad8ea-106">Создание нового объекта [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ad8ea-106">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad8ea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad8ea-107">Prerequisites</span></span>
<span data-ttu-id="ad8ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ad8ea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad8ea-110">Permission type</span></span>|<span data-ttu-id="ad8ea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad8ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad8ea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad8ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad8ea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8ea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad8ea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad8ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad8ea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-115">Not supported.</span></span>|
|<span data-ttu-id="ad8ea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad8ea-116">Application</span></span>|<span data-ttu-id="ad8ea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad8ea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad8ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="ad8ea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad8ea-119">Request headers</span></span>
|<span data-ttu-id="ad8ea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad8ea-120">Header</span></span>|<span data-ttu-id="ad8ea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ad8ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad8ea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad8ea-122">Authorization</span></span>|<span data-ttu-id="ad8ea-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad8ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad8ea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ad8ea-124">Accept</span></span>|<span data-ttu-id="ad8ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad8ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad8ea-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad8ea-126">Request body</span></span>
<span data-ttu-id="ad8ea-127">В тексте запроса добавьте представление объекта Иострустедрутцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-127">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="ad8ea-128">В следующей таблице приведены свойства, необходимые при создании Иострустедрутцертификате.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-128">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="ad8ea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad8ea-129">Property</span></span>|<span data-ttu-id="ad8ea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ad8ea-130">Type</span></span>|<span data-ttu-id="ad8ea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad8ea-132">id</span><span class="sxs-lookup"><span data-stu-id="ad8ea-132">id</span></span>|<span data-ttu-id="ad8ea-133">String</span><span class="sxs-lookup"><span data-stu-id="ad8ea-133">String</span></span>|<span data-ttu-id="ad8ea-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-134">Key of the entity.</span></span> <span data-ttu-id="ad8ea-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad8ea-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ad8ea-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad8ea-137">DateTimeOffset</span></span>|<span data-ttu-id="ad8ea-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ad8ea-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad8ea-140">roleScopeTagIds</span></span>|<span data-ttu-id="ad8ea-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad8ea-141">String collection</span></span>|<span data-ttu-id="ad8ea-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ad8ea-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ad8ea-144">supportsScopeTags</span></span>|<span data-ttu-id="ad8ea-145">Логический</span><span class="sxs-lookup"><span data-stu-id="ad8ea-145">Boolean</span></span>|<span data-ttu-id="ad8ea-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ad8ea-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ad8ea-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ad8ea-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-149">This property is read-only.</span></span> <span data-ttu-id="ad8ea-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad8ea-151">createdDateTime</span></span>|<span data-ttu-id="ad8ea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad8ea-152">DateTimeOffset</span></span>|<span data-ttu-id="ad8ea-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-153">DateTime the object was created.</span></span> <span data-ttu-id="ad8ea-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-155">description</span><span class="sxs-lookup"><span data-stu-id="ad8ea-155">description</span></span>|<span data-ttu-id="ad8ea-156">String</span><span class="sxs-lookup"><span data-stu-id="ad8ea-156">String</span></span>|<span data-ttu-id="ad8ea-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad8ea-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ad8ea-159">displayName</span></span>|<span data-ttu-id="ad8ea-160">String</span><span class="sxs-lookup"><span data-stu-id="ad8ea-160">String</span></span>|<span data-ttu-id="ad8ea-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad8ea-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-163">version</span><span class="sxs-lookup"><span data-stu-id="ad8ea-163">version</span></span>|<span data-ttu-id="ad8ea-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ad8ea-164">Int32</span></span>|<span data-ttu-id="ad8ea-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-165">Version of the device configuration.</span></span> <span data-ttu-id="ad8ea-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad8ea-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8ea-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ad8ea-167">trustedRootCertificate</span></span>|<span data-ttu-id="ad8ea-168">Binary</span><span class="sxs-lookup"><span data-stu-id="ad8ea-168">Binary</span></span>|<span data-ttu-id="ad8ea-169">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-169">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="ad8ea-170">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="ad8ea-170">certFileName</span></span>|<span data-ttu-id="ad8ea-171">String</span><span class="sxs-lookup"><span data-stu-id="ad8ea-171">String</span></span>|<span data-ttu-id="ad8ea-172">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="ad8ea-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad8ea-173">Response</span></span>
<span data-ttu-id="ad8ea-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-174">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad8ea-175">Пример</span><span class="sxs-lookup"><span data-stu-id="ad8ea-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad8ea-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad8ea-176">Request</span></span>
<span data-ttu-id="ad8ea-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="ad8ea-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad8ea-178">Response</span></span>
<span data-ttu-id="ad8ea-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad8ea-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




