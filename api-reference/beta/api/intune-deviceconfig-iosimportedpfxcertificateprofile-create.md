---
title: Создание Иосимпортедпфксцертификатепрофиле
description: Создание нового объекта Иосимпортедпфксцертификатепрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b53dbfb68420ff6d525319bab676746bbe6fef90
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467171"
---
# <a name="create-iosimportedpfxcertificateprofile"></a><span data-ttu-id="1a5e8-103">Создание Иосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="1a5e8-103">Create iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="1a5e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a5e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a5e8-106">Создание нового объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1a5e8-106">Create a new [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a5e8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1a5e8-107">Prerequisites</span></span>
<span data-ttu-id="1a5e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a5e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a5e8-110">Permission type</span></span>|<span data-ttu-id="1a5e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a5e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a5e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a5e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a5e8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a5e8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a5e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a5e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a5e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-115">Not supported.</span></span>|
|<span data-ttu-id="1a5e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a5e8-116">Application</span></span>|<span data-ttu-id="1a5e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a5e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a5e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a5e8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a5e8-119">Request headers</span></span>
|<span data-ttu-id="1a5e8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a5e8-120">Header</span></span>|<span data-ttu-id="1a5e8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a5e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a5e8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a5e8-122">Authorization</span></span>|<span data-ttu-id="1a5e8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a5e8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a5e8-124">Accept</span></span>|<span data-ttu-id="1a5e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a5e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a5e8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a5e8-126">Request body</span></span>
<span data-ttu-id="1a5e8-127">В тексте запроса добавьте представление объекта Иосимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-127">In the request body, supply a JSON representation for the iosImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="1a5e8-128">В следующей таблице приведены свойства, необходимые при создании Иосимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-128">The following table shows the properties that are required when you create the iosImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="1a5e8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a5e8-129">Property</span></span>|<span data-ttu-id="1a5e8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a5e8-130">Type</span></span>|<span data-ttu-id="1a5e8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a5e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a5e8-132">id</span><span class="sxs-lookup"><span data-stu-id="1a5e8-132">id</span></span>|<span data-ttu-id="1a5e8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1a5e8-133">String</span></span>|<span data-ttu-id="1a5e8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-134">Key of the entity.</span></span> <span data-ttu-id="1a5e8-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a5e8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1a5e8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a5e8-137">DateTimeOffset</span></span>|<span data-ttu-id="1a5e8-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1a5e8-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a5e8-140">roleScopeTagIds</span></span>|<span data-ttu-id="1a5e8-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1a5e8-141">String collection</span></span>|<span data-ttu-id="1a5e8-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a5e8-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1a5e8-144">supportsScopeTags</span></span>|<span data-ttu-id="1a5e8-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1a5e8-145">Boolean</span></span>|<span data-ttu-id="1a5e8-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a5e8-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a5e8-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a5e8-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-149">This property is read-only.</span></span> <span data-ttu-id="1a5e8-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a5e8-151">createdDateTime</span></span>|<span data-ttu-id="1a5e8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a5e8-152">DateTimeOffset</span></span>|<span data-ttu-id="1a5e8-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-153">DateTime the object was created.</span></span> <span data-ttu-id="1a5e8-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-155">description</span><span class="sxs-lookup"><span data-stu-id="1a5e8-155">description</span></span>|<span data-ttu-id="1a5e8-156">String</span><span class="sxs-lookup"><span data-stu-id="1a5e8-156">String</span></span>|<span data-ttu-id="1a5e8-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a5e8-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1a5e8-159">displayName</span></span>|<span data-ttu-id="1a5e8-160">String</span><span class="sxs-lookup"><span data-stu-id="1a5e8-160">String</span></span>|<span data-ttu-id="1a5e8-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a5e8-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-163">version</span><span class="sxs-lookup"><span data-stu-id="1a5e8-163">version</span></span>|<span data-ttu-id="1a5e8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5e8-164">Int32</span></span>|<span data-ttu-id="1a5e8-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-165">Version of the device configuration.</span></span> <span data-ttu-id="1a5e8-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5e8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5e8-167">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1a5e8-167">intendedPurpose</span></span>|[<span data-ttu-id="1a5e8-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1a5e8-168">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="1a5e8-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-169">Not yet documented.</span></span> <span data-ttu-id="1a5e8-170">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-170">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="1a5e8-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a5e8-171">Response</span></span>
<span data-ttu-id="1a5e8-172">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-172">If successful, this method returns a `201 Created` response code and a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a5e8-173">Пример</span><span class="sxs-lookup"><span data-stu-id="1a5e8-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a5e8-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a5e8-174">Request</span></span>
<span data-ttu-id="1a5e8-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="1a5e8-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a5e8-176">Response</span></span>
<span data-ttu-id="1a5e8-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a5e8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```





