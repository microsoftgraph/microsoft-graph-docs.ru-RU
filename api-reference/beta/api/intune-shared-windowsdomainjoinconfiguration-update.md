---
title: Обновление Виндовсдомаинжоинконфигуратион
description: Обновление свойств объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85a4361bc05a583efd0cf7287ca36deafe160d22
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350526"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="85720-103">Обновление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="85720-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="85720-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85720-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85720-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85720-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85720-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85720-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85720-107">Обновление свойств объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="85720-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85720-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85720-108">Prerequisites</span></span>
<span data-ttu-id="85720-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85720-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85720-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85720-111">Permission type</span></span>|<span data-ttu-id="85720-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85720-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85720-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85720-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="85720-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="85720-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="85720-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85720-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="85720-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="85720-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="85720-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85720-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85720-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85720-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85720-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85720-119">Not supported.</span></span>|
|<span data-ttu-id="85720-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85720-120">Application</span></span>|<span data-ttu-id="85720-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85720-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85720-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85720-122">HTTP Request</span></span>

<span data-ttu-id="85720-123">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="85720-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="85720-124">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="85720-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="85720-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85720-125">Request headers</span></span>
|<span data-ttu-id="85720-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85720-126">Header</span></span>|<span data-ttu-id="85720-127">Значение</span><span class="sxs-lookup"><span data-stu-id="85720-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85720-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85720-128">Authorization</span></span>|<span data-ttu-id="85720-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85720-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85720-130">Accept</span><span class="sxs-lookup"><span data-stu-id="85720-130">Accept</span></span>|<span data-ttu-id="85720-131">application/json</span><span class="sxs-lookup"><span data-stu-id="85720-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85720-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85720-132">Request body</span></span>
<span data-ttu-id="85720-133">В тексте запроса добавьте представление объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85720-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="85720-134">В следующей таблице приведены свойства, необходимые при создании [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="85720-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="85720-135">Property</span></span>|<span data-ttu-id="85720-136">Тип</span><span class="sxs-lookup"><span data-stu-id="85720-136">Type</span></span>|<span data-ttu-id="85720-137">Описание</span><span class="sxs-lookup"><span data-stu-id="85720-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85720-138">id</span><span class="sxs-lookup"><span data-stu-id="85720-138">id</span></span>|<span data-ttu-id="85720-139">String</span><span class="sxs-lookup"><span data-stu-id="85720-139">String</span></span>|<span data-ttu-id="85720-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85720-140">Key of the entity.</span></span> <span data-ttu-id="85720-141">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-142">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="85720-142">**Device configuration**</span></span>|
|<span data-ttu-id="85720-143">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="85720-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="85720-144">String</span><span class="sxs-lookup"><span data-stu-id="85720-144">String</span></span>|<span data-ttu-id="85720-145">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="85720-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="85720-146">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="85720-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="85720-147">String</span><span class="sxs-lookup"><span data-stu-id="85720-147">String</span></span>|<span data-ttu-id="85720-148">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="85720-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="85720-149">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="85720-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="85720-150">Int32</span><span class="sxs-lookup"><span data-stu-id="85720-150">Int32</span></span>|<span data-ttu-id="85720-151">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="85720-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="85720-152">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="85720-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="85720-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85720-153">createdDateTime</span></span>|<span data-ttu-id="85720-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85720-154">DateTimeOffset</span></span>|<span data-ttu-id="85720-155">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="85720-155">DateTime the object was created.</span></span> <span data-ttu-id="85720-156">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-157">description</span><span class="sxs-lookup"><span data-stu-id="85720-157">description</span></span>|<span data-ttu-id="85720-158">String</span><span class="sxs-lookup"><span data-stu-id="85720-158">String</span></span>|<span data-ttu-id="85720-159">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85720-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85720-160">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-161">displayName</span><span class="sxs-lookup"><span data-stu-id="85720-161">displayName</span></span>|<span data-ttu-id="85720-162">Строка</span><span class="sxs-lookup"><span data-stu-id="85720-162">String</span></span>|<span data-ttu-id="85720-163">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85720-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85720-164">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85720-165">lastModifiedDateTime</span></span>|<span data-ttu-id="85720-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85720-166">DateTimeOffset</span></span>|<span data-ttu-id="85720-167">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="85720-167">DateTime the object was last modified.</span></span> <span data-ttu-id="85720-168">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="85720-169">organizationalUnit</span></span>|<span data-ttu-id="85720-170">String</span><span class="sxs-lookup"><span data-stu-id="85720-170">String</span></span>|<span data-ttu-id="85720-171">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="85720-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="85720-172">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="85720-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="85720-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85720-173">roleScopeTagIds</span></span>|<span data-ttu-id="85720-174">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="85720-174">String collection</span></span>|<span data-ttu-id="85720-175">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="85720-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85720-176">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-177">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="85720-177">supportsScopeTags</span></span>|<span data-ttu-id="85720-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="85720-178">Boolean</span></span>|<span data-ttu-id="85720-179">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="85720-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85720-180">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="85720-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85720-181">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="85720-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85720-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85720-182">This property is read-only.</span></span> <span data-ttu-id="85720-183">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85720-184">version</span><span class="sxs-lookup"><span data-stu-id="85720-184">version</span></span>|<span data-ttu-id="85720-185">Int32</span><span class="sxs-lookup"><span data-stu-id="85720-185">Int32</span></span>|<span data-ttu-id="85720-186">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85720-186">Version of the device configuration.</span></span> <span data-ttu-id="85720-187">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85720-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="85720-188">Note: поддержка свойств текста запроса зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="85720-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="85720-189">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="85720-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="85720-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="85720-190">Response</span></span>
<span data-ttu-id="85720-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85720-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85720-192">Пример</span><span class="sxs-lookup"><span data-stu-id="85720-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="85720-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="85720-193">Request</span></span>
<span data-ttu-id="85720-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85720-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85720-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="85720-195">Response</span></span>
<span data-ttu-id="85720-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85720-196">Here is an example of the response.</span></span> <span data-ttu-id="85720-197">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="85720-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="85720-198">Свойства, возвращаемые фактическими вызовами, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="85720-198">Properties returned by actual calls vary according to the context.</span></span>
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






