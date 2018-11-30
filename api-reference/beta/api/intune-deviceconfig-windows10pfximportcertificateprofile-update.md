---
title: Обновление windows10PFXImportCertificateProfile
description: Обновление свойства объекта windows10PFXImportCertificateProfile.
ms.openlocfilehash: 087314950ead6e31fb8a74cff6b20ec9060d9935
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081779"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="06026-103">Обновление windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="06026-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="06026-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06026-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06026-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06026-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06026-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06026-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06026-107">Обновление свойства объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="06026-107">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06026-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06026-108">Prerequisites</span></span>
<span data-ttu-id="06026-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06026-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06026-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06026-111">Permission type</span></span>|<span data-ttu-id="06026-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06026-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06026-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06026-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06026-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06026-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06026-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06026-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06026-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06026-116">Not supported.</span></span>|
|<span data-ttu-id="06026-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06026-117">Application</span></span>|<span data-ttu-id="06026-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06026-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06026-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06026-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06026-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06026-120">Request headers</span></span>
|<span data-ttu-id="06026-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06026-121">Header</span></span>|<span data-ttu-id="06026-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06026-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06026-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06026-123">Authorization</span></span>|<span data-ttu-id="06026-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="06026-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06026-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06026-125">Accept</span></span>|<span data-ttu-id="06026-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06026-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06026-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06026-127">Request body</span></span>
<span data-ttu-id="06026-128">В тексте запроса укажите представление JSON для объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="06026-128">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="06026-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="06026-129">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="06026-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06026-130">Property</span></span>|<span data-ttu-id="06026-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06026-131">Type</span></span>|<span data-ttu-id="06026-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06026-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06026-133">id</span><span class="sxs-lookup"><span data-stu-id="06026-133">id</span></span>|<span data-ttu-id="06026-134">String</span><span class="sxs-lookup"><span data-stu-id="06026-134">String</span></span>|<span data-ttu-id="06026-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="06026-135">Key of the entity.</span></span> <span data-ttu-id="06026-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06026-137">lastModifiedDateTime</span></span>|<span data-ttu-id="06026-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06026-138">DateTimeOffset</span></span>|<span data-ttu-id="06026-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="06026-139">DateTime the object was last modified.</span></span> <span data-ttu-id="06026-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06026-141">roleScopeTagIds</span></span>|<span data-ttu-id="06026-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06026-142">String collection</span></span>|<span data-ttu-id="06026-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="06026-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06026-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06026-145">supportsScopeTags</span></span>|<span data-ttu-id="06026-146">Логический</span><span class="sxs-lookup"><span data-stu-id="06026-146">Boolean</span></span>|<span data-ttu-id="06026-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="06026-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06026-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="06026-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06026-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="06026-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06026-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06026-150">This property is read-only.</span></span> <span data-ttu-id="06026-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06026-152">createdDateTime</span></span>|<span data-ttu-id="06026-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06026-153">DateTimeOffset</span></span>|<span data-ttu-id="06026-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="06026-154">DateTime the object was created.</span></span> <span data-ttu-id="06026-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-156">описание</span><span class="sxs-lookup"><span data-stu-id="06026-156">description</span></span>|<span data-ttu-id="06026-157">String</span><span class="sxs-lookup"><span data-stu-id="06026-157">String</span></span>|<span data-ttu-id="06026-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06026-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06026-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-160">displayName</span><span class="sxs-lookup"><span data-stu-id="06026-160">displayName</span></span>|<span data-ttu-id="06026-161">String</span><span class="sxs-lookup"><span data-stu-id="06026-161">String</span></span>|<span data-ttu-id="06026-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06026-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06026-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-164">version</span><span class="sxs-lookup"><span data-stu-id="06026-164">version</span></span>|<span data-ttu-id="06026-165">Int32</span><span class="sxs-lookup"><span data-stu-id="06026-165">Int32</span></span>|<span data-ttu-id="06026-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06026-166">Version of the device configuration.</span></span> <span data-ttu-id="06026-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06026-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06026-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="06026-168">keyStorageProvider</span></span>|[<span data-ttu-id="06026-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="06026-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="06026-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="06026-170">Not yet documented.</span></span> <span data-ttu-id="06026-171">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="06026-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="06026-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="06026-172">Response</span></span>
<span data-ttu-id="06026-173">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06026-173">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06026-174">Пример</span><span class="sxs-lookup"><span data-stu-id="06026-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="06026-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="06026-175">Request</span></span>
<span data-ttu-id="06026-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06026-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 306

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="06026-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="06026-177">Response</span></span>
<span data-ttu-id="06026-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="06026-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





