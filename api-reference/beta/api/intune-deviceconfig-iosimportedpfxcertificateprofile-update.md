---
title: Обновление iosImportedPFXCertificateProfile
description: Обновление свойства объекта iosImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b5e851d13b0e3d5ec65671fc712f9402c67474a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407944"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="72f06-103">Обновление iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="72f06-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="72f06-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72f06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72f06-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72f06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72f06-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72f06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72f06-107">Обновление свойства объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="72f06-107">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72f06-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="72f06-108">Prerequisites</span></span>
<span data-ttu-id="72f06-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="72f06-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72f06-111">Permission type</span></span>|<span data-ttu-id="72f06-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72f06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72f06-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72f06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72f06-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72f06-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72f06-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72f06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72f06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72f06-116">Not supported.</span></span>|
|<span data-ttu-id="72f06-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72f06-117">Application</span></span>|<span data-ttu-id="72f06-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72f06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72f06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72f06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="72f06-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72f06-120">Request headers</span></span>
|<span data-ttu-id="72f06-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72f06-121">Header</span></span>|<span data-ttu-id="72f06-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72f06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72f06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72f06-123">Authorization</span></span>|<span data-ttu-id="72f06-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="72f06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72f06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72f06-125">Accept</span></span>|<span data-ttu-id="72f06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72f06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72f06-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72f06-127">Request body</span></span>
<span data-ttu-id="72f06-128">В тексте запроса укажите представление JSON для объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="72f06-128">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="72f06-129">В следующей таблице показаны свойства, которые необходимы для создания [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-129">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="72f06-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72f06-130">Property</span></span>|<span data-ttu-id="72f06-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72f06-131">Type</span></span>|<span data-ttu-id="72f06-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72f06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72f06-133">id</span><span class="sxs-lookup"><span data-stu-id="72f06-133">id</span></span>|<span data-ttu-id="72f06-134">String</span><span class="sxs-lookup"><span data-stu-id="72f06-134">String</span></span>|<span data-ttu-id="72f06-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72f06-135">Key of the entity.</span></span> <span data-ttu-id="72f06-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72f06-137">lastModifiedDateTime</span></span>|<span data-ttu-id="72f06-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72f06-138">DateTimeOffset</span></span>|<span data-ttu-id="72f06-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="72f06-139">DateTime the object was last modified.</span></span> <span data-ttu-id="72f06-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="72f06-141">roleScopeTagIds</span></span>|<span data-ttu-id="72f06-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="72f06-142">String collection</span></span>|<span data-ttu-id="72f06-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="72f06-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="72f06-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="72f06-145">supportsScopeTags</span></span>|<span data-ttu-id="72f06-146">Логический</span><span class="sxs-lookup"><span data-stu-id="72f06-146">Boolean</span></span>|<span data-ttu-id="72f06-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="72f06-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="72f06-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="72f06-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="72f06-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="72f06-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="72f06-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f06-150">This property is read-only.</span></span> <span data-ttu-id="72f06-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72f06-152">createdDateTime</span></span>|<span data-ttu-id="72f06-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72f06-153">DateTimeOffset</span></span>|<span data-ttu-id="72f06-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="72f06-154">DateTime the object was created.</span></span> <span data-ttu-id="72f06-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-156">description</span><span class="sxs-lookup"><span data-stu-id="72f06-156">description</span></span>|<span data-ttu-id="72f06-157">String</span><span class="sxs-lookup"><span data-stu-id="72f06-157">String</span></span>|<span data-ttu-id="72f06-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="72f06-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72f06-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-160">displayName</span><span class="sxs-lookup"><span data-stu-id="72f06-160">displayName</span></span>|<span data-ttu-id="72f06-161">String</span><span class="sxs-lookup"><span data-stu-id="72f06-161">String</span></span>|<span data-ttu-id="72f06-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="72f06-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72f06-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-164">version</span><span class="sxs-lookup"><span data-stu-id="72f06-164">version</span></span>|<span data-ttu-id="72f06-165">Int32</span><span class="sxs-lookup"><span data-stu-id="72f06-165">Int32</span></span>|<span data-ttu-id="72f06-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="72f06-166">Version of the device configuration.</span></span> <span data-ttu-id="72f06-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72f06-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72f06-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="72f06-168">intendedPurpose</span></span>|[<span data-ttu-id="72f06-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="72f06-169">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="72f06-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="72f06-170">Not yet documented.</span></span> <span data-ttu-id="72f06-171">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="72f06-171">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="72f06-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="72f06-172">Response</span></span>
<span data-ttu-id="72f06-173">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="72f06-173">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72f06-174">Пример</span><span class="sxs-lookup"><span data-stu-id="72f06-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="72f06-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="72f06-175">Request</span></span>
<span data-ttu-id="72f06-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72f06-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="72f06-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="72f06-177">Response</span></span>
<span data-ttu-id="72f06-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="72f06-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




