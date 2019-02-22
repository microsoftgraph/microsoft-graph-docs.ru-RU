---
title: Обновление windows81WifiImportConfiguration
description: Обновление свойств объекта windows81WifiImportConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3163018e7f8822dbdf151f19949bf1be626c0f66
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162869"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="89d9d-103">Обновление windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="89d9d-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="89d9d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89d9d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89d9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d9d-106">Обновление свойств объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="89d9d-106">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89d9d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89d9d-107">Prerequisites</span></span>
<span data-ttu-id="89d9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="89d9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89d9d-110">Permission type</span></span>|<span data-ttu-id="89d9d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89d9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89d9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89d9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89d9d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d9d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89d9d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89d9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89d9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d9d-115">Not supported.</span></span>|
|<span data-ttu-id="89d9d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89d9d-116">Application</span></span>|<span data-ttu-id="89d9d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89d9d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89d9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="89d9d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89d9d-119">Request headers</span></span>
|<span data-ttu-id="89d9d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89d9d-120">Header</span></span>|<span data-ttu-id="89d9d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89d9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89d9d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89d9d-122">Authorization</span></span>|<span data-ttu-id="89d9d-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="89d9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89d9d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89d9d-124">Accept</span></span>|<span data-ttu-id="89d9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89d9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d9d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89d9d-126">Request body</span></span>
<span data-ttu-id="89d9d-127">В тексте запроса добавьте представление объекта [Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89d9d-127">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="89d9d-128">В следующей таблице приведены свойства, необходимые при создании [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-128">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="89d9d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="89d9d-129">Property</span></span>|<span data-ttu-id="89d9d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="89d9d-130">Type</span></span>|<span data-ttu-id="89d9d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="89d9d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d9d-132">id</span><span class="sxs-lookup"><span data-stu-id="89d9d-132">id</span></span>|<span data-ttu-id="89d9d-133">String</span><span class="sxs-lookup"><span data-stu-id="89d9d-133">String</span></span>|<span data-ttu-id="89d9d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89d9d-134">Key of the entity.</span></span> <span data-ttu-id="89d9d-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89d9d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="89d9d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d9d-137">DateTimeOffset</span></span>|<span data-ttu-id="89d9d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="89d9d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="89d9d-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89d9d-140">roleScopeTagIds</span></span>|<span data-ttu-id="89d9d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="89d9d-141">String collection</span></span>|<span data-ttu-id="89d9d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="89d9d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89d9d-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="89d9d-144">supportsScopeTags</span></span>|<span data-ttu-id="89d9d-145">Логический</span><span class="sxs-lookup"><span data-stu-id="89d9d-145">Boolean</span></span>|<span data-ttu-id="89d9d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="89d9d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89d9d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="89d9d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89d9d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="89d9d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89d9d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89d9d-149">This property is read-only.</span></span> <span data-ttu-id="89d9d-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89d9d-151">createdDateTime</span></span>|<span data-ttu-id="89d9d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d9d-152">DateTimeOffset</span></span>|<span data-ttu-id="89d9d-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="89d9d-153">DateTime the object was created.</span></span> <span data-ttu-id="89d9d-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-155">description</span><span class="sxs-lookup"><span data-stu-id="89d9d-155">description</span></span>|<span data-ttu-id="89d9d-156">String</span><span class="sxs-lookup"><span data-stu-id="89d9d-156">String</span></span>|<span data-ttu-id="89d9d-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89d9d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89d9d-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="89d9d-159">displayName</span></span>|<span data-ttu-id="89d9d-160">String</span><span class="sxs-lookup"><span data-stu-id="89d9d-160">String</span></span>|<span data-ttu-id="89d9d-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89d9d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89d9d-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-163">version</span><span class="sxs-lookup"><span data-stu-id="89d9d-163">version</span></span>|<span data-ttu-id="89d9d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="89d9d-164">Int32</span></span>|<span data-ttu-id="89d9d-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89d9d-165">Version of the device configuration.</span></span> <span data-ttu-id="89d9d-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d9d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d9d-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="89d9d-167">payloadFileName</span></span>|<span data-ttu-id="89d9d-168">String</span><span class="sxs-lookup"><span data-stu-id="89d9d-168">String</span></span>|<span data-ttu-id="89d9d-169">Имя файла полезных данных (XML).</span><span class="sxs-lookup"><span data-stu-id="89d9d-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="89d9d-170">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="89d9d-170">profileName</span></span>|<span data-ttu-id="89d9d-171">String</span><span class="sxs-lookup"><span data-stu-id="89d9d-171">String</span></span>|<span data-ttu-id="89d9d-172">Имя профиля, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="89d9d-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="89d9d-173">payload</span><span class="sxs-lookup"><span data-stu-id="89d9d-173">payload</span></span>|<span data-ttu-id="89d9d-174">Binary</span><span class="sxs-lookup"><span data-stu-id="89d9d-174">Binary</span></span>|<span data-ttu-id="89d9d-175">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="89d9d-175">Payload.</span></span> <span data-ttu-id="89d9d-176">(Массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="89d9d-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="89d9d-177">Это XML-файл, сохраненный на устройстве, используемом для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="89d9d-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="89d9d-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="89d9d-178">Response</span></span>
<span data-ttu-id="89d9d-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89d9d-179">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89d9d-180">Пример</span><span class="sxs-lookup"><span data-stu-id="89d9d-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="89d9d-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="89d9d-181">Request</span></span>
<span data-ttu-id="89d9d-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89d9d-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="89d9d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="89d9d-183">Response</span></span>
<span data-ttu-id="89d9d-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89d9d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```




