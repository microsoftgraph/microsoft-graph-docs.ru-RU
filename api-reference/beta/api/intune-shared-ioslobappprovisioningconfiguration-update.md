---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойств объекта iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebde41570abd913bb51c320286fd315ad213d843
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443480"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="6d9cc-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d9cc-103">Update iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="6d9cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d9cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d9cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d9cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d9cc-107">Обновление свойств объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6d9cc-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d9cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d9cc-108">Prerequisites</span></span>
<span data-ttu-id="6d9cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d9cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d9cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d9cc-111">Permission type</span></span>|<span data-ttu-id="6d9cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d9cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d9cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d9cc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6d9cc-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="6d9cc-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="6d9cc-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d9cc-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="6d9cc-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6d9cc-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6d9cc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d9cc-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d9cc-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d9cc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d9cc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-119">Not supported.</span></span>|
|<span data-ttu-id="6d9cc-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d9cc-120">Application</span></span>||
| <span data-ttu-id="6d9cc-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="6d9cc-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="6d9cc-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d9cc-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="6d9cc-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6d9cc-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6d9cc-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d9cc-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d9cc-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d9cc-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6d9cc-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6d9cc-126">Request headers</span></span>
|<span data-ttu-id="6d9cc-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d9cc-127">Header</span></span>|<span data-ttu-id="6d9cc-128">Значение</span><span class="sxs-lookup"><span data-stu-id="6d9cc-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d9cc-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d9cc-129">Authorization</span></span>|<span data-ttu-id="6d9cc-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d9cc-131">Accept</span><span class="sxs-lookup"><span data-stu-id="6d9cc-131">Accept</span></span>|<span data-ttu-id="6d9cc-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6d9cc-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d9cc-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d9cc-133">Request body</span></span>
<span data-ttu-id="6d9cc-134">В тексте запроса добавьте представление объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-134">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="6d9cc-135">В следующей таблице приведены свойства, необходимые при создании [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d9cc-135">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="6d9cc-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d9cc-136">Property</span></span>|<span data-ttu-id="6d9cc-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6d9cc-137">Type</span></span>|<span data-ttu-id="6d9cc-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6d9cc-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d9cc-139">id</span><span class="sxs-lookup"><span data-stu-id="6d9cc-139">id</span></span>|<span data-ttu-id="6d9cc-140">Строка</span><span class="sxs-lookup"><span data-stu-id="6d9cc-140">String</span></span>|<span data-ttu-id="6d9cc-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-141">Key of the entity.</span></span>|
|<span data-ttu-id="6d9cc-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6d9cc-142">expirationDateTime</span></span>|<span data-ttu-id="6d9cc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d9cc-143">DateTimeOffset</span></span>|<span data-ttu-id="6d9cc-144">Дата и время необязательного окончания срока действия профиля.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="6d9cc-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6d9cc-145">payloadFileName</span></span>|<span data-ttu-id="6d9cc-146">String</span><span class="sxs-lookup"><span data-stu-id="6d9cc-146">String</span></span>|<span data-ttu-id="6d9cc-147">Имя файла полезных данных (\*. мобилепровисион</span><span class="sxs-lookup"><span data-stu-id="6d9cc-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="6d9cc-148">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6d9cc-148">\*.xml).</span></span>|
|<span data-ttu-id="6d9cc-149">payload</span><span class="sxs-lookup"><span data-stu-id="6d9cc-149">payload</span></span>|<span data-ttu-id="6d9cc-150">Binary</span><span class="sxs-lookup"><span data-stu-id="6d9cc-150">Binary</span></span>|<span data-ttu-id="6d9cc-151">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="6d9cc-151">Payload.</span></span> <span data-ttu-id="6d9cc-152">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="6d9cc-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6d9cc-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6d9cc-153">roleScopeTagIds</span></span>|<span data-ttu-id="6d9cc-154">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="6d9cc-154">String collection</span></span>|<span data-ttu-id="6d9cc-155">Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="6d9cc-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d9cc-156">createdDateTime</span></span>|<span data-ttu-id="6d9cc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d9cc-157">DateTimeOffset</span></span>|<span data-ttu-id="6d9cc-158">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="6d9cc-159">description</span><span class="sxs-lookup"><span data-stu-id="6d9cc-159">description</span></span>|<span data-ttu-id="6d9cc-160">String</span><span class="sxs-lookup"><span data-stu-id="6d9cc-160">String</span></span>|<span data-ttu-id="6d9cc-161">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="6d9cc-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d9cc-162">lastModifiedDateTime</span></span>|<span data-ttu-id="6d9cc-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d9cc-163">DateTimeOffset</span></span>|<span data-ttu-id="6d9cc-164">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6d9cc-165">displayName</span><span class="sxs-lookup"><span data-stu-id="6d9cc-165">displayName</span></span>|<span data-ttu-id="6d9cc-166">Строка</span><span class="sxs-lookup"><span data-stu-id="6d9cc-166">String</span></span>|<span data-ttu-id="6d9cc-167">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="6d9cc-168">version</span><span class="sxs-lookup"><span data-stu-id="6d9cc-168">version</span></span>|<span data-ttu-id="6d9cc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6d9cc-169">Int32</span></span>|<span data-ttu-id="6d9cc-170">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="6d9cc-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d9cc-171">Response</span></span>
<span data-ttu-id="6d9cc-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-172">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d9cc-173">Пример</span><span class="sxs-lookup"><span data-stu-id="6d9cc-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d9cc-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d9cc-174">Request</span></span>
<span data-ttu-id="6d9cc-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="6d9cc-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d9cc-176">Response</span></span>
<span data-ttu-id="6d9cc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d9cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```






