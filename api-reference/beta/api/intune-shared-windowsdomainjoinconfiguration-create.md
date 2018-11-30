---
title: Создание windowsDomainJoinConfiguration
description: Создание нового объекта windowsDomainJoinConfiguration.
ms.openlocfilehash: 8069dfac727ee24d96f72875a4cec19fa42b8baa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082129"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="cb327-103">Создание windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb327-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="cb327-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb327-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb327-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb327-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb327-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb327-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb327-107">Создание нового объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cb327-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb327-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb327-108">Prerequisites</span></span>
<span data-ttu-id="cb327-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb327-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb327-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb327-111">Permission type</span></span>|<span data-ttu-id="cb327-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb327-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb327-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb327-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cb327-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="cb327-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cb327-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb327-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="cb327-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb327-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb327-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb327-117">Not supported.</span></span>|
|<span data-ttu-id="cb327-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb327-118">Application</span></span>|<span data-ttu-id="cb327-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb327-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb327-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb327-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cb327-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb327-121">Request headers</span></span>

|<span data-ttu-id="cb327-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb327-122">Header</span></span>|<span data-ttu-id="cb327-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cb327-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb327-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb327-124">Authorization</span></span>|<span data-ttu-id="cb327-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cb327-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb327-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cb327-126">Accept</span></span>|<span data-ttu-id="cb327-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cb327-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb327-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb327-128">Request body</span></span>

<span data-ttu-id="cb327-129">В тексте запроса укажите представление JSON для объекта windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cb327-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="cb327-130">В следующей таблице показаны свойства, которые необходимы для создания windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cb327-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="cb327-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb327-131">Property</span></span>|<span data-ttu-id="cb327-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cb327-132">Type</span></span>|<span data-ttu-id="cb327-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cb327-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb327-134">id</span><span class="sxs-lookup"><span data-stu-id="cb327-134">id</span></span>|<span data-ttu-id="cb327-135">String</span><span class="sxs-lookup"><span data-stu-id="cb327-135">String</span></span>|<span data-ttu-id="cb327-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb327-136">Key of the entity.</span></span> <span data-ttu-id="cb327-137">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-138">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="cb327-138">**Device configuration**</span></span>|
|<span data-ttu-id="cb327-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="cb327-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="cb327-140">String</span><span class="sxs-lookup"><span data-stu-id="cb327-140">String</span></span>|<span data-ttu-id="cb327-141">Имя домена Active Directory для присоединения к.</span><span class="sxs-lookup"><span data-stu-id="cb327-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="cb327-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="cb327-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="cb327-143">String</span><span class="sxs-lookup"><span data-stu-id="cb327-143">String</span></span>|<span data-ttu-id="cb327-144">Фиксированный префикс для использования для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="cb327-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="cb327-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="cb327-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="cb327-146">Int32</span><span class="sxs-lookup"><span data-stu-id="cb327-146">Int32</span></span>|<span data-ttu-id="cb327-147">Динамически созданные символы, используемого в качестве суффикса имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="cb327-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="cb327-148">Допустимые значения 3 до 14</span><span class="sxs-lookup"><span data-stu-id="cb327-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="cb327-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb327-149">createdDateTime</span></span>|<span data-ttu-id="cb327-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb327-150">DateTimeOffset</span></span>|<span data-ttu-id="cb327-151">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cb327-151">DateTime the object was created.</span></span> <span data-ttu-id="cb327-152">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-153">описание</span><span class="sxs-lookup"><span data-stu-id="cb327-153">description</span></span>|<span data-ttu-id="cb327-154">String</span><span class="sxs-lookup"><span data-stu-id="cb327-154">String</span></span>|<span data-ttu-id="cb327-155">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb327-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb327-156">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-157">displayName</span><span class="sxs-lookup"><span data-stu-id="cb327-157">displayName</span></span>|<span data-ttu-id="cb327-158">String</span><span class="sxs-lookup"><span data-stu-id="cb327-158">String</span></span>|<span data-ttu-id="cb327-159">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb327-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb327-160">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb327-161">lastModifiedDateTime</span></span>|<span data-ttu-id="cb327-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb327-162">DateTimeOffset</span></span>|<span data-ttu-id="cb327-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cb327-163">DateTime the object was last modified.</span></span> <span data-ttu-id="cb327-164">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="cb327-165">organizationalUnit</span></span>|<span data-ttu-id="cb327-166">String</span><span class="sxs-lookup"><span data-stu-id="cb327-166">String</span></span>|<span data-ttu-id="cb327-167">Подразделение (OU) которой будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="cb327-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="cb327-168">Если этот параметр имеет значение NULL, объект контейнера хорошо известных компьютера будет использоваться, опубликованной в домене.</span><span class="sxs-lookup"><span data-stu-id="cb327-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="cb327-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb327-169">roleScopeTagIds</span></span>|<span data-ttu-id="cb327-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cb327-170">String collection</span></span>|<span data-ttu-id="cb327-171">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cb327-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cb327-172">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cb327-173">supportsScopeTags</span></span>|<span data-ttu-id="cb327-174">Логический</span><span class="sxs-lookup"><span data-stu-id="cb327-174">Boolean</span></span>|<span data-ttu-id="cb327-175">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="cb327-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cb327-176">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="cb327-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cb327-177">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cb327-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cb327-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb327-178">This property is read-only.</span></span> <span data-ttu-id="cb327-179">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb327-180">version</span><span class="sxs-lookup"><span data-stu-id="cb327-180">version</span></span>|<span data-ttu-id="cb327-181">Int32</span><span class="sxs-lookup"><span data-stu-id="cb327-181">Int32</span></span>|<span data-ttu-id="cb327-182">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb327-182">Version of the device configuration.</span></span> <span data-ttu-id="cb327-183">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb327-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cb327-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb327-184">Response</span></span>

<span data-ttu-id="cb327-185">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb327-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb327-186">Пример</span><span class="sxs-lookup"><span data-stu-id="cb327-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb327-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb327-187">Request</span></span>

<span data-ttu-id="cb327-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb327-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="cb327-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb327-189">Response</span></span>

<span data-ttu-id="cb327-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb327-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



