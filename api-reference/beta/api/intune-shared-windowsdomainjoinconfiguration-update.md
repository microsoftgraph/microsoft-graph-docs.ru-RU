---
title: Обновление windowsDomainJoinConfiguration
description: Обновление свойства объекта windowsDomainJoinConfiguration.
author: tfitzmac
ms.openlocfilehash: 20d096d4ddbdb8abdbc1cb88679c480d3a29f37e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352082"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="d481a-103">Обновление windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="d481a-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="d481a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d481a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d481a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d481a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d481a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d481a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d481a-107">Обновление свойства объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d481a-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d481a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d481a-108">Prerequisites</span></span>
<span data-ttu-id="d481a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d481a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d481a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d481a-111">Permission type</span></span>|<span data-ttu-id="d481a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d481a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d481a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d481a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d481a-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="d481a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d481a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d481a-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d481a-116">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d481a-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d481a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d481a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d481a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d481a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d481a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d481a-119">Not supported.</span></span>|
|<span data-ttu-id="d481a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d481a-120">Application</span></span>|<span data-ttu-id="d481a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d481a-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d481a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d481a-122">HTTP Request</span></span>

<span data-ttu-id="d481a-123">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="d481a-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="d481a-124">**Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d481a-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="d481a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d481a-125">Request headers</span></span>
|<span data-ttu-id="d481a-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d481a-126">Header</span></span>|<span data-ttu-id="d481a-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d481a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d481a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d481a-128">Authorization</span></span>|<span data-ttu-id="d481a-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d481a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d481a-130">Accept</span><span class="sxs-lookup"><span data-stu-id="d481a-130">Accept</span></span>|<span data-ttu-id="d481a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d481a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d481a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d481a-132">Request body</span></span>
<span data-ttu-id="d481a-133">В тексте запроса укажите представление JSON для объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d481a-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="d481a-134">В следующей таблице показаны свойства, которые необходимы для создания [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="d481a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="d481a-135">Property</span></span>|<span data-ttu-id="d481a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d481a-136">Type</span></span>|<span data-ttu-id="d481a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d481a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d481a-138">id</span><span class="sxs-lookup"><span data-stu-id="d481a-138">id</span></span>|<span data-ttu-id="d481a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d481a-139">String</span></span>|<span data-ttu-id="d481a-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d481a-140">Key of the entity.</span></span> <span data-ttu-id="d481a-141">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-142">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="d481a-142">**Device configuration**</span></span>|
|<span data-ttu-id="d481a-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="d481a-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="d481a-144">String.</span><span class="sxs-lookup"><span data-stu-id="d481a-144">String</span></span>|<span data-ttu-id="d481a-145">Имя домена Active Directory для присоединения к.</span><span class="sxs-lookup"><span data-stu-id="d481a-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="d481a-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="d481a-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="d481a-147">String.</span><span class="sxs-lookup"><span data-stu-id="d481a-147">String</span></span>|<span data-ttu-id="d481a-148">Фиксированный префикс для использования для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="d481a-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="d481a-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="d481a-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="d481a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d481a-150">Int32</span></span>|<span data-ttu-id="d481a-151">Динамически созданные символы, используемого в качестве суффикса имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="d481a-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="d481a-152">Допустимые значения 3 до 14</span><span class="sxs-lookup"><span data-stu-id="d481a-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="d481a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d481a-153">createdDateTime</span></span>|<span data-ttu-id="d481a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d481a-154">DateTimeOffset</span></span>|<span data-ttu-id="d481a-155">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d481a-155">DateTime the object was created.</span></span> <span data-ttu-id="d481a-156">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-157">описание</span><span class="sxs-lookup"><span data-stu-id="d481a-157">description</span></span>|<span data-ttu-id="d481a-158">Строка</span><span class="sxs-lookup"><span data-stu-id="d481a-158">String</span></span>|<span data-ttu-id="d481a-159">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d481a-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d481a-160">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-161">displayName</span><span class="sxs-lookup"><span data-stu-id="d481a-161">displayName</span></span>|<span data-ttu-id="d481a-162">Строка</span><span class="sxs-lookup"><span data-stu-id="d481a-162">String</span></span>|<span data-ttu-id="d481a-163">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d481a-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d481a-164">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d481a-165">lastModifiedDateTime</span></span>|<span data-ttu-id="d481a-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d481a-166">DateTimeOffset</span></span>|<span data-ttu-id="d481a-167">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d481a-167">DateTime the object was last modified.</span></span> <span data-ttu-id="d481a-168">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="d481a-169">organizationalUnit</span></span>|<span data-ttu-id="d481a-170">String.</span><span class="sxs-lookup"><span data-stu-id="d481a-170">String</span></span>|<span data-ttu-id="d481a-171">Подразделение (OU) которой будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="d481a-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="d481a-172">Если этот параметр имеет значение NULL, объект контейнера хорошо известных компьютера будет использоваться, опубликованной в домене.</span><span class="sxs-lookup"><span data-stu-id="d481a-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="d481a-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d481a-173">roleScopeTagIds</span></span>|<span data-ttu-id="d481a-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d481a-174">String collection</span></span>|<span data-ttu-id="d481a-175">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d481a-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d481a-176">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d481a-177">supportsScopeTags</span></span>|<span data-ttu-id="d481a-178">Boolean.</span><span class="sxs-lookup"><span data-stu-id="d481a-178">Boolean</span></span>|<span data-ttu-id="d481a-179">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="d481a-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d481a-180">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="d481a-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d481a-181">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d481a-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d481a-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d481a-182">This property is read-only.</span></span> <span data-ttu-id="d481a-183">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d481a-184">version</span><span class="sxs-lookup"><span data-stu-id="d481a-184">version</span></span>|<span data-ttu-id="d481a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d481a-185">Int32</span></span>|<span data-ttu-id="d481a-186">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d481a-186">Version of the device configuration.</span></span> <span data-ttu-id="d481a-187">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d481a-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="d481a-188">Примечание: Поддержка свойства body запрос зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="d481a-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="d481a-189">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="d481a-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="d481a-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="d481a-190">Response</span></span>
<span data-ttu-id="d481a-191">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d481a-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d481a-192">Пример</span><span class="sxs-lookup"><span data-stu-id="d481a-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="d481a-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="d481a-193">Request</span></span>
<span data-ttu-id="d481a-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d481a-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d481a-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="d481a-195">Response</span></span>
<span data-ttu-id="d481a-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d481a-196">Here is an example of the response.</span></span> <span data-ttu-id="d481a-197">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d481a-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d481a-198">Свойств, возвращаемых фактические вызовы различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="d481a-198">Properties returned by actual calls vary according to the context.</span></span>
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



