---
title: Создание windowsDomainJoinConfiguration
description: Создание нового объекта windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1622bbcf755837115431e77a9b319d1ca749af28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811636"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="51a97-103">Создание windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="51a97-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="51a97-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51a97-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51a97-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51a97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51a97-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51a97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51a97-107">Создание нового объекта [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="51a97-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51a97-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51a97-108">Prerequisites</span></span>
<span data-ttu-id="51a97-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51a97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51a97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51a97-111">Permission type</span></span>|<span data-ttu-id="51a97-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51a97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51a97-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51a97-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="51a97-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="51a97-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="51a97-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a97-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="51a97-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51a97-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51a97-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51a97-117">Not supported.</span></span>|
|<span data-ttu-id="51a97-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51a97-118">Application</span></span>|<span data-ttu-id="51a97-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51a97-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51a97-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51a97-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="51a97-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51a97-121">Request headers</span></span>

|<span data-ttu-id="51a97-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51a97-122">Header</span></span>|<span data-ttu-id="51a97-123">Значение</span><span class="sxs-lookup"><span data-stu-id="51a97-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51a97-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="51a97-124">Authorization</span></span>|<span data-ttu-id="51a97-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="51a97-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51a97-126">Accept</span><span class="sxs-lookup"><span data-stu-id="51a97-126">Accept</span></span>|<span data-ttu-id="51a97-127">application/json</span><span class="sxs-lookup"><span data-stu-id="51a97-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51a97-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51a97-128">Request body</span></span>

<span data-ttu-id="51a97-129">В тексте запроса укажите представление JSON для объекта windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="51a97-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="51a97-130">В следующей таблице показаны свойства, которые необходимы для создания windowsDomainJoinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="51a97-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="51a97-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="51a97-131">Property</span></span>|<span data-ttu-id="51a97-132">Тип</span><span class="sxs-lookup"><span data-stu-id="51a97-132">Type</span></span>|<span data-ttu-id="51a97-133">Описание</span><span class="sxs-lookup"><span data-stu-id="51a97-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51a97-134">id</span><span class="sxs-lookup"><span data-stu-id="51a97-134">id</span></span>|<span data-ttu-id="51a97-135">Строка</span><span class="sxs-lookup"><span data-stu-id="51a97-135">String</span></span>|<span data-ttu-id="51a97-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51a97-136">Key of the entity.</span></span> <span data-ttu-id="51a97-137">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-138">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="51a97-138">**Device configuration**</span></span>|
|<span data-ttu-id="51a97-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="51a97-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="51a97-140">Строка</span><span class="sxs-lookup"><span data-stu-id="51a97-140">String</span></span>|<span data-ttu-id="51a97-141">Имя домена Active Directory для присоединения к.</span><span class="sxs-lookup"><span data-stu-id="51a97-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="51a97-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="51a97-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="51a97-143">Строка</span><span class="sxs-lookup"><span data-stu-id="51a97-143">String</span></span>|<span data-ttu-id="51a97-144">Фиксированный префикс для использования для имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="51a97-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="51a97-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="51a97-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="51a97-146">Int32</span><span class="sxs-lookup"><span data-stu-id="51a97-146">Int32</span></span>|<span data-ttu-id="51a97-147">Динамически созданные символы, используемого в качестве суффикса имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="51a97-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="51a97-148">Допустимые значения 3 до 14</span><span class="sxs-lookup"><span data-stu-id="51a97-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="51a97-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51a97-149">createdDateTime</span></span>|<span data-ttu-id="51a97-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51a97-150">DateTimeOffset</span></span>|<span data-ttu-id="51a97-151">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="51a97-151">DateTime the object was created.</span></span> <span data-ttu-id="51a97-152">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-153">описание</span><span class="sxs-lookup"><span data-stu-id="51a97-153">description</span></span>|<span data-ttu-id="51a97-154">Строка</span><span class="sxs-lookup"><span data-stu-id="51a97-154">String</span></span>|<span data-ttu-id="51a97-155">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51a97-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51a97-156">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-157">displayName</span><span class="sxs-lookup"><span data-stu-id="51a97-157">displayName</span></span>|<span data-ttu-id="51a97-158">Строка</span><span class="sxs-lookup"><span data-stu-id="51a97-158">String</span></span>|<span data-ttu-id="51a97-159">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51a97-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51a97-160">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51a97-161">lastModifiedDateTime</span></span>|<span data-ttu-id="51a97-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51a97-162">DateTimeOffset</span></span>|<span data-ttu-id="51a97-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="51a97-163">DateTime the object was last modified.</span></span> <span data-ttu-id="51a97-164">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="51a97-165">organizationalUnit</span></span>|<span data-ttu-id="51a97-166">Строка</span><span class="sxs-lookup"><span data-stu-id="51a97-166">String</span></span>|<span data-ttu-id="51a97-167">Подразделение (OU) которой будет создана учетная запись компьютера.</span><span class="sxs-lookup"><span data-stu-id="51a97-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="51a97-168">Если этот параметр имеет значение NULL, объект контейнера хорошо известных компьютера будет использоваться, опубликованной в домене.</span><span class="sxs-lookup"><span data-stu-id="51a97-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="51a97-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51a97-169">roleScopeTagIds</span></span>|<span data-ttu-id="51a97-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="51a97-170">String collection</span></span>|<span data-ttu-id="51a97-171">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="51a97-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51a97-172">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51a97-173">supportsScopeTags</span></span>|<span data-ttu-id="51a97-174">Логический</span><span class="sxs-lookup"><span data-stu-id="51a97-174">Boolean</span></span>|<span data-ttu-id="51a97-175">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="51a97-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51a97-176">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="51a97-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51a97-177">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="51a97-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51a97-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51a97-178">This property is read-only.</span></span> <span data-ttu-id="51a97-179">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51a97-180">version</span><span class="sxs-lookup"><span data-stu-id="51a97-180">version</span></span>|<span data-ttu-id="51a97-181">Int32</span><span class="sxs-lookup"><span data-stu-id="51a97-181">Int32</span></span>|<span data-ttu-id="51a97-182">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51a97-182">Version of the device configuration.</span></span> <span data-ttu-id="51a97-183">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51a97-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="51a97-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="51a97-184">Response</span></span>

<span data-ttu-id="51a97-185">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51a97-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51a97-186">Пример</span><span class="sxs-lookup"><span data-stu-id="51a97-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="51a97-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="51a97-187">Request</span></span>

<span data-ttu-id="51a97-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51a97-188">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="51a97-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="51a97-189">Response</span></span>

<span data-ttu-id="51a97-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51a97-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



