---
title: Обновление iosImportedPFXCertificateProfile
description: Обновление свойства объекта iosImportedPFXCertificateProfile.
ms.openlocfilehash: 4f44664571ae116403d5403263e3839a0ab45443
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075207"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="ed94e-103">Обновление iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ed94e-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="ed94e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed94e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed94e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed94e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed94e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed94e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed94e-107">Обновление свойства объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ed94e-107">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed94e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed94e-108">Prerequisites</span></span>
<span data-ttu-id="ed94e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed94e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed94e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed94e-111">Permission type</span></span>|<span data-ttu-id="ed94e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed94e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed94e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed94e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed94e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed94e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed94e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed94e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed94e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed94e-116">Not supported.</span></span>|
|<span data-ttu-id="ed94e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed94e-117">Application</span></span>|<span data-ttu-id="ed94e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed94e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed94e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed94e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ed94e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed94e-120">Request headers</span></span>
|<span data-ttu-id="ed94e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed94e-121">Header</span></span>|<span data-ttu-id="ed94e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ed94e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed94e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed94e-123">Authorization</span></span>|<span data-ttu-id="ed94e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed94e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed94e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed94e-125">Accept</span></span>|<span data-ttu-id="ed94e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed94e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed94e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed94e-127">Request body</span></span>
<span data-ttu-id="ed94e-128">В тексте запроса укажите представление JSON для объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ed94e-128">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="ed94e-129">В следующей таблице показаны свойства, которые необходимы для создания [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-129">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="ed94e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed94e-130">Property</span></span>|<span data-ttu-id="ed94e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ed94e-131">Type</span></span>|<span data-ttu-id="ed94e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ed94e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed94e-133">id</span><span class="sxs-lookup"><span data-stu-id="ed94e-133">id</span></span>|<span data-ttu-id="ed94e-134">String</span><span class="sxs-lookup"><span data-stu-id="ed94e-134">String</span></span>|<span data-ttu-id="ed94e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed94e-135">Key of the entity.</span></span> <span data-ttu-id="ed94e-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed94e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ed94e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed94e-138">DateTimeOffset</span></span>|<span data-ttu-id="ed94e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ed94e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ed94e-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed94e-141">roleScopeTagIds</span></span>|<span data-ttu-id="ed94e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ed94e-142">String collection</span></span>|<span data-ttu-id="ed94e-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ed94e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ed94e-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ed94e-145">supportsScopeTags</span></span>|<span data-ttu-id="ed94e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ed94e-146">Boolean</span></span>|<span data-ttu-id="ed94e-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ed94e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ed94e-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ed94e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ed94e-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ed94e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ed94e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed94e-150">This property is read-only.</span></span> <span data-ttu-id="ed94e-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed94e-152">createdDateTime</span></span>|<span data-ttu-id="ed94e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed94e-153">DateTimeOffset</span></span>|<span data-ttu-id="ed94e-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ed94e-154">DateTime the object was created.</span></span> <span data-ttu-id="ed94e-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-156">описание</span><span class="sxs-lookup"><span data-stu-id="ed94e-156">description</span></span>|<span data-ttu-id="ed94e-157">String</span><span class="sxs-lookup"><span data-stu-id="ed94e-157">String</span></span>|<span data-ttu-id="ed94e-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed94e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed94e-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ed94e-160">displayName</span></span>|<span data-ttu-id="ed94e-161">String</span><span class="sxs-lookup"><span data-stu-id="ed94e-161">String</span></span>|<span data-ttu-id="ed94e-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed94e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed94e-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-164">version</span><span class="sxs-lookup"><span data-stu-id="ed94e-164">version</span></span>|<span data-ttu-id="ed94e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ed94e-165">Int32</span></span>|<span data-ttu-id="ed94e-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed94e-166">Version of the device configuration.</span></span> <span data-ttu-id="ed94e-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed94e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed94e-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ed94e-168">intendedPurpose</span></span>|[<span data-ttu-id="ed94e-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ed94e-169">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="ed94e-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="ed94e-170">Not yet documented.</span></span> <span data-ttu-id="ed94e-171">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="ed94e-171">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="ed94e-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed94e-172">Response</span></span>
<span data-ttu-id="ed94e-173">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ed94e-173">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed94e-174">Пример</span><span class="sxs-lookup"><span data-stu-id="ed94e-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed94e-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed94e-175">Request</span></span>
<span data-ttu-id="ed94e-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed94e-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 296

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="ed94e-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed94e-177">Response</span></span>
<span data-ttu-id="ed94e-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ed94e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





