---
title: Создание windows81WifiImportConfiguration
description: Создание нового объекта windows81WifiImportConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fccaccdee4a7028b3e718c516cfc4c6467eac311
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971999"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="e0c45-103">Создание windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0c45-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="e0c45-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0c45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0c45-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0c45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0c45-106">Создание нового объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e0c45-106">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0c45-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0c45-107">Prerequisites</span></span>
<span data-ttu-id="e0c45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0c45-110">Permission type</span></span>|<span data-ttu-id="e0c45-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0c45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0c45-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0c45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0c45-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c45-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0c45-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0c45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0c45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0c45-115">Not supported.</span></span>|
|<span data-ttu-id="e0c45-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0c45-116">Application</span></span>|<span data-ttu-id="e0c45-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0c45-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0c45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0c45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e0c45-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0c45-119">Request headers</span></span>
|<span data-ttu-id="e0c45-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0c45-120">Header</span></span>|<span data-ttu-id="e0c45-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0c45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0c45-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0c45-122">Authorization</span></span>|<span data-ttu-id="e0c45-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0c45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0c45-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0c45-124">Accept</span></span>|<span data-ttu-id="e0c45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0c45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0c45-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0c45-126">Request body</span></span>
<span data-ttu-id="e0c45-127">В тексте запроса добавьте представление объекта windows81WifiImportConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0c45-127">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="e0c45-128">В следующей таблице приведены свойства, необходимые при создании windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e0c45-128">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="e0c45-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0c45-129">Property</span></span>|<span data-ttu-id="e0c45-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e0c45-130">Type</span></span>|<span data-ttu-id="e0c45-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e0c45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0c45-132">id</span><span class="sxs-lookup"><span data-stu-id="e0c45-132">id</span></span>|<span data-ttu-id="e0c45-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e0c45-133">String</span></span>|<span data-ttu-id="e0c45-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0c45-134">Key of the entity.</span></span> <span data-ttu-id="e0c45-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0c45-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e0c45-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0c45-137">DateTimeOffset</span></span>|<span data-ttu-id="e0c45-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e0c45-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e0c45-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0c45-140">roleScopeTagIds</span></span>|<span data-ttu-id="e0c45-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e0c45-141">String collection</span></span>|<span data-ttu-id="e0c45-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e0c45-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0c45-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e0c45-144">supportsScopeTags</span></span>|<span data-ttu-id="e0c45-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0c45-145">Boolean</span></span>|<span data-ttu-id="e0c45-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e0c45-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0c45-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e0c45-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0c45-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e0c45-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0c45-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0c45-149">This property is read-only.</span></span> <span data-ttu-id="e0c45-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0c45-151">createdDateTime</span></span>|<span data-ttu-id="e0c45-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0c45-152">DateTimeOffset</span></span>|<span data-ttu-id="e0c45-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e0c45-153">DateTime the object was created.</span></span> <span data-ttu-id="e0c45-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-155">description</span><span class="sxs-lookup"><span data-stu-id="e0c45-155">description</span></span>|<span data-ttu-id="e0c45-156">String</span><span class="sxs-lookup"><span data-stu-id="e0c45-156">String</span></span>|<span data-ttu-id="e0c45-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0c45-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0c45-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e0c45-159">displayName</span></span>|<span data-ttu-id="e0c45-160">Строка</span><span class="sxs-lookup"><span data-stu-id="e0c45-160">String</span></span>|<span data-ttu-id="e0c45-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0c45-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0c45-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-163">version</span><span class="sxs-lookup"><span data-stu-id="e0c45-163">version</span></span>|<span data-ttu-id="e0c45-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c45-164">Int32</span></span>|<span data-ttu-id="e0c45-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0c45-165">Version of the device configuration.</span></span> <span data-ttu-id="e0c45-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0c45-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0c45-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e0c45-167">payloadFileName</span></span>|<span data-ttu-id="e0c45-168">String</span><span class="sxs-lookup"><span data-stu-id="e0c45-168">String</span></span>|<span data-ttu-id="e0c45-169">Имя файла полезных данных (XML).</span><span class="sxs-lookup"><span data-stu-id="e0c45-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="e0c45-170">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="e0c45-170">profileName</span></span>|<span data-ttu-id="e0c45-171">String</span><span class="sxs-lookup"><span data-stu-id="e0c45-171">String</span></span>|<span data-ttu-id="e0c45-172">Имя профиля, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="e0c45-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="e0c45-173">payload</span><span class="sxs-lookup"><span data-stu-id="e0c45-173">payload</span></span>|<span data-ttu-id="e0c45-174">Binary</span><span class="sxs-lookup"><span data-stu-id="e0c45-174">Binary</span></span>|<span data-ttu-id="e0c45-175">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="e0c45-175">Payload.</span></span> <span data-ttu-id="e0c45-176">(Массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="e0c45-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="e0c45-177">Это XML-файл, сохраненный на устройстве, используемом для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e0c45-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="e0c45-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0c45-178">Response</span></span>
<span data-ttu-id="e0c45-179">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0c45-179">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c45-180">Пример</span><span class="sxs-lookup"><span data-stu-id="e0c45-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0c45-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0c45-181">Request</span></span>
<span data-ttu-id="e0c45-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0c45-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="e0c45-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0c45-183">Response</span></span>
<span data-ttu-id="e0c45-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0c45-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




