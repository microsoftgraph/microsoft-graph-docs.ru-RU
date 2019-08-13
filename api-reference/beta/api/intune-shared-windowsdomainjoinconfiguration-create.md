---
title: Создание Виндовсдомаинжоинконфигуратион
description: Создание нового объекта Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a11a58f8edf38225ddbd01edfa4c55457840ac9e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350540"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="587a9-103">Создание Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="587a9-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="587a9-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="587a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="587a9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="587a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="587a9-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="587a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="587a9-107">Создание нового объекта [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="587a9-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="587a9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="587a9-108">Prerequisites</span></span>
<span data-ttu-id="587a9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="587a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="587a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="587a9-111">Permission type</span></span>|<span data-ttu-id="587a9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="587a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="587a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="587a9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="587a9-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="587a9-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="587a9-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="587a9-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="587a9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="587a9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="587a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="587a9-117">Not supported.</span></span>|
|<span data-ttu-id="587a9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="587a9-118">Application</span></span>|<span data-ttu-id="587a9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="587a9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="587a9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="587a9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="587a9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="587a9-121">Request headers</span></span>

|<span data-ttu-id="587a9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="587a9-122">Header</span></span>|<span data-ttu-id="587a9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="587a9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="587a9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="587a9-124">Authorization</span></span>|<span data-ttu-id="587a9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="587a9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="587a9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="587a9-126">Accept</span></span>|<span data-ttu-id="587a9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="587a9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="587a9-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="587a9-128">Request body</span></span>

<span data-ttu-id="587a9-129">В тексте запроса добавьте представление объекта Виндовсдомаинжоинконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="587a9-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="587a9-130">В следующей таблице приведены свойства, необходимые при создании Виндовсдомаинжоинконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="587a9-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="587a9-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="587a9-131">Property</span></span>|<span data-ttu-id="587a9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="587a9-132">Type</span></span>|<span data-ttu-id="587a9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="587a9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="587a9-134">id</span><span class="sxs-lookup"><span data-stu-id="587a9-134">id</span></span>|<span data-ttu-id="587a9-135">String</span><span class="sxs-lookup"><span data-stu-id="587a9-135">String</span></span>|<span data-ttu-id="587a9-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="587a9-136">Key of the entity.</span></span> <span data-ttu-id="587a9-137">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-138">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="587a9-138">**Device configuration**</span></span>|
|<span data-ttu-id="587a9-139">активедиректоридомаиннаме</span><span class="sxs-lookup"><span data-stu-id="587a9-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="587a9-140">String</span><span class="sxs-lookup"><span data-stu-id="587a9-140">String</span></span>|<span data-ttu-id="587a9-141">Имя домена Active Directory, к которому необходимо присоединиться.</span><span class="sxs-lookup"><span data-stu-id="587a9-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="587a9-142">компутернаместатикпрефикс</span><span class="sxs-lookup"><span data-stu-id="587a9-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="587a9-143">String</span><span class="sxs-lookup"><span data-stu-id="587a9-143">String</span></span>|<span data-ttu-id="587a9-144">Фиксированный префикс, который будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="587a9-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="587a9-145">компутернамесуффиксрандомчаркаунт</span><span class="sxs-lookup"><span data-stu-id="587a9-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="587a9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="587a9-146">Int32</span></span>|<span data-ttu-id="587a9-147">Динамически создаваемые символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="587a9-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="587a9-148">Допустимые значения — от 3 до 14.</span><span class="sxs-lookup"><span data-stu-id="587a9-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="587a9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="587a9-149">createdDateTime</span></span>|<span data-ttu-id="587a9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="587a9-150">DateTimeOffset</span></span>|<span data-ttu-id="587a9-151">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="587a9-151">DateTime the object was created.</span></span> <span data-ttu-id="587a9-152">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-153">description</span><span class="sxs-lookup"><span data-stu-id="587a9-153">description</span></span>|<span data-ttu-id="587a9-154">String</span><span class="sxs-lookup"><span data-stu-id="587a9-154">String</span></span>|<span data-ttu-id="587a9-155">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="587a9-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="587a9-156">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-157">displayName</span><span class="sxs-lookup"><span data-stu-id="587a9-157">displayName</span></span>|<span data-ttu-id="587a9-158">Строка</span><span class="sxs-lookup"><span data-stu-id="587a9-158">String</span></span>|<span data-ttu-id="587a9-159">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="587a9-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="587a9-160">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="587a9-161">lastModifiedDateTime</span></span>|<span data-ttu-id="587a9-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="587a9-162">DateTimeOffset</span></span>|<span data-ttu-id="587a9-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="587a9-163">DateTime the object was last modified.</span></span> <span data-ttu-id="587a9-164">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="587a9-165">organizationalUnit</span></span>|<span data-ttu-id="587a9-166">String</span><span class="sxs-lookup"><span data-stu-id="587a9-166">String</span></span>|<span data-ttu-id="587a9-167">Подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="587a9-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="587a9-168">Если этот параметр имеет значение NULL, известный контейнер объект-компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="587a9-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="587a9-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="587a9-169">roleScopeTagIds</span></span>|<span data-ttu-id="587a9-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="587a9-170">String collection</span></span>|<span data-ttu-id="587a9-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="587a9-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="587a9-172">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-173">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="587a9-173">supportsScopeTags</span></span>|<span data-ttu-id="587a9-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="587a9-174">Boolean</span></span>|<span data-ttu-id="587a9-175">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="587a9-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="587a9-176">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="587a9-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="587a9-177">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="587a9-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="587a9-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="587a9-178">This property is read-only.</span></span> <span data-ttu-id="587a9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="587a9-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="587a9-180">version</span><span class="sxs-lookup"><span data-stu-id="587a9-180">version</span></span>|<span data-ttu-id="587a9-181">Int32</span><span class="sxs-lookup"><span data-stu-id="587a9-181">Int32</span></span>|<span data-ttu-id="587a9-182">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="587a9-182">Version of the device configuration.</span></span> <span data-ttu-id="587a9-183">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="587a9-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="587a9-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="587a9-184">Response</span></span>

<span data-ttu-id="587a9-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="587a9-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="587a9-186">Пример</span><span class="sxs-lookup"><span data-stu-id="587a9-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="587a9-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="587a9-187">Request</span></span>

<span data-ttu-id="587a9-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="587a9-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="587a9-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="587a9-189">Response</span></span>

<span data-ttu-id="587a9-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="587a9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






