---
title: Создание windowsDomainJoinConfiguration
description: Создайте новый объект windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55244869dd22c626d211a2b24e30e7befa28c6af
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866981"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="88a43-103">Создание windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="88a43-103">Create windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="88a43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88a43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88a43-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="88a43-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88a43-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a43-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88a43-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88a43-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a43-108">Создайте [новый объект windowsDomainJoinConfiguration.](../resources/intune-shared-windowsdomainjoinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88a43-108">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88a43-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88a43-109">Prerequisites</span></span>
<span data-ttu-id="88a43-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a43-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88a43-112">Permission type</span></span>|<span data-ttu-id="88a43-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88a43-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88a43-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88a43-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88a43-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="88a43-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a43-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a43-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="88a43-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88a43-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88a43-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a43-118">Not supported.</span></span>|
|<span data-ttu-id="88a43-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="88a43-119">Application</span></span>||
| <span data-ttu-id="88a43-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="88a43-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a43-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a43-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88a43-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88a43-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="88a43-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88a43-123">Request headers</span></span>

|<span data-ttu-id="88a43-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88a43-124">Header</span></span>|<span data-ttu-id="88a43-125">Значение</span><span class="sxs-lookup"><span data-stu-id="88a43-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a43-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88a43-126">Authorization</span></span>|<span data-ttu-id="88a43-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88a43-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a43-128">Accept</span><span class="sxs-lookup"><span data-stu-id="88a43-128">Accept</span></span>|<span data-ttu-id="88a43-129">application/json</span><span class="sxs-lookup"><span data-stu-id="88a43-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a43-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88a43-130">Request body</span></span>

<span data-ttu-id="88a43-131">В корпусе запроса поставляем представление JSON для объекта windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="88a43-131">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="88a43-132">В следующей таблице показаны свойства, необходимые при создании windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="88a43-132">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="88a43-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a43-133">Property</span></span>|<span data-ttu-id="88a43-134">Тип</span><span class="sxs-lookup"><span data-stu-id="88a43-134">Type</span></span>|<span data-ttu-id="88a43-135">Описание</span><span class="sxs-lookup"><span data-stu-id="88a43-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a43-136">id</span><span class="sxs-lookup"><span data-stu-id="88a43-136">id</span></span>|<span data-ttu-id="88a43-137">String</span><span class="sxs-lookup"><span data-stu-id="88a43-137">String</span></span>|<span data-ttu-id="88a43-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="88a43-138">Key of the entity.</span></span> <span data-ttu-id="88a43-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-140">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="88a43-140">**Device configuration**</span></span>|
|<span data-ttu-id="88a43-141">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="88a43-141">activeDirectoryDomainName</span></span>|<span data-ttu-id="88a43-142">String</span><span class="sxs-lookup"><span data-stu-id="88a43-142">String</span></span>|<span data-ttu-id="88a43-143">Доменное имя Active Directory для пользования.</span><span class="sxs-lookup"><span data-stu-id="88a43-143">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="88a43-144">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="88a43-144">computerNameStaticPrefix</span></span>|<span data-ttu-id="88a43-145">String</span><span class="sxs-lookup"><span data-stu-id="88a43-145">String</span></span>|<span data-ttu-id="88a43-146">Исправленная префикс, которая будет использоваться для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="88a43-146">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="88a43-147">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="88a43-147">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="88a43-148">Int32</span><span class="sxs-lookup"><span data-stu-id="88a43-148">Int32</span></span>|<span data-ttu-id="88a43-149">Динамически созданные символы, используемые в качестве суффикса для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="88a43-149">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="88a43-150">Допустимые значения от 3 до 14</span><span class="sxs-lookup"><span data-stu-id="88a43-150">Valid values 3 to 14</span></span>|
|<span data-ttu-id="88a43-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88a43-151">createdDateTime</span></span>|<span data-ttu-id="88a43-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a43-152">DateTimeOffset</span></span>|<span data-ttu-id="88a43-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="88a43-153">DateTime the object was created.</span></span> <span data-ttu-id="88a43-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-155">description</span><span class="sxs-lookup"><span data-stu-id="88a43-155">description</span></span>|<span data-ttu-id="88a43-156">String</span><span class="sxs-lookup"><span data-stu-id="88a43-156">String</span></span>|<span data-ttu-id="88a43-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="88a43-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88a43-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-159">displayName</span><span class="sxs-lookup"><span data-stu-id="88a43-159">displayName</span></span>|<span data-ttu-id="88a43-160">String</span><span class="sxs-lookup"><span data-stu-id="88a43-160">String</span></span>|<span data-ttu-id="88a43-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="88a43-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88a43-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88a43-163">lastModifiedDateTime</span></span>|<span data-ttu-id="88a43-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a43-164">DateTimeOffset</span></span>|<span data-ttu-id="88a43-165">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="88a43-165">DateTime the object was last modified.</span></span> <span data-ttu-id="88a43-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-167">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="88a43-167">organizationalUnit</span></span>|<span data-ttu-id="88a43-168">String</span><span class="sxs-lookup"><span data-stu-id="88a43-168">String</span></span>|<span data-ttu-id="88a43-169">Организационное подразделение (OU), в котором будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="88a43-169">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="88a43-170">Если этот параметр NULL, хорошо известный контейнер объектов компьютера будет использоваться как опубликованный в домене.</span><span class="sxs-lookup"><span data-stu-id="88a43-170">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="88a43-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88a43-171">roleScopeTagIds</span></span>|<span data-ttu-id="88a43-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="88a43-172">String collection</span></span>|<span data-ttu-id="88a43-173">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="88a43-173">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88a43-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-175">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88a43-175">supportsScopeTags</span></span>|<span data-ttu-id="88a43-176">Логический</span><span class="sxs-lookup"><span data-stu-id="88a43-176">Boolean</span></span>|<span data-ttu-id="88a43-177">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="88a43-177">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88a43-178">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="88a43-178">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88a43-179">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="88a43-179">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88a43-180">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88a43-180">This property is read-only.</span></span> <span data-ttu-id="88a43-181">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88a43-182">version</span><span class="sxs-lookup"><span data-stu-id="88a43-182">version</span></span>|<span data-ttu-id="88a43-183">Int32</span><span class="sxs-lookup"><span data-stu-id="88a43-183">Int32</span></span>|<span data-ttu-id="88a43-184">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="88a43-184">Version of the device configuration.</span></span> <span data-ttu-id="88a43-185">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88a43-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="88a43-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a43-186">Response</span></span>

<span data-ttu-id="88a43-187">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="88a43-187">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a43-188">Пример</span><span class="sxs-lookup"><span data-stu-id="88a43-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="88a43-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="88a43-189">Request</span></span>

<span data-ttu-id="88a43-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88a43-190">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="88a43-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a43-191">Response</span></span>

<span data-ttu-id="88a43-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88a43-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










