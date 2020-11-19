---
title: Обновление Виндовсдомаинжоинконфигуратион
description: Обновление свойств объекта Виндовсдомаинжоинконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d75acbf1be6bad1f5397378170e6eeb0d7b81c4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257102"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="77a65-103">Обновление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="77a65-103">Update windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="77a65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77a65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77a65-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77a65-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77a65-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a65-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77a65-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77a65-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77a65-108">Обновление свойств объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="77a65-108">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77a65-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77a65-109">Prerequisites</span></span>
<span data-ttu-id="77a65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77a65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a65-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77a65-112">Permission type</span></span>|<span data-ttu-id="77a65-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77a65-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77a65-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77a65-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="77a65-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="77a65-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="77a65-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a65-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="77a65-117">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="77a65-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="77a65-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a65-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77a65-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77a65-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77a65-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a65-120">Not supported.</span></span>|
|<span data-ttu-id="77a65-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="77a65-121">Application</span></span>||
| <span data-ttu-id="77a65-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="77a65-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="77a65-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a65-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="77a65-124">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="77a65-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="77a65-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a65-125">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77a65-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77a65-126">HTTP Request</span></span>

<span data-ttu-id="77a65-127">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="77a65-127">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="77a65-128">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="77a65-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="77a65-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77a65-129">Request headers</span></span>
|<span data-ttu-id="77a65-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77a65-130">Header</span></span>|<span data-ttu-id="77a65-131">Значение</span><span class="sxs-lookup"><span data-stu-id="77a65-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77a65-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77a65-132">Authorization</span></span>|<span data-ttu-id="77a65-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77a65-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77a65-134">Accept</span><span class="sxs-lookup"><span data-stu-id="77a65-134">Accept</span></span>|<span data-ttu-id="77a65-135">application/json</span><span class="sxs-lookup"><span data-stu-id="77a65-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77a65-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77a65-136">Request body</span></span>
<span data-ttu-id="77a65-137">В тексте запроса добавьте представление объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77a65-137">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="77a65-138">В следующей таблице приведены свойства, необходимые при создании [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-138">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="77a65-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="77a65-139">Property</span></span>|<span data-ttu-id="77a65-140">Тип</span><span class="sxs-lookup"><span data-stu-id="77a65-140">Type</span></span>|<span data-ttu-id="77a65-141">Описание</span><span class="sxs-lookup"><span data-stu-id="77a65-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77a65-142">id</span><span class="sxs-lookup"><span data-stu-id="77a65-142">id</span></span>|<span data-ttu-id="77a65-143">String</span><span class="sxs-lookup"><span data-stu-id="77a65-143">String</span></span>|<span data-ttu-id="77a65-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77a65-144">Key of the entity.</span></span> <span data-ttu-id="77a65-145">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-146">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="77a65-146">**Device configuration**</span></span>|
|<span data-ttu-id="77a65-147">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="77a65-147">activeDirectoryDomainName</span></span>|<span data-ttu-id="77a65-148">String</span><span class="sxs-lookup"><span data-stu-id="77a65-148">String</span></span>|<span data-ttu-id="77a65-149">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="77a65-149">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="77a65-150">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="77a65-150">computerNameStaticPrefix</span></span>|<span data-ttu-id="77a65-151">String</span><span class="sxs-lookup"><span data-stu-id="77a65-151">String</span></span>|<span data-ttu-id="77a65-152">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="77a65-152">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="77a65-153">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="77a65-153">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="77a65-154">Int32</span><span class="sxs-lookup"><span data-stu-id="77a65-154">Int32</span></span>|<span data-ttu-id="77a65-155">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="77a65-155">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="77a65-156">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="77a65-156">Valid values 3 to 14</span></span>|
|<span data-ttu-id="77a65-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77a65-157">createdDateTime</span></span>|<span data-ttu-id="77a65-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a65-158">DateTimeOffset</span></span>|<span data-ttu-id="77a65-159">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="77a65-159">DateTime the object was created.</span></span> <span data-ttu-id="77a65-160">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-161">description</span><span class="sxs-lookup"><span data-stu-id="77a65-161">description</span></span>|<span data-ttu-id="77a65-162">String</span><span class="sxs-lookup"><span data-stu-id="77a65-162">String</span></span>|<span data-ttu-id="77a65-163">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77a65-163">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77a65-164">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-165">displayName</span><span class="sxs-lookup"><span data-stu-id="77a65-165">displayName</span></span>|<span data-ttu-id="77a65-166">String</span><span class="sxs-lookup"><span data-stu-id="77a65-166">String</span></span>|<span data-ttu-id="77a65-167">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77a65-167">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77a65-168">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77a65-169">lastModifiedDateTime</span></span>|<span data-ttu-id="77a65-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a65-170">DateTimeOffset</span></span>|<span data-ttu-id="77a65-171">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="77a65-171">DateTime the object was last modified.</span></span> <span data-ttu-id="77a65-172">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-173">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="77a65-173">organizationalUnit</span></span>|<span data-ttu-id="77a65-174">String</span><span class="sxs-lookup"><span data-stu-id="77a65-174">String</span></span>|<span data-ttu-id="77a65-175">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="77a65-175">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="77a65-176">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="77a65-176">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="77a65-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77a65-177">roleScopeTagIds</span></span>|<span data-ttu-id="77a65-178">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="77a65-178">String collection</span></span>|<span data-ttu-id="77a65-179">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="77a65-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77a65-180">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-181">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="77a65-181">supportsScopeTags</span></span>|<span data-ttu-id="77a65-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="77a65-182">Boolean</span></span>|<span data-ttu-id="77a65-183">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="77a65-183">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77a65-184">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="77a65-184">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77a65-185">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="77a65-185">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77a65-186">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77a65-186">This property is read-only.</span></span> <span data-ttu-id="77a65-187">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-187">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77a65-188">version</span><span class="sxs-lookup"><span data-stu-id="77a65-188">version</span></span>|<span data-ttu-id="77a65-189">Int32</span><span class="sxs-lookup"><span data-stu-id="77a65-189">Int32</span></span>|<span data-ttu-id="77a65-190">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77a65-190">Version of the device configuration.</span></span> <span data-ttu-id="77a65-191">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77a65-191">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="77a65-192">Note: поддержка свойств текста запроса зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="77a65-192">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="77a65-193">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="77a65-193">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="77a65-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="77a65-194">Response</span></span>
<span data-ttu-id="77a65-195">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77a65-195">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77a65-196">Пример</span><span class="sxs-lookup"><span data-stu-id="77a65-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="77a65-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="77a65-197">Request</span></span>
<span data-ttu-id="77a65-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77a65-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77a65-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="77a65-199">Response</span></span>
<span data-ttu-id="77a65-200">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77a65-200">Here is an example of the response.</span></span> <span data-ttu-id="77a65-201">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="77a65-201">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="77a65-202">Свойства, возвращаемые фактическими вызовами, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="77a65-202">Properties returned by actual calls vary according to the context.</span></span>
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










