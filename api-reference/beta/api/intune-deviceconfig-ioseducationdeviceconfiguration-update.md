---
title: Обновление iosEducationDeviceConfiguration
description: Обновление свойства объекта iosEducationDeviceConfiguration.
ms.openlocfilehash: 071d3162ca001eb3d52d75b5b6934c44df691bf0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080246"
---
# <a name="update-ioseducationdeviceconfiguration"></a><span data-ttu-id="30aa0-103">Обновление iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="30aa0-103">Update iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="30aa0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30aa0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30aa0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30aa0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30aa0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="30aa0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30aa0-107">Обновление свойства объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="30aa0-107">Update the properties of a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30aa0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30aa0-108">Prerequisites</span></span>
<span data-ttu-id="30aa0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30aa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30aa0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30aa0-111">Permission type</span></span>|<span data-ttu-id="30aa0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30aa0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30aa0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30aa0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30aa0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30aa0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30aa0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30aa0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30aa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30aa0-116">Not supported.</span></span>|
|<span data-ttu-id="30aa0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30aa0-117">Application</span></span>|<span data-ttu-id="30aa0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30aa0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30aa0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30aa0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="30aa0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30aa0-120">Request headers</span></span>
|<span data-ttu-id="30aa0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30aa0-121">Header</span></span>|<span data-ttu-id="30aa0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30aa0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30aa0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30aa0-123">Authorization</span></span>|<span data-ttu-id="30aa0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="30aa0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30aa0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30aa0-125">Accept</span></span>|<span data-ttu-id="30aa0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30aa0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30aa0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30aa0-127">Request body</span></span>
<span data-ttu-id="30aa0-128">В тексте запроса укажите представление JSON для объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="30aa0-128">In the request body, supply a JSON representation for the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="30aa0-129">В следующей таблице показаны свойства, которые необходимы для создания [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-129">The following table shows the properties that are required when you create the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

|<span data-ttu-id="30aa0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30aa0-130">Property</span></span>|<span data-ttu-id="30aa0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30aa0-131">Type</span></span>|<span data-ttu-id="30aa0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30aa0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30aa0-133">id</span><span class="sxs-lookup"><span data-stu-id="30aa0-133">id</span></span>|<span data-ttu-id="30aa0-134">String</span><span class="sxs-lookup"><span data-stu-id="30aa0-134">String</span></span>|<span data-ttu-id="30aa0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30aa0-135">Key of the entity.</span></span> <span data-ttu-id="30aa0-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30aa0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="30aa0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30aa0-138">DateTimeOffset</span></span>|<span data-ttu-id="30aa0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="30aa0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="30aa0-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30aa0-141">roleScopeTagIds</span></span>|<span data-ttu-id="30aa0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="30aa0-142">String collection</span></span>|<span data-ttu-id="30aa0-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="30aa0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="30aa0-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="30aa0-145">supportsScopeTags</span></span>|<span data-ttu-id="30aa0-146">Логический</span><span class="sxs-lookup"><span data-stu-id="30aa0-146">Boolean</span></span>|<span data-ttu-id="30aa0-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="30aa0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="30aa0-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="30aa0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="30aa0-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="30aa0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="30aa0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30aa0-150">This property is read-only.</span></span> <span data-ttu-id="30aa0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30aa0-152">createdDateTime</span></span>|<span data-ttu-id="30aa0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30aa0-153">DateTimeOffset</span></span>|<span data-ttu-id="30aa0-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="30aa0-154">DateTime the object was created.</span></span> <span data-ttu-id="30aa0-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-156">описание</span><span class="sxs-lookup"><span data-stu-id="30aa0-156">description</span></span>|<span data-ttu-id="30aa0-157">String</span><span class="sxs-lookup"><span data-stu-id="30aa0-157">String</span></span>|<span data-ttu-id="30aa0-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="30aa0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="30aa0-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="30aa0-160">displayName</span></span>|<span data-ttu-id="30aa0-161">String</span><span class="sxs-lookup"><span data-stu-id="30aa0-161">String</span></span>|<span data-ttu-id="30aa0-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="30aa0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="30aa0-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30aa0-164">version</span><span class="sxs-lookup"><span data-stu-id="30aa0-164">version</span></span>|<span data-ttu-id="30aa0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="30aa0-165">Int32</span></span>|<span data-ttu-id="30aa0-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="30aa0-166">Version of the device configuration.</span></span> <span data-ttu-id="30aa0-167">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30aa0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="30aa0-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="30aa0-168">Response</span></span>
<span data-ttu-id="30aa0-169">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30aa0-169">If successful, this method returns a `200 OK` response code and an updated [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30aa0-170">Пример</span><span class="sxs-lookup"><span data-stu-id="30aa0-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="30aa0-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="30aa0-171">Request</span></span>
<span data-ttu-id="30aa0-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30aa0-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 255

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="30aa0-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="30aa0-173">Response</span></span>
<span data-ttu-id="30aa0-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="30aa0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```





