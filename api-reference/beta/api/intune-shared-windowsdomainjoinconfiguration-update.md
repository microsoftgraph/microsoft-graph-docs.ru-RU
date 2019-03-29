---
title: Обновление Виндовсдомаинжоинконфигуратион
description: Обновление свойств объекта Виндовсдомаинжоинконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66314179f65748abca432dcf4f41bab3c16ebd32
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969640"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="5f7be-103">Обновление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5f7be-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="5f7be-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f7be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f7be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f7be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f7be-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f7be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f7be-107">Обновление свойств объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5f7be-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f7be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f7be-108">Prerequisites</span></span>
<span data-ttu-id="5f7be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f7be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f7be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f7be-111">Permission type</span></span>|<span data-ttu-id="5f7be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f7be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f7be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f7be-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5f7be-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="5f7be-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5f7be-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f7be-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5f7be-116">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="5f7be-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5f7be-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f7be-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f7be-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f7be-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f7be-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f7be-119">Not supported.</span></span>|
|<span data-ttu-id="5f7be-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f7be-120">Application</span></span>|<span data-ttu-id="5f7be-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f7be-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f7be-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f7be-122">HTTP Request</span></span>

<span data-ttu-id="5f7be-123">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="5f7be-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="5f7be-124">**Регистрации**</span><span class="sxs-lookup"><span data-stu-id="5f7be-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="5f7be-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f7be-125">Request headers</span></span>
|<span data-ttu-id="5f7be-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f7be-126">Header</span></span>|<span data-ttu-id="5f7be-127">Значение</span><span class="sxs-lookup"><span data-stu-id="5f7be-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f7be-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f7be-128">Authorization</span></span>|<span data-ttu-id="5f7be-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f7be-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f7be-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5f7be-130">Accept</span></span>|<span data-ttu-id="5f7be-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5f7be-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f7be-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f7be-132">Request body</span></span>
<span data-ttu-id="5f7be-133">В тексте запроса добавьте представление объекта [Виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f7be-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="5f7be-134">В следующей таблице приведены свойства, необходимые при создании [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="5f7be-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f7be-135">Property</span></span>|<span data-ttu-id="5f7be-136">Тип</span><span class="sxs-lookup"><span data-stu-id="5f7be-136">Type</span></span>|<span data-ttu-id="5f7be-137">Описание</span><span class="sxs-lookup"><span data-stu-id="5f7be-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f7be-138">id</span><span class="sxs-lookup"><span data-stu-id="5f7be-138">id</span></span>|<span data-ttu-id="5f7be-139">Строка</span><span class="sxs-lookup"><span data-stu-id="5f7be-139">String</span></span>|<span data-ttu-id="5f7be-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5f7be-140">Key of the entity.</span></span> <span data-ttu-id="5f7be-141">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-142">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="5f7be-142">**Device configuration**</span></span>|
|<span data-ttu-id="5f7be-143">Активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="5f7be-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="5f7be-144">String</span><span class="sxs-lookup"><span data-stu-id="5f7be-144">String</span></span>|<span data-ttu-id="5f7be-145">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="5f7be-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="5f7be-146">Компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="5f7be-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="5f7be-147">String</span><span class="sxs-lookup"><span data-stu-id="5f7be-147">String</span></span>|<span data-ttu-id="5f7be-148">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="5f7be-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="5f7be-149">Компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="5f7be-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="5f7be-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5f7be-150">Int32</span></span>|<span data-ttu-id="5f7be-151">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="5f7be-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="5f7be-152">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="5f7be-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="5f7be-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f7be-153">createdDateTime</span></span>|<span data-ttu-id="5f7be-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f7be-154">DateTimeOffset</span></span>|<span data-ttu-id="5f7be-155">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5f7be-155">DateTime the object was created.</span></span> <span data-ttu-id="5f7be-156">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-157">description</span><span class="sxs-lookup"><span data-stu-id="5f7be-157">description</span></span>|<span data-ttu-id="5f7be-158">String</span><span class="sxs-lookup"><span data-stu-id="5f7be-158">String</span></span>|<span data-ttu-id="5f7be-159">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f7be-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f7be-160">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-161">displayName</span><span class="sxs-lookup"><span data-stu-id="5f7be-161">displayName</span></span>|<span data-ttu-id="5f7be-162">String</span><span class="sxs-lookup"><span data-stu-id="5f7be-162">String</span></span>|<span data-ttu-id="5f7be-163">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f7be-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f7be-164">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f7be-165">lastModifiedDateTime</span></span>|<span data-ttu-id="5f7be-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f7be-166">DateTimeOffset</span></span>|<span data-ttu-id="5f7be-167">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5f7be-167">DateTime the object was last modified.</span></span> <span data-ttu-id="5f7be-168">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="5f7be-169">organizationalUnit</span></span>|<span data-ttu-id="5f7be-170">String</span><span class="sxs-lookup"><span data-stu-id="5f7be-170">String</span></span>|<span data-ttu-id="5f7be-171">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="5f7be-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="5f7be-172">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="5f7be-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="5f7be-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5f7be-173">roleScopeTagIds</span></span>|<span data-ttu-id="5f7be-174">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5f7be-174">String collection</span></span>|<span data-ttu-id="5f7be-175">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5f7be-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5f7be-176">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-177">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5f7be-177">supportsScopeTags</span></span>|<span data-ttu-id="5f7be-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f7be-178">Boolean</span></span>|<span data-ttu-id="5f7be-179">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5f7be-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5f7be-180">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5f7be-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5f7be-181">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5f7be-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5f7be-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f7be-182">This property is read-only.</span></span> <span data-ttu-id="5f7be-183">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f7be-184">version</span><span class="sxs-lookup"><span data-stu-id="5f7be-184">version</span></span>|<span data-ttu-id="5f7be-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5f7be-185">Int32</span></span>|<span data-ttu-id="5f7be-186">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f7be-186">Version of the device configuration.</span></span> <span data-ttu-id="5f7be-187">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f7be-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="5f7be-188">Note: поддержка свойств текста запроса зависит от контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="5f7be-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="5f7be-189">Не все свойства подходят для всех рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="5f7be-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="5f7be-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f7be-190">Response</span></span>
<span data-ttu-id="5f7be-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f7be-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f7be-192">Пример</span><span class="sxs-lookup"><span data-stu-id="5f7be-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f7be-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f7be-193">Request</span></span>
<span data-ttu-id="5f7be-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f7be-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f7be-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f7be-195">Response</span></span>
<span data-ttu-id="5f7be-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f7be-196">Here is an example of the response.</span></span> <span data-ttu-id="5f7be-197">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5f7be-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5f7be-198">Свойства, возвращаемые фактическими вызовами, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="5f7be-198">Properties returned by actual calls vary according to the context.</span></span>
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



