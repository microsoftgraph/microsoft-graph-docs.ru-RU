---
title: Создание Виндовсдомаинжоинконфигуратион
description: Создание нового объекта Виндовсдомаинжоинконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97d760b9e5dd34038a70cea14294fa4a27e55a3b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447359"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="795a5-103">Создание Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="795a5-103">Create windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="795a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="795a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="795a5-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="795a5-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="795a5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="795a5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="795a5-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="795a5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="795a5-108">Создание нового объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="795a5-108">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="795a5-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="795a5-109">Prerequisites</span></span>
<span data-ttu-id="795a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="795a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="795a5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="795a5-112">Permission type</span></span>|<span data-ttu-id="795a5-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="795a5-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="795a5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="795a5-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="795a5-115">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="795a5-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="795a5-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="795a5-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="795a5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="795a5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="795a5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="795a5-118">Not supported.</span></span>|
|<span data-ttu-id="795a5-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="795a5-119">Application</span></span>||
| <span data-ttu-id="795a5-120">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="795a5-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="795a5-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="795a5-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="795a5-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="795a5-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="795a5-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="795a5-123">Request headers</span></span>

|<span data-ttu-id="795a5-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="795a5-124">Header</span></span>|<span data-ttu-id="795a5-125">Значение</span><span class="sxs-lookup"><span data-stu-id="795a5-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="795a5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="795a5-126">Authorization</span></span>|<span data-ttu-id="795a5-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="795a5-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="795a5-128">Accept</span><span class="sxs-lookup"><span data-stu-id="795a5-128">Accept</span></span>|<span data-ttu-id="795a5-129">application/json</span><span class="sxs-lookup"><span data-stu-id="795a5-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="795a5-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="795a5-130">Request body</span></span>

<span data-ttu-id="795a5-131">В тексте запроса добавьте представление объекта Виндовсдомаинжоинконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="795a5-131">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="795a5-132">В следующей таблице приведены свойства, необходимые при создании Виндовсдомаинжоинконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="795a5-132">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="795a5-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="795a5-133">Property</span></span>|<span data-ttu-id="795a5-134">Тип</span><span class="sxs-lookup"><span data-stu-id="795a5-134">Type</span></span>|<span data-ttu-id="795a5-135">Описание</span><span class="sxs-lookup"><span data-stu-id="795a5-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="795a5-136">id</span><span class="sxs-lookup"><span data-stu-id="795a5-136">id</span></span>|<span data-ttu-id="795a5-137">String</span><span class="sxs-lookup"><span data-stu-id="795a5-137">String</span></span>|<span data-ttu-id="795a5-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="795a5-138">Key of the entity.</span></span> <span data-ttu-id="795a5-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-140">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="795a5-140">**Device configuration**</span></span>|
|<span data-ttu-id="795a5-141">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="795a5-141">activeDirectoryDomainName</span></span>|<span data-ttu-id="795a5-142">String</span><span class="sxs-lookup"><span data-stu-id="795a5-142">String</span></span>|<span data-ttu-id="795a5-143">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="795a5-143">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="795a5-144">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="795a5-144">computerNameStaticPrefix</span></span>|<span data-ttu-id="795a5-145">String</span><span class="sxs-lookup"><span data-stu-id="795a5-145">String</span></span>|<span data-ttu-id="795a5-146">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="795a5-146">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="795a5-147">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="795a5-147">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="795a5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="795a5-148">Int32</span></span>|<span data-ttu-id="795a5-149">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="795a5-149">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="795a5-150">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="795a5-150">Valid values 3 to 14</span></span>|
|<span data-ttu-id="795a5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="795a5-151">createdDateTime</span></span>|<span data-ttu-id="795a5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="795a5-152">DateTimeOffset</span></span>|<span data-ttu-id="795a5-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="795a5-153">DateTime the object was created.</span></span> <span data-ttu-id="795a5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-155">description</span><span class="sxs-lookup"><span data-stu-id="795a5-155">description</span></span>|<span data-ttu-id="795a5-156">String</span><span class="sxs-lookup"><span data-stu-id="795a5-156">String</span></span>|<span data-ttu-id="795a5-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="795a5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="795a5-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="795a5-159">displayName</span></span>|<span data-ttu-id="795a5-160">Строка</span><span class="sxs-lookup"><span data-stu-id="795a5-160">String</span></span>|<span data-ttu-id="795a5-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="795a5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="795a5-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="795a5-163">lastModifiedDateTime</span></span>|<span data-ttu-id="795a5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="795a5-164">DateTimeOffset</span></span>|<span data-ttu-id="795a5-165">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="795a5-165">DateTime the object was last modified.</span></span> <span data-ttu-id="795a5-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-167">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="795a5-167">organizationalUnit</span></span>|<span data-ttu-id="795a5-168">String</span><span class="sxs-lookup"><span data-stu-id="795a5-168">String</span></span>|<span data-ttu-id="795a5-169">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="795a5-169">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="795a5-170">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="795a5-170">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="795a5-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="795a5-171">roleScopeTagIds</span></span>|<span data-ttu-id="795a5-172">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="795a5-172">String collection</span></span>|<span data-ttu-id="795a5-173">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="795a5-173">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="795a5-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-175">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="795a5-175">supportsScopeTags</span></span>|<span data-ttu-id="795a5-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="795a5-176">Boolean</span></span>|<span data-ttu-id="795a5-177">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="795a5-177">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="795a5-178">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="795a5-178">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="795a5-179">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="795a5-179">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="795a5-180">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="795a5-180">This property is read-only.</span></span> <span data-ttu-id="795a5-181">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="795a5-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="795a5-182">version</span><span class="sxs-lookup"><span data-stu-id="795a5-182">version</span></span>|<span data-ttu-id="795a5-183">Int32</span><span class="sxs-lookup"><span data-stu-id="795a5-183">Int32</span></span>|<span data-ttu-id="795a5-184">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="795a5-184">Version of the device configuration.</span></span> <span data-ttu-id="795a5-185">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="795a5-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="795a5-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="795a5-186">Response</span></span>

<span data-ttu-id="795a5-187">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="795a5-187">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="795a5-188">Пример</span><span class="sxs-lookup"><span data-stu-id="795a5-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="795a5-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="795a5-189">Request</span></span>

<span data-ttu-id="795a5-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="795a5-190">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 559

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```

### <a name="response"></a><span data-ttu-id="795a5-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="795a5-191">Response</span></span>

<span data-ttu-id="795a5-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="795a5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```









