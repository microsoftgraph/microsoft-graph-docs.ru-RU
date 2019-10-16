---
title: Обновление Виндовсдомаинжоинконфигуратион
description: Обновление свойств объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea6a898e7f508b31e2e55c8fd1a42b415bad9add
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537841"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="ae95a-103">Обновление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ae95a-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="ae95a-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae95a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae95a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae95a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae95a-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae95a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae95a-107">Обновление свойств объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ae95a-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae95a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ae95a-108">Prerequisites</span></span>
<span data-ttu-id="ae95a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae95a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae95a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae95a-111">Permission type</span></span>|<span data-ttu-id="ae95a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae95a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae95a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae95a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ae95a-114">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="ae95a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ae95a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae95a-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ae95a-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="ae95a-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ae95a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae95a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae95a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae95a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae95a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae95a-119">Not supported.</span></span>|
|<span data-ttu-id="ae95a-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae95a-120">Application</span></span>||
| <span data-ttu-id="ae95a-121">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="ae95a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ae95a-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae95a-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ae95a-123">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="ae95a-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ae95a-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae95a-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae95a-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae95a-125">HTTP Request</span></span>

<span data-ttu-id="ae95a-126">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="ae95a-126">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="ae95a-127">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="ae95a-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="ae95a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae95a-128">Request headers</span></span>
|<span data-ttu-id="ae95a-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae95a-129">Header</span></span>|<span data-ttu-id="ae95a-130">Значение</span><span class="sxs-lookup"><span data-stu-id="ae95a-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae95a-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae95a-131">Authorization</span></span>|<span data-ttu-id="ae95a-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae95a-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae95a-133">Accept</span><span class="sxs-lookup"><span data-stu-id="ae95a-133">Accept</span></span>|<span data-ttu-id="ae95a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ae95a-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae95a-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae95a-135">Request body</span></span>
<span data-ttu-id="ae95a-136">В тексте запроса добавьте представление объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae95a-136">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="ae95a-137">В следующей таблице приведены свойства, необходимые при создании [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-137">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="ae95a-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae95a-138">Property</span></span>|<span data-ttu-id="ae95a-139">Тип</span><span class="sxs-lookup"><span data-stu-id="ae95a-139">Type</span></span>|<span data-ttu-id="ae95a-140">Описание</span><span class="sxs-lookup"><span data-stu-id="ae95a-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae95a-141">id</span><span class="sxs-lookup"><span data-stu-id="ae95a-141">id</span></span>|<span data-ttu-id="ae95a-142">String</span><span class="sxs-lookup"><span data-stu-id="ae95a-142">String</span></span>|<span data-ttu-id="ae95a-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae95a-143">Key of the entity.</span></span> <span data-ttu-id="ae95a-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-145">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="ae95a-145">**Device configuration**</span></span>|
|<span data-ttu-id="ae95a-146">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="ae95a-146">activeDirectoryDomainName</span></span>|<span data-ttu-id="ae95a-147">String</span><span class="sxs-lookup"><span data-stu-id="ae95a-147">String</span></span>|<span data-ttu-id="ae95a-148">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="ae95a-148">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="ae95a-149">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="ae95a-149">computerNameStaticPrefix</span></span>|<span data-ttu-id="ae95a-150">String</span><span class="sxs-lookup"><span data-stu-id="ae95a-150">String</span></span>|<span data-ttu-id="ae95a-151">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="ae95a-151">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="ae95a-152">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="ae95a-152">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="ae95a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ae95a-153">Int32</span></span>|<span data-ttu-id="ae95a-154">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="ae95a-154">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="ae95a-155">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="ae95a-155">Valid values 3 to 14</span></span>|
|<span data-ttu-id="ae95a-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae95a-156">createdDateTime</span></span>|<span data-ttu-id="ae95a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae95a-157">DateTimeOffset</span></span>|<span data-ttu-id="ae95a-158">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ae95a-158">DateTime the object was created.</span></span> <span data-ttu-id="ae95a-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-160">description</span><span class="sxs-lookup"><span data-stu-id="ae95a-160">description</span></span>|<span data-ttu-id="ae95a-161">String</span><span class="sxs-lookup"><span data-stu-id="ae95a-161">String</span></span>|<span data-ttu-id="ae95a-162">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae95a-162">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae95a-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-164">displayName</span><span class="sxs-lookup"><span data-stu-id="ae95a-164">displayName</span></span>|<span data-ttu-id="ae95a-165">Строка</span><span class="sxs-lookup"><span data-stu-id="ae95a-165">String</span></span>|<span data-ttu-id="ae95a-166">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae95a-166">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae95a-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae95a-168">lastModifiedDateTime</span></span>|<span data-ttu-id="ae95a-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae95a-169">DateTimeOffset</span></span>|<span data-ttu-id="ae95a-170">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ae95a-170">DateTime the object was last modified.</span></span> <span data-ttu-id="ae95a-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-172">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="ae95a-172">organizationalUnit</span></span>|<span data-ttu-id="ae95a-173">String</span><span class="sxs-lookup"><span data-stu-id="ae95a-173">String</span></span>|<span data-ttu-id="ae95a-174">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="ae95a-174">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="ae95a-175">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="ae95a-175">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="ae95a-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae95a-176">roleScopeTagIds</span></span>|<span data-ttu-id="ae95a-177">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ae95a-177">String collection</span></span>|<span data-ttu-id="ae95a-178">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ae95a-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae95a-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-180">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ae95a-180">supportsScopeTags</span></span>|<span data-ttu-id="ae95a-181">Логический</span><span class="sxs-lookup"><span data-stu-id="ae95a-181">Boolean</span></span>|<span data-ttu-id="ae95a-182">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ae95a-182">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae95a-183">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ae95a-183">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae95a-184">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ae95a-184">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae95a-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae95a-185">This property is read-only.</span></span> <span data-ttu-id="ae95a-186">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-186">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae95a-187">version</span><span class="sxs-lookup"><span data-stu-id="ae95a-187">version</span></span>|<span data-ttu-id="ae95a-188">Int32</span><span class="sxs-lookup"><span data-stu-id="ae95a-188">Int32</span></span>|<span data-ttu-id="ae95a-189">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae95a-189">Version of the device configuration.</span></span> <span data-ttu-id="ae95a-190">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae95a-190">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="ae95a-191">Note: поддержка свойств текста запроса зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="ae95a-191">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="ae95a-192">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="ae95a-192">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="ae95a-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae95a-193">Response</span></span>
<span data-ttu-id="ae95a-194">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae95a-194">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae95a-195">Пример</span><span class="sxs-lookup"><span data-stu-id="ae95a-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae95a-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae95a-196">Request</span></span>
<span data-ttu-id="ae95a-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae95a-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae95a-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae95a-198">Response</span></span>
<span data-ttu-id="ae95a-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae95a-199">Here is an example of the response.</span></span> <span data-ttu-id="ae95a-200">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ae95a-200">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ae95a-201">Свойства, возвращаемые фактическими вызовами, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="ae95a-201">Properties returned by actual calls vary according to the context.</span></span>
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









