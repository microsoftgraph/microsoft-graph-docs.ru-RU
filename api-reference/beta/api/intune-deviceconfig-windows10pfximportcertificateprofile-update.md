---
title: Обновление windows10PFXImportCertificateProfile
description: Обновление свойств объекта windows10PFXImportCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77495930295654e04658f7908c3909a8c0c4863e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515773"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="65793-103">Обновление windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="65793-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="65793-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65793-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65793-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65793-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65793-106">Обновление свойств объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="65793-106">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65793-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65793-107">Prerequisites</span></span>
<span data-ttu-id="65793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65793-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65793-110">Permission type</span></span>|<span data-ttu-id="65793-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65793-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65793-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65793-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65793-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65793-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65793-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65793-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65793-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65793-115">Not supported.</span></span>|
|<span data-ttu-id="65793-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65793-116">Application</span></span>|<span data-ttu-id="65793-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65793-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65793-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65793-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="65793-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65793-119">Request headers</span></span>
|<span data-ttu-id="65793-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65793-120">Header</span></span>|<span data-ttu-id="65793-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65793-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65793-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65793-122">Authorization</span></span>|<span data-ttu-id="65793-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65793-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65793-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65793-124">Accept</span></span>|<span data-ttu-id="65793-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65793-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65793-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65793-126">Request body</span></span>
<span data-ttu-id="65793-127">В тексте запроса добавьте представление объекта [Windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65793-127">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="65793-128">В следующей таблице приведены свойства, необходимые при создании [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="65793-128">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="65793-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="65793-129">Property</span></span>|<span data-ttu-id="65793-130">Тип</span><span class="sxs-lookup"><span data-stu-id="65793-130">Type</span></span>|<span data-ttu-id="65793-131">Описание</span><span class="sxs-lookup"><span data-stu-id="65793-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65793-132">id</span><span class="sxs-lookup"><span data-stu-id="65793-132">id</span></span>|<span data-ttu-id="65793-133">Строка</span><span class="sxs-lookup"><span data-stu-id="65793-133">String</span></span>|<span data-ttu-id="65793-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65793-134">Key of the entity.</span></span> <span data-ttu-id="65793-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65793-136">lastModifiedDateTime</span></span>|<span data-ttu-id="65793-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65793-137">DateTimeOffset</span></span>|<span data-ttu-id="65793-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="65793-138">DateTime the object was last modified.</span></span> <span data-ttu-id="65793-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65793-140">roleScopeTagIds</span></span>|<span data-ttu-id="65793-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65793-141">String collection</span></span>|<span data-ttu-id="65793-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="65793-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65793-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="65793-144">supportsScopeTags</span></span>|<span data-ttu-id="65793-145">Логический</span><span class="sxs-lookup"><span data-stu-id="65793-145">Boolean</span></span>|<span data-ttu-id="65793-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="65793-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65793-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="65793-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65793-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="65793-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65793-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65793-149">This property is read-only.</span></span> <span data-ttu-id="65793-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65793-151">createdDateTime</span></span>|<span data-ttu-id="65793-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65793-152">DateTimeOffset</span></span>|<span data-ttu-id="65793-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="65793-153">DateTime the object was created.</span></span> <span data-ttu-id="65793-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-155">description</span><span class="sxs-lookup"><span data-stu-id="65793-155">description</span></span>|<span data-ttu-id="65793-156">String</span><span class="sxs-lookup"><span data-stu-id="65793-156">String</span></span>|<span data-ttu-id="65793-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65793-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65793-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-159">displayName</span><span class="sxs-lookup"><span data-stu-id="65793-159">displayName</span></span>|<span data-ttu-id="65793-160">String</span><span class="sxs-lookup"><span data-stu-id="65793-160">String</span></span>|<span data-ttu-id="65793-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65793-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65793-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-163">version</span><span class="sxs-lookup"><span data-stu-id="65793-163">version</span></span>|<span data-ttu-id="65793-164">Int32</span><span class="sxs-lookup"><span data-stu-id="65793-164">Int32</span></span>|<span data-ttu-id="65793-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65793-165">Version of the device configuration.</span></span> <span data-ttu-id="65793-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65793-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65793-167">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="65793-167">keyStorageProvider</span></span>|[<span data-ttu-id="65793-168">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="65793-168">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="65793-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="65793-169">Not yet documented.</span></span> <span data-ttu-id="65793-170">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="65793-170">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="65793-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="65793-171">Response</span></span>
<span data-ttu-id="65793-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65793-172">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65793-173">Пример</span><span class="sxs-lookup"><span data-stu-id="65793-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="65793-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="65793-174">Request</span></span>
<span data-ttu-id="65793-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65793-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="65793-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="65793-176">Response</span></span>
<span data-ttu-id="65793-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65793-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





