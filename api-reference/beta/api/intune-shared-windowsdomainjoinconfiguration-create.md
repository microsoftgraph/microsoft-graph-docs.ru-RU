---
title: Создание Виндовсдомаинжоинконфигуратион
description: Создание нового объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a39a5d91c77edc094f34ae6ff2c00d7e53c1ff57
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194322"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="cebdb-103">Создание Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cebdb-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="cebdb-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cebdb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cebdb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cebdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cebdb-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cebdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cebdb-107">Создание нового объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cebdb-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cebdb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cebdb-108">Prerequisites</span></span>
<span data-ttu-id="cebdb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cebdb-111">Permission type</span></span>|<span data-ttu-id="cebdb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cebdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cebdb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cebdb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cebdb-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="cebdb-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cebdb-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebdb-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="cebdb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cebdb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cebdb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cebdb-117">Not supported.</span></span>|
|<span data-ttu-id="cebdb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cebdb-118">Application</span></span>||
| <span data-ttu-id="cebdb-119">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="cebdb-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cebdb-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebdb-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cebdb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cebdb-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cebdb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cebdb-122">Request headers</span></span>

|<span data-ttu-id="cebdb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cebdb-123">Header</span></span>|<span data-ttu-id="cebdb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cebdb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cebdb-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cebdb-125">Authorization</span></span>|<span data-ttu-id="cebdb-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cebdb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cebdb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cebdb-127">Accept</span></span>|<span data-ttu-id="cebdb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cebdb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cebdb-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cebdb-129">Request body</span></span>

<span data-ttu-id="cebdb-130">В тексте запроса добавьте представление объекта Виндовсдомаинжоинконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cebdb-130">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="cebdb-131">В следующей таблице приведены свойства, необходимые при создании Виндовсдомаинжоинконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="cebdb-131">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="cebdb-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="cebdb-132">Property</span></span>|<span data-ttu-id="cebdb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="cebdb-133">Type</span></span>|<span data-ttu-id="cebdb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cebdb-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cebdb-135">id</span><span class="sxs-lookup"><span data-stu-id="cebdb-135">id</span></span>|<span data-ttu-id="cebdb-136">String</span><span class="sxs-lookup"><span data-stu-id="cebdb-136">String</span></span>|<span data-ttu-id="cebdb-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cebdb-137">Key of the entity.</span></span> <span data-ttu-id="cebdb-138">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-138">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-139">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="cebdb-139">**Device configuration**</span></span>|
|<span data-ttu-id="cebdb-140">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="cebdb-140">activeDirectoryDomainName</span></span>|<span data-ttu-id="cebdb-141">String.</span><span class="sxs-lookup"><span data-stu-id="cebdb-141">String</span></span>|<span data-ttu-id="cebdb-142">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="cebdb-142">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="cebdb-143">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="cebdb-143">computerNameStaticPrefix</span></span>|<span data-ttu-id="cebdb-144">String.</span><span class="sxs-lookup"><span data-stu-id="cebdb-144">String</span></span>|<span data-ttu-id="cebdb-145">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="cebdb-145">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="cebdb-146">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="cebdb-146">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="cebdb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cebdb-147">Int32</span></span>|<span data-ttu-id="cebdb-148">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="cebdb-148">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="cebdb-149">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="cebdb-149">Valid values 3 to 14</span></span>|
|<span data-ttu-id="cebdb-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cebdb-150">createdDateTime</span></span>|<span data-ttu-id="cebdb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cebdb-151">DateTimeOffset</span></span>|<span data-ttu-id="cebdb-152">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cebdb-152">DateTime the object was created.</span></span> <span data-ttu-id="cebdb-153">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-154">description</span><span class="sxs-lookup"><span data-stu-id="cebdb-154">description</span></span>|<span data-ttu-id="cebdb-155">String</span><span class="sxs-lookup"><span data-stu-id="cebdb-155">String</span></span>|<span data-ttu-id="cebdb-156">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cebdb-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cebdb-157">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-158">displayName</span><span class="sxs-lookup"><span data-stu-id="cebdb-158">displayName</span></span>|<span data-ttu-id="cebdb-159">Строка</span><span class="sxs-lookup"><span data-stu-id="cebdb-159">String</span></span>|<span data-ttu-id="cebdb-160">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cebdb-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cebdb-161">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cebdb-162">lastModifiedDateTime</span></span>|<span data-ttu-id="cebdb-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cebdb-163">DateTimeOffset</span></span>|<span data-ttu-id="cebdb-164">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cebdb-164">DateTime the object was last modified.</span></span> <span data-ttu-id="cebdb-165">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-166">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="cebdb-166">organizationalUnit</span></span>|<span data-ttu-id="cebdb-167">String.</span><span class="sxs-lookup"><span data-stu-id="cebdb-167">String</span></span>|<span data-ttu-id="cebdb-168">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="cebdb-168">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="cebdb-169">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="cebdb-169">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="cebdb-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cebdb-170">roleScopeTagIds</span></span>|<span data-ttu-id="cebdb-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cebdb-171">String collection</span></span>|<span data-ttu-id="cebdb-172">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cebdb-172">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cebdb-173">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-173">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-174">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cebdb-174">supportsScopeTags</span></span>|<span data-ttu-id="cebdb-175">Boolean.</span><span class="sxs-lookup"><span data-stu-id="cebdb-175">Boolean</span></span>|<span data-ttu-id="cebdb-176">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cebdb-176">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cebdb-177">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cebdb-177">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cebdb-178">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cebdb-178">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cebdb-179">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cebdb-179">This property is read-only.</span></span> <span data-ttu-id="cebdb-180">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cebdb-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cebdb-181">version</span><span class="sxs-lookup"><span data-stu-id="cebdb-181">version</span></span>|<span data-ttu-id="cebdb-182">Int32</span><span class="sxs-lookup"><span data-stu-id="cebdb-182">Int32</span></span>|<span data-ttu-id="cebdb-183">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cebdb-183">Version of the device configuration.</span></span> <span data-ttu-id="cebdb-184">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cebdb-184">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cebdb-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="cebdb-185">Response</span></span>

<span data-ttu-id="cebdb-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cebdb-186">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cebdb-187">Пример</span><span class="sxs-lookup"><span data-stu-id="cebdb-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="cebdb-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="cebdb-188">Request</span></span>

<span data-ttu-id="cebdb-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cebdb-189">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="cebdb-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="cebdb-190">Response</span></span>

<span data-ttu-id="cebdb-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cebdb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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







