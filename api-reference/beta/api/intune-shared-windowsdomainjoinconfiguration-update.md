---
title: Обновление windowsDomainJoinConfiguration
description: Обновление свойства объекта windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66314179f65748abca432dcf4f41bab3c16ebd32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410856"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="f42c8-103">Обновление windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f42c8-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f42c8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f42c8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f42c8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f42c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f42c8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f42c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f42c8-107">Обновление свойства объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f42c8-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f42c8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f42c8-108">Prerequisites</span></span>
<span data-ttu-id="f42c8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f42c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f42c8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f42c8-111">Permission type</span></span>|<span data-ttu-id="f42c8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f42c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f42c8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f42c8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f42c8-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f42c8-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f42c8-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f42c8-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="f42c8-116">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="f42c8-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f42c8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f42c8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f42c8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f42c8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f42c8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f42c8-119">Not supported.</span></span>|
|<span data-ttu-id="f42c8-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f42c8-120">Application</span></span>|<span data-ttu-id="f42c8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f42c8-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f42c8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f42c8-122">HTTP Request</span></span>

<span data-ttu-id="f42c8-123">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f42c8-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="f42c8-124">**Регистрация**</span><span class="sxs-lookup"><span data-stu-id="f42c8-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="f42c8-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f42c8-125">Request headers</span></span>
|<span data-ttu-id="f42c8-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f42c8-126">Header</span></span>|<span data-ttu-id="f42c8-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f42c8-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f42c8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f42c8-128">Authorization</span></span>|<span data-ttu-id="f42c8-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f42c8-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f42c8-130">Accept</span><span class="sxs-lookup"><span data-stu-id="f42c8-130">Accept</span></span>|<span data-ttu-id="f42c8-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f42c8-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f42c8-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f42c8-132">Request body</span></span>
<span data-ttu-id="f42c8-133">В тексте запроса укажите представление JSON для объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f42c8-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="f42c8-134">В следующей таблице показаны свойства, которые необходимы для создания [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="f42c8-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="f42c8-135">Property</span></span>|<span data-ttu-id="f42c8-136">Тип</span><span class="sxs-lookup"><span data-stu-id="f42c8-136">Type</span></span>|<span data-ttu-id="f42c8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f42c8-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f42c8-138">id</span><span class="sxs-lookup"><span data-stu-id="f42c8-138">id</span></span>|<span data-ttu-id="f42c8-139">String</span><span class="sxs-lookup"><span data-stu-id="f42c8-139">String</span></span>|<span data-ttu-id="f42c8-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f42c8-140">Key of the entity.</span></span> <span data-ttu-id="f42c8-141">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-142">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f42c8-142">**Device configuration**</span></span>|
|<span data-ttu-id="f42c8-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="f42c8-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="f42c8-144">String</span><span class="sxs-lookup"><span data-stu-id="f42c8-144">String</span></span>|<span data-ttu-id="f42c8-145">Имя домена Active Directory для присоединения к.</span><span class="sxs-lookup"><span data-stu-id="f42c8-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="f42c8-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="f42c8-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="f42c8-147">String</span><span class="sxs-lookup"><span data-stu-id="f42c8-147">String</span></span>|<span data-ttu-id="f42c8-148">Фиксированный префикс для использования для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="f42c8-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="f42c8-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="f42c8-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="f42c8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f42c8-150">Int32</span></span>|<span data-ttu-id="f42c8-151">Динамически созданные символы, используемого в качестве суффикса имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="f42c8-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="f42c8-152">Допустимые значения 3 до 14</span><span class="sxs-lookup"><span data-stu-id="f42c8-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="f42c8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f42c8-153">createdDateTime</span></span>|<span data-ttu-id="f42c8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f42c8-154">DateTimeOffset</span></span>|<span data-ttu-id="f42c8-155">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f42c8-155">DateTime the object was created.</span></span> <span data-ttu-id="f42c8-156">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-157">description</span><span class="sxs-lookup"><span data-stu-id="f42c8-157">description</span></span>|<span data-ttu-id="f42c8-158">String</span><span class="sxs-lookup"><span data-stu-id="f42c8-158">String</span></span>|<span data-ttu-id="f42c8-159">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f42c8-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f42c8-160">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-161">displayName</span><span class="sxs-lookup"><span data-stu-id="f42c8-161">displayName</span></span>|<span data-ttu-id="f42c8-162">String</span><span class="sxs-lookup"><span data-stu-id="f42c8-162">String</span></span>|<span data-ttu-id="f42c8-163">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f42c8-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f42c8-164">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f42c8-165">lastModifiedDateTime</span></span>|<span data-ttu-id="f42c8-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f42c8-166">DateTimeOffset</span></span>|<span data-ttu-id="f42c8-167">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f42c8-167">DateTime the object was last modified.</span></span> <span data-ttu-id="f42c8-168">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="f42c8-169">organizationalUnit</span></span>|<span data-ttu-id="f42c8-170">String</span><span class="sxs-lookup"><span data-stu-id="f42c8-170">String</span></span>|<span data-ttu-id="f42c8-171">Подразделение (OU) которой будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="f42c8-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="f42c8-172">Если этот параметр имеет значение NULL, объект контейнера хорошо известных компьютера будет использоваться, опубликованной в домене.</span><span class="sxs-lookup"><span data-stu-id="f42c8-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="f42c8-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f42c8-173">roleScopeTagIds</span></span>|<span data-ttu-id="f42c8-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f42c8-174">String collection</span></span>|<span data-ttu-id="f42c8-175">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f42c8-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f42c8-176">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f42c8-177">supportsScopeTags</span></span>|<span data-ttu-id="f42c8-178">Логический</span><span class="sxs-lookup"><span data-stu-id="f42c8-178">Boolean</span></span>|<span data-ttu-id="f42c8-179">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f42c8-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f42c8-180">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f42c8-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f42c8-181">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f42c8-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f42c8-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f42c8-182">This property is read-only.</span></span> <span data-ttu-id="f42c8-183">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f42c8-184">version</span><span class="sxs-lookup"><span data-stu-id="f42c8-184">version</span></span>|<span data-ttu-id="f42c8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f42c8-185">Int32</span></span>|<span data-ttu-id="f42c8-186">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f42c8-186">Version of the device configuration.</span></span> <span data-ttu-id="f42c8-187">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f42c8-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="f42c8-188">Примечание: Поддержка свойства body запрос зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="f42c8-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="f42c8-189">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="f42c8-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="f42c8-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="f42c8-190">Response</span></span>
<span data-ttu-id="f42c8-191">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f42c8-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f42c8-192">Пример</span><span class="sxs-lookup"><span data-stu-id="f42c8-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="f42c8-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="f42c8-193">Request</span></span>
<span data-ttu-id="f42c8-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f42c8-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 344

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="f42c8-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="f42c8-195">Response</span></span>
<span data-ttu-id="f42c8-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f42c8-196">Here is an example of the response.</span></span> <span data-ttu-id="f42c8-197">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f42c8-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f42c8-198">Свойств, возвращаемых фактические вызовы различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="f42c8-198">Properties returned by actual calls vary according to the context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```



