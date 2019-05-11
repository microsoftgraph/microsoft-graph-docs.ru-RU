---
title: Создание Виндовсдомаинжоинконфигуратион
description: Создание нового объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d20a752b5ce4ba2fb55c8cbe7e41d5221c44a4d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898166"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="4245e-103">Создание Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4245e-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="4245e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4245e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4245e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4245e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4245e-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4245e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4245e-107">Создание нового объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4245e-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4245e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4245e-108">Prerequisites</span></span>
<span data-ttu-id="4245e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4245e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4245e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4245e-111">Permission type</span></span>|<span data-ttu-id="4245e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4245e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4245e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4245e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4245e-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="4245e-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4245e-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4245e-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="4245e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4245e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4245e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4245e-117">Not supported.</span></span>|
|<span data-ttu-id="4245e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4245e-118">Application</span></span>|<span data-ttu-id="4245e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4245e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4245e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4245e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4245e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4245e-121">Request headers</span></span>

|<span data-ttu-id="4245e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4245e-122">Header</span></span>|<span data-ttu-id="4245e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4245e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4245e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4245e-124">Authorization</span></span>|<span data-ttu-id="4245e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4245e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4245e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4245e-126">Accept</span></span>|<span data-ttu-id="4245e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4245e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4245e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4245e-128">Request body</span></span>

<span data-ttu-id="4245e-129">В тексте запроса добавьте представление объекта Виндовсдомаинжоинконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4245e-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="4245e-130">В следующей таблице приведены свойства, необходимые при создании Виндовсдомаинжоинконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4245e-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="4245e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4245e-131">Property</span></span>|<span data-ttu-id="4245e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4245e-132">Type</span></span>|<span data-ttu-id="4245e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4245e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4245e-134">id</span><span class="sxs-lookup"><span data-stu-id="4245e-134">id</span></span>|<span data-ttu-id="4245e-135">String</span><span class="sxs-lookup"><span data-stu-id="4245e-135">String</span></span>|<span data-ttu-id="4245e-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4245e-136">Key of the entity.</span></span> <span data-ttu-id="4245e-137">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-138">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="4245e-138">**Device configuration**</span></span>|
|<span data-ttu-id="4245e-139">Активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="4245e-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="4245e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4245e-140">String</span></span>|<span data-ttu-id="4245e-141">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="4245e-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="4245e-142">Компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="4245e-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="4245e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="4245e-143">String</span></span>|<span data-ttu-id="4245e-144">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="4245e-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="4245e-145">Компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="4245e-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="4245e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4245e-146">Int32</span></span>|<span data-ttu-id="4245e-147">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="4245e-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="4245e-148">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="4245e-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="4245e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4245e-149">createdDateTime</span></span>|<span data-ttu-id="4245e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4245e-150">DateTimeOffset</span></span>|<span data-ttu-id="4245e-151">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4245e-151">DateTime the object was created.</span></span> <span data-ttu-id="4245e-152">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-153">description</span><span class="sxs-lookup"><span data-stu-id="4245e-153">description</span></span>|<span data-ttu-id="4245e-154">String</span><span class="sxs-lookup"><span data-stu-id="4245e-154">String</span></span>|<span data-ttu-id="4245e-155">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4245e-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4245e-156">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-157">displayName</span><span class="sxs-lookup"><span data-stu-id="4245e-157">displayName</span></span>|<span data-ttu-id="4245e-158">Строка</span><span class="sxs-lookup"><span data-stu-id="4245e-158">String</span></span>|<span data-ttu-id="4245e-159">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4245e-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4245e-160">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4245e-161">lastModifiedDateTime</span></span>|<span data-ttu-id="4245e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4245e-162">DateTimeOffset</span></span>|<span data-ttu-id="4245e-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4245e-163">DateTime the object was last modified.</span></span> <span data-ttu-id="4245e-164">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="4245e-165">organizationalUnit</span></span>|<span data-ttu-id="4245e-166">Строка</span><span class="sxs-lookup"><span data-stu-id="4245e-166">String</span></span>|<span data-ttu-id="4245e-167">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="4245e-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="4245e-168">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="4245e-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="4245e-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4245e-169">roleScopeTagIds</span></span>|<span data-ttu-id="4245e-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4245e-170">String collection</span></span>|<span data-ttu-id="4245e-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4245e-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4245e-172">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-173">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4245e-173">supportsScopeTags</span></span>|<span data-ttu-id="4245e-174">Логический</span><span class="sxs-lookup"><span data-stu-id="4245e-174">Boolean</span></span>|<span data-ttu-id="4245e-175">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4245e-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4245e-176">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4245e-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4245e-177">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4245e-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4245e-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4245e-178">This property is read-only.</span></span> <span data-ttu-id="4245e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4245e-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4245e-180">version</span><span class="sxs-lookup"><span data-stu-id="4245e-180">version</span></span>|<span data-ttu-id="4245e-181">Int32</span><span class="sxs-lookup"><span data-stu-id="4245e-181">Int32</span></span>|<span data-ttu-id="4245e-182">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4245e-182">Version of the device configuration.</span></span> <span data-ttu-id="4245e-183">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4245e-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4245e-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="4245e-184">Response</span></span>

<span data-ttu-id="4245e-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4245e-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4245e-186">Пример</span><span class="sxs-lookup"><span data-stu-id="4245e-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="4245e-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="4245e-187">Request</span></span>

<span data-ttu-id="4245e-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4245e-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="4245e-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="4245e-189">Response</span></span>

<span data-ttu-id="4245e-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4245e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



