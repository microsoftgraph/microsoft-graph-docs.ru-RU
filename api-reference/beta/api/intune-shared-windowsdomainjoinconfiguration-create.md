---
title: Создание Виндовсдомаинжоинконфигуратион
description: Создание нового объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d98dd05c206f63077e481d0aad8b01c33f4776a6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939390"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="a048b-103">Создание Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a048b-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="a048b-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a048b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a048b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a048b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a048b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a048b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a048b-107">Создание нового объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a048b-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a048b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a048b-108">Prerequisites</span></span>
<span data-ttu-id="a048b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a048b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a048b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a048b-111">Permission type</span></span>|<span data-ttu-id="a048b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a048b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a048b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a048b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a048b-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a048b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a048b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a048b-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="a048b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a048b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a048b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a048b-117">Not supported.</span></span>|
|<span data-ttu-id="a048b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a048b-118">Application</span></span>||
| <span data-ttu-id="a048b-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a048b-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a048b-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a048b-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a048b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a048b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a048b-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a048b-122">Request headers</span></span>

|<span data-ttu-id="a048b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a048b-123">Header</span></span>|<span data-ttu-id="a048b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a048b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a048b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a048b-125">Authorization</span></span>|<span data-ttu-id="a048b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a048b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a048b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a048b-127">Accept</span></span>|<span data-ttu-id="a048b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a048b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a048b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a048b-129">Request body</span></span>

<span data-ttu-id="a048b-130">В тексте запроса добавьте представление объекта Виндовсдомаинжоинконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a048b-130">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="a048b-131">В следующей таблице приведены свойства, необходимые при создании Виндовсдомаинжоинконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="a048b-131">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="a048b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a048b-132">Property</span></span>|<span data-ttu-id="a048b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a048b-133">Type</span></span>|<span data-ttu-id="a048b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a048b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a048b-135">id</span><span class="sxs-lookup"><span data-stu-id="a048b-135">id</span></span>|<span data-ttu-id="a048b-136">String</span><span class="sxs-lookup"><span data-stu-id="a048b-136">String</span></span>|<span data-ttu-id="a048b-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a048b-137">Key of the entity.</span></span> <span data-ttu-id="a048b-138">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-138">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-139">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a048b-139">**Device configuration**</span></span>|
|<span data-ttu-id="a048b-140">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="a048b-140">activeDirectoryDomainName</span></span>|<span data-ttu-id="a048b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a048b-141">String</span></span>|<span data-ttu-id="a048b-142">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="a048b-142">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="a048b-143">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="a048b-143">computerNameStaticPrefix</span></span>|<span data-ttu-id="a048b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="a048b-144">String</span></span>|<span data-ttu-id="a048b-145">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="a048b-145">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="a048b-146">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="a048b-146">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="a048b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a048b-147">Int32</span></span>|<span data-ttu-id="a048b-148">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="a048b-148">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="a048b-149">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="a048b-149">Valid values 3 to 14</span></span>|
|<span data-ttu-id="a048b-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a048b-150">createdDateTime</span></span>|<span data-ttu-id="a048b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a048b-151">DateTimeOffset</span></span>|<span data-ttu-id="a048b-152">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a048b-152">DateTime the object was created.</span></span> <span data-ttu-id="a048b-153">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-154">description</span><span class="sxs-lookup"><span data-stu-id="a048b-154">description</span></span>|<span data-ttu-id="a048b-155">String</span><span class="sxs-lookup"><span data-stu-id="a048b-155">String</span></span>|<span data-ttu-id="a048b-156">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a048b-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a048b-157">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-158">displayName</span><span class="sxs-lookup"><span data-stu-id="a048b-158">displayName</span></span>|<span data-ttu-id="a048b-159">Строка</span><span class="sxs-lookup"><span data-stu-id="a048b-159">String</span></span>|<span data-ttu-id="a048b-160">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a048b-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a048b-161">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a048b-162">lastModifiedDateTime</span></span>|<span data-ttu-id="a048b-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a048b-163">DateTimeOffset</span></span>|<span data-ttu-id="a048b-164">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a048b-164">DateTime the object was last modified.</span></span> <span data-ttu-id="a048b-165">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-166">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="a048b-166">organizationalUnit</span></span>|<span data-ttu-id="a048b-167">Строка</span><span class="sxs-lookup"><span data-stu-id="a048b-167">String</span></span>|<span data-ttu-id="a048b-168">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="a048b-168">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="a048b-169">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="a048b-169">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="a048b-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a048b-170">roleScopeTagIds</span></span>|<span data-ttu-id="a048b-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a048b-171">String collection</span></span>|<span data-ttu-id="a048b-172">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a048b-172">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a048b-173">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-173">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-174">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a048b-174">supportsScopeTags</span></span>|<span data-ttu-id="a048b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a048b-175">Boolean</span></span>|<span data-ttu-id="a048b-176">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a048b-176">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a048b-177">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a048b-177">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a048b-178">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a048b-178">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a048b-179">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a048b-179">This property is read-only.</span></span> <span data-ttu-id="a048b-180">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a048b-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a048b-181">version</span><span class="sxs-lookup"><span data-stu-id="a048b-181">version</span></span>|<span data-ttu-id="a048b-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a048b-182">Int32</span></span>|<span data-ttu-id="a048b-183">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a048b-183">Version of the device configuration.</span></span> <span data-ttu-id="a048b-184">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a048b-184">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a048b-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="a048b-185">Response</span></span>

<span data-ttu-id="a048b-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a048b-186">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a048b-187">Пример</span><span class="sxs-lookup"><span data-stu-id="a048b-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="a048b-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="a048b-188">Request</span></span>

<span data-ttu-id="a048b-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a048b-189">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="a048b-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="a048b-190">Response</span></span>

<span data-ttu-id="a048b-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a048b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











