---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойств объекта iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a33e868fc5910e6d3d167b3e5541cd9abafea94b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036172"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="7e4cf-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e4cf-103">Update iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="7e4cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e4cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e4cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e4cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e4cf-107">Обновление свойств объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7e4cf-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e4cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e4cf-108">Prerequisites</span></span>
<span data-ttu-id="7e4cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e4cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e4cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e4cf-111">Permission type</span></span>|<span data-ttu-id="7e4cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e4cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e4cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e4cf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7e4cf-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="7e4cf-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="7e4cf-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e4cf-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7e4cf-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="7e4cf-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7e4cf-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e4cf-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e4cf-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e4cf-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e4cf-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-119">Not supported.</span></span>|
|<span data-ttu-id="7e4cf-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e4cf-120">Application</span></span>||
| <span data-ttu-id="7e4cf-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="7e4cf-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="7e4cf-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e4cf-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7e4cf-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="7e4cf-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7e4cf-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e4cf-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e4cf-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e4cf-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7e4cf-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e4cf-126">Request headers</span></span>
|<span data-ttu-id="7e4cf-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e4cf-127">Header</span></span>|<span data-ttu-id="7e4cf-128">Значение</span><span class="sxs-lookup"><span data-stu-id="7e4cf-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e4cf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e4cf-129">Authorization</span></span>|<span data-ttu-id="7e4cf-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e4cf-131">Accept</span><span class="sxs-lookup"><span data-stu-id="7e4cf-131">Accept</span></span>|<span data-ttu-id="7e4cf-132">application/json</span><span class="sxs-lookup"><span data-stu-id="7e4cf-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e4cf-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e4cf-133">Request body</span></span>
<span data-ttu-id="7e4cf-134">В тексте запроса добавьте представление объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-134">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="7e4cf-135">В следующей таблице приведены свойства, необходимые при создании [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e4cf-135">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="7e4cf-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e4cf-136">Property</span></span>|<span data-ttu-id="7e4cf-137">Тип</span><span class="sxs-lookup"><span data-stu-id="7e4cf-137">Type</span></span>|<span data-ttu-id="7e4cf-138">Описание</span><span class="sxs-lookup"><span data-stu-id="7e4cf-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e4cf-139">id</span><span class="sxs-lookup"><span data-stu-id="7e4cf-139">id</span></span>|<span data-ttu-id="7e4cf-140">String</span><span class="sxs-lookup"><span data-stu-id="7e4cf-140">String</span></span>|<span data-ttu-id="7e4cf-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-141">Key of the entity.</span></span>|
|<span data-ttu-id="7e4cf-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e4cf-142">expirationDateTime</span></span>|<span data-ttu-id="7e4cf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e4cf-143">DateTimeOffset</span></span>|<span data-ttu-id="7e4cf-144">Дата и время необязательного окончания срока действия профиля.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="7e4cf-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="7e4cf-145">payloadFileName</span></span>|<span data-ttu-id="7e4cf-146">String</span><span class="sxs-lookup"><span data-stu-id="7e4cf-146">String</span></span>|<span data-ttu-id="7e4cf-147">Имя файла полезных данных (\*. мобилепровисион</span><span class="sxs-lookup"><span data-stu-id="7e4cf-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="7e4cf-148">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="7e4cf-148">\*.xml).</span></span>|
|<span data-ttu-id="7e4cf-149">payload</span><span class="sxs-lookup"><span data-stu-id="7e4cf-149">payload</span></span>|<span data-ttu-id="7e4cf-150">Binary</span><span class="sxs-lookup"><span data-stu-id="7e4cf-150">Binary</span></span>|<span data-ttu-id="7e4cf-151">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="7e4cf-151">Payload.</span></span> <span data-ttu-id="7e4cf-152">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="7e4cf-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="7e4cf-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e4cf-153">roleScopeTagIds</span></span>|<span data-ttu-id="7e4cf-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7e4cf-154">String collection</span></span>|<span data-ttu-id="7e4cf-155">Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="7e4cf-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e4cf-156">createdDateTime</span></span>|<span data-ttu-id="7e4cf-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e4cf-157">DateTimeOffset</span></span>|<span data-ttu-id="7e4cf-158">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="7e4cf-159">description</span><span class="sxs-lookup"><span data-stu-id="7e4cf-159">description</span></span>|<span data-ttu-id="7e4cf-160">String</span><span class="sxs-lookup"><span data-stu-id="7e4cf-160">String</span></span>|<span data-ttu-id="7e4cf-161">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7e4cf-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e4cf-162">lastModifiedDateTime</span></span>|<span data-ttu-id="7e4cf-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e4cf-163">DateTimeOffset</span></span>|<span data-ttu-id="7e4cf-164">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7e4cf-165">displayName</span><span class="sxs-lookup"><span data-stu-id="7e4cf-165">displayName</span></span>|<span data-ttu-id="7e4cf-166">String</span><span class="sxs-lookup"><span data-stu-id="7e4cf-166">String</span></span>|<span data-ttu-id="7e4cf-167">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7e4cf-168">version</span><span class="sxs-lookup"><span data-stu-id="7e4cf-168">version</span></span>|<span data-ttu-id="7e4cf-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7e4cf-169">Int32</span></span>|<span data-ttu-id="7e4cf-170">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="7e4cf-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e4cf-171">Response</span></span>
<span data-ttu-id="7e4cf-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-172">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e4cf-173">Пример</span><span class="sxs-lookup"><span data-stu-id="7e4cf-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e4cf-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e4cf-174">Request</span></span>
<span data-ttu-id="7e4cf-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e4cf-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e4cf-176">Response</span></span>
<span data-ttu-id="7e4cf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e4cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









