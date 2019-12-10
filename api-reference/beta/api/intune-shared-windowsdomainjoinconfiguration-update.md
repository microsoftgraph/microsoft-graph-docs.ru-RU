---
title: Обновление Виндовсдомаинжоинконфигуратион
description: Обновление свойств объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cadf31d0d7ada9b8e94ea17f326e102d8404c00e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939348"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="b6f36-103">Обновление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b6f36-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="b6f36-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6f36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6f36-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6f36-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6f36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f36-107">Обновление свойств объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b6f36-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6f36-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6f36-108">Prerequisites</span></span>
<span data-ttu-id="b6f36-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6f36-111">Permission type</span></span>|<span data-ttu-id="b6f36-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6f36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6f36-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6f36-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="b6f36-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6f36-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f36-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="b6f36-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="b6f36-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b6f36-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f36-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6f36-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6f36-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f36-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f36-119">Not supported.</span></span>|
|<span data-ttu-id="b6f36-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6f36-120">Application</span></span>||
| <span data-ttu-id="b6f36-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="b6f36-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6f36-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f36-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="b6f36-123">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="b6f36-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b6f36-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f36-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f36-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6f36-125">HTTP Request</span></span>

<span data-ttu-id="b6f36-126">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="b6f36-126">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="b6f36-127">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="b6f36-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="b6f36-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6f36-128">Request headers</span></span>
|<span data-ttu-id="b6f36-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6f36-129">Header</span></span>|<span data-ttu-id="b6f36-130">Значение</span><span class="sxs-lookup"><span data-stu-id="b6f36-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f36-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6f36-131">Authorization</span></span>|<span data-ttu-id="b6f36-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6f36-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f36-133">Accept</span><span class="sxs-lookup"><span data-stu-id="b6f36-133">Accept</span></span>|<span data-ttu-id="b6f36-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f36-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f36-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6f36-135">Request body</span></span>
<span data-ttu-id="b6f36-136">В тексте запроса добавьте представление объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6f36-136">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="b6f36-137">В следующей таблице приведены свойства, необходимые при создании [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-137">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="b6f36-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6f36-138">Property</span></span>|<span data-ttu-id="b6f36-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b6f36-139">Type</span></span>|<span data-ttu-id="b6f36-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b6f36-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6f36-141">id</span><span class="sxs-lookup"><span data-stu-id="b6f36-141">id</span></span>|<span data-ttu-id="b6f36-142">String</span><span class="sxs-lookup"><span data-stu-id="b6f36-142">String</span></span>|<span data-ttu-id="b6f36-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6f36-143">Key of the entity.</span></span> <span data-ttu-id="b6f36-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-145">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="b6f36-145">**Device configuration**</span></span>|
|<span data-ttu-id="b6f36-146">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="b6f36-146">activeDirectoryDomainName</span></span>|<span data-ttu-id="b6f36-147">Строка</span><span class="sxs-lookup"><span data-stu-id="b6f36-147">String</span></span>|<span data-ttu-id="b6f36-148">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="b6f36-148">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="b6f36-149">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="b6f36-149">computerNameStaticPrefix</span></span>|<span data-ttu-id="b6f36-150">Строка</span><span class="sxs-lookup"><span data-stu-id="b6f36-150">String</span></span>|<span data-ttu-id="b6f36-151">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="b6f36-151">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="b6f36-152">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="b6f36-152">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="b6f36-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b6f36-153">Int32</span></span>|<span data-ttu-id="b6f36-154">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="b6f36-154">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="b6f36-155">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="b6f36-155">Valid values 3 to 14</span></span>|
|<span data-ttu-id="b6f36-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6f36-156">createdDateTime</span></span>|<span data-ttu-id="b6f36-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6f36-157">DateTimeOffset</span></span>|<span data-ttu-id="b6f36-158">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b6f36-158">DateTime the object was created.</span></span> <span data-ttu-id="b6f36-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-160">description</span><span class="sxs-lookup"><span data-stu-id="b6f36-160">description</span></span>|<span data-ttu-id="b6f36-161">String</span><span class="sxs-lookup"><span data-stu-id="b6f36-161">String</span></span>|<span data-ttu-id="b6f36-162">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6f36-162">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6f36-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-164">displayName</span><span class="sxs-lookup"><span data-stu-id="b6f36-164">displayName</span></span>|<span data-ttu-id="b6f36-165">Строка</span><span class="sxs-lookup"><span data-stu-id="b6f36-165">String</span></span>|<span data-ttu-id="b6f36-166">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6f36-166">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6f36-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6f36-168">lastModifiedDateTime</span></span>|<span data-ttu-id="b6f36-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6f36-169">DateTimeOffset</span></span>|<span data-ttu-id="b6f36-170">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b6f36-170">DateTime the object was last modified.</span></span> <span data-ttu-id="b6f36-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-172">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="b6f36-172">organizationalUnit</span></span>|<span data-ttu-id="b6f36-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b6f36-173">String</span></span>|<span data-ttu-id="b6f36-174">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="b6f36-174">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="b6f36-175">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="b6f36-175">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="b6f36-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6f36-176">roleScopeTagIds</span></span>|<span data-ttu-id="b6f36-177">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b6f36-177">String collection</span></span>|<span data-ttu-id="b6f36-178">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b6f36-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6f36-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-180">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b6f36-180">supportsScopeTags</span></span>|<span data-ttu-id="b6f36-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6f36-181">Boolean</span></span>|<span data-ttu-id="b6f36-182">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b6f36-182">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b6f36-183">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b6f36-183">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b6f36-184">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b6f36-184">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b6f36-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6f36-185">This property is read-only.</span></span> <span data-ttu-id="b6f36-186">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-186">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6f36-187">version</span><span class="sxs-lookup"><span data-stu-id="b6f36-187">version</span></span>|<span data-ttu-id="b6f36-188">Int32</span><span class="sxs-lookup"><span data-stu-id="b6f36-188">Int32</span></span>|<span data-ttu-id="b6f36-189">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6f36-189">Version of the device configuration.</span></span> <span data-ttu-id="b6f36-190">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6f36-190">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="b6f36-191">Note: поддержка свойств текста запроса зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="b6f36-191">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="b6f36-192">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="b6f36-192">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="b6f36-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6f36-193">Response</span></span>
<span data-ttu-id="b6f36-194">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6f36-194">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f36-195">Пример</span><span class="sxs-lookup"><span data-stu-id="b6f36-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6f36-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6f36-196">Request</span></span>
<span data-ttu-id="b6f36-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6f36-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6f36-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6f36-198">Response</span></span>
<span data-ttu-id="b6f36-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6f36-199">Here is an example of the response.</span></span> <span data-ttu-id="b6f36-200">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b6f36-200">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b6f36-201">Свойства, возвращаемые фактическими вызовами, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="b6f36-201">Properties returned by actual calls vary according to the context.</span></span>
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











