---
title: Обновление iosImportedPFXCertificateProfile
description: Обновление свойства объекта iosImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19c8eaabd05bcafa545bdfa93677c68df9f28dfb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929685"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="e8380-103">Обновление iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e8380-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="e8380-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8380-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8380-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8380-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8380-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e8380-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8380-107">Обновление свойства объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e8380-107">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8380-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8380-108">Prerequisites</span></span>
<span data-ttu-id="e8380-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8380-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8380-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8380-111">Permission type</span></span>|<span data-ttu-id="e8380-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8380-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8380-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8380-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8380-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8380-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8380-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8380-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8380-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8380-116">Not supported.</span></span>|
|<span data-ttu-id="e8380-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8380-117">Application</span></span>|<span data-ttu-id="e8380-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8380-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8380-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8380-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e8380-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8380-120">Request headers</span></span>
|<span data-ttu-id="e8380-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8380-121">Header</span></span>|<span data-ttu-id="e8380-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8380-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8380-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8380-123">Authorization</span></span>|<span data-ttu-id="e8380-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e8380-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8380-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8380-125">Accept</span></span>|<span data-ttu-id="e8380-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8380-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8380-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8380-127">Request body</span></span>
<span data-ttu-id="e8380-128">В тексте запроса укажите представление JSON для объекта [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e8380-128">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="e8380-129">В следующей таблице показаны свойства, которые необходимы для создания [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-129">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="e8380-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8380-130">Property</span></span>|<span data-ttu-id="e8380-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8380-131">Type</span></span>|<span data-ttu-id="e8380-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8380-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8380-133">id</span><span class="sxs-lookup"><span data-stu-id="e8380-133">id</span></span>|<span data-ttu-id="e8380-134">String</span><span class="sxs-lookup"><span data-stu-id="e8380-134">String</span></span>|<span data-ttu-id="e8380-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8380-135">Key of the entity.</span></span> <span data-ttu-id="e8380-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8380-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e8380-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8380-138">DateTimeOffset</span></span>|<span data-ttu-id="e8380-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e8380-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e8380-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8380-141">roleScopeTagIds</span></span>|<span data-ttu-id="e8380-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8380-142">String collection</span></span>|<span data-ttu-id="e8380-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e8380-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e8380-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e8380-145">supportsScopeTags</span></span>|<span data-ttu-id="e8380-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8380-146">Boolean</span></span>|<span data-ttu-id="e8380-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="e8380-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e8380-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="e8380-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e8380-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e8380-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e8380-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8380-150">This property is read-only.</span></span> <span data-ttu-id="e8380-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8380-152">createdDateTime</span></span>|<span data-ttu-id="e8380-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8380-153">DateTimeOffset</span></span>|<span data-ttu-id="e8380-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e8380-154">DateTime the object was created.</span></span> <span data-ttu-id="e8380-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-156">описание</span><span class="sxs-lookup"><span data-stu-id="e8380-156">description</span></span>|<span data-ttu-id="e8380-157">String</span><span class="sxs-lookup"><span data-stu-id="e8380-157">String</span></span>|<span data-ttu-id="e8380-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8380-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8380-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e8380-160">displayName</span></span>|<span data-ttu-id="e8380-161">String</span><span class="sxs-lookup"><span data-stu-id="e8380-161">String</span></span>|<span data-ttu-id="e8380-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8380-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8380-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-164">version</span><span class="sxs-lookup"><span data-stu-id="e8380-164">version</span></span>|<span data-ttu-id="e8380-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e8380-165">Int32</span></span>|<span data-ttu-id="e8380-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8380-166">Version of the device configuration.</span></span> <span data-ttu-id="e8380-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8380-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8380-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="e8380-168">intendedPurpose</span></span>|[<span data-ttu-id="e8380-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="e8380-169">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="e8380-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="e8380-170">Not yet documented.</span></span> <span data-ttu-id="e8380-171">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="e8380-171">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="e8380-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8380-172">Response</span></span>
<span data-ttu-id="e8380-173">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8380-173">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8380-174">Пример</span><span class="sxs-lookup"><span data-stu-id="e8380-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8380-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8380-175">Request</span></span>
<span data-ttu-id="e8380-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8380-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8380-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8380-177">Response</span></span>
<span data-ttu-id="e8380-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8380-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





