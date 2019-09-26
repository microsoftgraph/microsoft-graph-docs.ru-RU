---
title: Обновление Виндовсдомаинжоинконфигуратион
description: Обновление свойств объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5d6edfe045d0e2bb559d81451ff6ab1a2b540af
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195701"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="35b1e-103">Обновление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="35b1e-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="35b1e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35b1e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35b1e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35b1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35b1e-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35b1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35b1e-107">Обновление свойств объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="35b1e-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35b1e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35b1e-108">Prerequisites</span></span>
<span data-ttu-id="35b1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35b1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35b1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35b1e-111">Permission type</span></span>|<span data-ttu-id="35b1e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35b1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35b1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35b1e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="35b1e-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="35b1e-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="35b1e-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35b1e-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="35b1e-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="35b1e-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="35b1e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35b1e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="35b1e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35b1e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35b1e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35b1e-119">Not supported.</span></span>|
|<span data-ttu-id="35b1e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35b1e-120">Application</span></span>||
| <span data-ttu-id="35b1e-121">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="35b1e-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="35b1e-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35b1e-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="35b1e-123">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="35b1e-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="35b1e-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35b1e-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35b1e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35b1e-125">HTTP Request</span></span>

<span data-ttu-id="35b1e-126">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="35b1e-126">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="35b1e-127">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="35b1e-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="35b1e-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35b1e-128">Request headers</span></span>
|<span data-ttu-id="35b1e-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35b1e-129">Header</span></span>|<span data-ttu-id="35b1e-130">Значение</span><span class="sxs-lookup"><span data-stu-id="35b1e-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35b1e-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35b1e-131">Authorization</span></span>|<span data-ttu-id="35b1e-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35b1e-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35b1e-133">Accept</span><span class="sxs-lookup"><span data-stu-id="35b1e-133">Accept</span></span>|<span data-ttu-id="35b1e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="35b1e-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35b1e-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35b1e-135">Request body</span></span>
<span data-ttu-id="35b1e-136">В тексте запроса добавьте представление объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35b1e-136">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="35b1e-137">В следующей таблице приведены свойства, необходимые при создании [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-137">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="35b1e-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="35b1e-138">Property</span></span>|<span data-ttu-id="35b1e-139">Тип</span><span class="sxs-lookup"><span data-stu-id="35b1e-139">Type</span></span>|<span data-ttu-id="35b1e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="35b1e-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b1e-141">id</span><span class="sxs-lookup"><span data-stu-id="35b1e-141">id</span></span>|<span data-ttu-id="35b1e-142">String</span><span class="sxs-lookup"><span data-stu-id="35b1e-142">String</span></span>|<span data-ttu-id="35b1e-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35b1e-143">Key of the entity.</span></span> <span data-ttu-id="35b1e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-145">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="35b1e-145">**Device configuration**</span></span>|
|<span data-ttu-id="35b1e-146">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="35b1e-146">activeDirectoryDomainName</span></span>|<span data-ttu-id="35b1e-147">String.</span><span class="sxs-lookup"><span data-stu-id="35b1e-147">String</span></span>|<span data-ttu-id="35b1e-148">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="35b1e-148">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="35b1e-149">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="35b1e-149">computerNameStaticPrefix</span></span>|<span data-ttu-id="35b1e-150">String.</span><span class="sxs-lookup"><span data-stu-id="35b1e-150">String</span></span>|<span data-ttu-id="35b1e-151">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="35b1e-151">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="35b1e-152">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="35b1e-152">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="35b1e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="35b1e-153">Int32</span></span>|<span data-ttu-id="35b1e-154">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="35b1e-154">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="35b1e-155">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="35b1e-155">Valid values 3 to 14</span></span>|
|<span data-ttu-id="35b1e-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35b1e-156">createdDateTime</span></span>|<span data-ttu-id="35b1e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35b1e-157">DateTimeOffset</span></span>|<span data-ttu-id="35b1e-158">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="35b1e-158">DateTime the object was created.</span></span> <span data-ttu-id="35b1e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-160">description</span><span class="sxs-lookup"><span data-stu-id="35b1e-160">description</span></span>|<span data-ttu-id="35b1e-161">String</span><span class="sxs-lookup"><span data-stu-id="35b1e-161">String</span></span>|<span data-ttu-id="35b1e-162">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35b1e-162">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35b1e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-164">displayName</span><span class="sxs-lookup"><span data-stu-id="35b1e-164">displayName</span></span>|<span data-ttu-id="35b1e-165">Строка</span><span class="sxs-lookup"><span data-stu-id="35b1e-165">String</span></span>|<span data-ttu-id="35b1e-166">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35b1e-166">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35b1e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35b1e-168">lastModifiedDateTime</span></span>|<span data-ttu-id="35b1e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35b1e-169">DateTimeOffset</span></span>|<span data-ttu-id="35b1e-170">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="35b1e-170">DateTime the object was last modified.</span></span> <span data-ttu-id="35b1e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-172">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="35b1e-172">organizationalUnit</span></span>|<span data-ttu-id="35b1e-173">String.</span><span class="sxs-lookup"><span data-stu-id="35b1e-173">String</span></span>|<span data-ttu-id="35b1e-174">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="35b1e-174">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="35b1e-175">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="35b1e-175">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="35b1e-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35b1e-176">roleScopeTagIds</span></span>|<span data-ttu-id="35b1e-177">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="35b1e-177">String collection</span></span>|<span data-ttu-id="35b1e-178">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="35b1e-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35b1e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-180">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="35b1e-180">supportsScopeTags</span></span>|<span data-ttu-id="35b1e-181">Boolean.</span><span class="sxs-lookup"><span data-stu-id="35b1e-181">Boolean</span></span>|<span data-ttu-id="35b1e-182">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="35b1e-182">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35b1e-183">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="35b1e-183">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35b1e-184">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="35b1e-184">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35b1e-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35b1e-185">This property is read-only.</span></span> <span data-ttu-id="35b1e-186">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-186">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35b1e-187">version</span><span class="sxs-lookup"><span data-stu-id="35b1e-187">version</span></span>|<span data-ttu-id="35b1e-188">Int32</span><span class="sxs-lookup"><span data-stu-id="35b1e-188">Int32</span></span>|<span data-ttu-id="35b1e-189">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35b1e-189">Version of the device configuration.</span></span> <span data-ttu-id="35b1e-190">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35b1e-190">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="35b1e-191">Note: поддержка свойств текста запроса зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="35b1e-191">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="35b1e-192">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="35b1e-192">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="35b1e-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="35b1e-193">Response</span></span>
<span data-ttu-id="35b1e-194">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35b1e-194">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35b1e-195">Пример</span><span class="sxs-lookup"><span data-stu-id="35b1e-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="35b1e-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="35b1e-196">Request</span></span>
<span data-ttu-id="35b1e-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35b1e-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35b1e-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="35b1e-198">Response</span></span>
<span data-ttu-id="35b1e-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35b1e-199">Here is an example of the response.</span></span> <span data-ttu-id="35b1e-200">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="35b1e-200">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="35b1e-201">Свойства, возвращаемые фактическими вызовами, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="35b1e-201">Properties returned by actual calls vary according to the context.</span></span>
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







