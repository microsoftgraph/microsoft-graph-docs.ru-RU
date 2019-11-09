---
title: Создание iosLobAppProvisioningConfiguration
description: Создание нового объекта iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35d2d18ded6a4dc24a31fc59b2ac37a899c329a2
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085936"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="d5664-103">Создание iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5664-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="d5664-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5664-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5664-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5664-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5664-106">Создание нового объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d5664-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5664-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5664-107">Prerequisites</span></span>
<span data-ttu-id="d5664-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5664-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5664-110">Permission type</span></span>|<span data-ttu-id="d5664-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5664-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5664-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5664-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5664-113">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="d5664-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d5664-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5664-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d5664-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d5664-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d5664-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5664-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5664-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5664-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5664-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5664-118">Not supported.</span></span>|
|<span data-ttu-id="d5664-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5664-119">Application</span></span>||
| <span data-ttu-id="d5664-120">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="d5664-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d5664-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5664-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d5664-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d5664-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d5664-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5664-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5664-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5664-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5664-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5664-125">Request headers</span></span>
|<span data-ttu-id="d5664-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5664-126">Header</span></span>|<span data-ttu-id="d5664-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d5664-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5664-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5664-128">Authorization</span></span>|<span data-ttu-id="d5664-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5664-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5664-130">Accept</span><span class="sxs-lookup"><span data-stu-id="d5664-130">Accept</span></span>|<span data-ttu-id="d5664-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d5664-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5664-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5664-132">Request body</span></span>
<span data-ttu-id="d5664-133">В тексте запроса добавьте представление объекта iosLobAppProvisioningConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5664-133">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="d5664-134">В следующей таблице приведены свойства, необходимые при создании iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d5664-134">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="d5664-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5664-135">Property</span></span>|<span data-ttu-id="d5664-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d5664-136">Type</span></span>|<span data-ttu-id="d5664-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d5664-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5664-138">id</span><span class="sxs-lookup"><span data-stu-id="d5664-138">id</span></span>|<span data-ttu-id="d5664-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d5664-139">String</span></span>|<span data-ttu-id="d5664-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d5664-140">Key of the entity.</span></span>|
|<span data-ttu-id="d5664-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d5664-141">expirationDateTime</span></span>|<span data-ttu-id="d5664-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5664-142">DateTimeOffset</span></span>|<span data-ttu-id="d5664-143">Дата и время необязательного окончания срока действия профиля.</span><span class="sxs-lookup"><span data-stu-id="d5664-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="d5664-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d5664-144">payloadFileName</span></span>|<span data-ttu-id="d5664-145">String</span><span class="sxs-lookup"><span data-stu-id="d5664-145">String</span></span>|<span data-ttu-id="d5664-146">Имя файла полезных данных (\*. мобилепровисион</span><span class="sxs-lookup"><span data-stu-id="d5664-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="d5664-147">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="d5664-147">\*.xml).</span></span>|
|<span data-ttu-id="d5664-148">payload</span><span class="sxs-lookup"><span data-stu-id="d5664-148">payload</span></span>|<span data-ttu-id="d5664-149">Binary</span><span class="sxs-lookup"><span data-stu-id="d5664-149">Binary</span></span>|<span data-ttu-id="d5664-150">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="d5664-150">Payload.</span></span> <span data-ttu-id="d5664-151">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="d5664-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="d5664-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5664-152">roleScopeTagIds</span></span>|<span data-ttu-id="d5664-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d5664-153">String collection</span></span>|<span data-ttu-id="d5664-154">Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="d5664-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="d5664-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5664-155">createdDateTime</span></span>|<span data-ttu-id="d5664-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5664-156">DateTimeOffset</span></span>|<span data-ttu-id="d5664-157">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d5664-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="d5664-158">description</span><span class="sxs-lookup"><span data-stu-id="d5664-158">description</span></span>|<span data-ttu-id="d5664-159">String</span><span class="sxs-lookup"><span data-stu-id="d5664-159">String</span></span>|<span data-ttu-id="d5664-160">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d5664-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="d5664-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5664-161">lastModifiedDateTime</span></span>|<span data-ttu-id="d5664-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5664-162">DateTimeOffset</span></span>|<span data-ttu-id="d5664-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d5664-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d5664-164">displayName</span><span class="sxs-lookup"><span data-stu-id="d5664-164">displayName</span></span>|<span data-ttu-id="d5664-165">Строка</span><span class="sxs-lookup"><span data-stu-id="d5664-165">String</span></span>|<span data-ttu-id="d5664-166">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d5664-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d5664-167">version</span><span class="sxs-lookup"><span data-stu-id="d5664-167">version</span></span>|<span data-ttu-id="d5664-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d5664-168">Int32</span></span>|<span data-ttu-id="d5664-169">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d5664-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="d5664-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5664-170">Response</span></span>
<span data-ttu-id="d5664-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5664-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5664-172">Пример</span><span class="sxs-lookup"><span data-stu-id="d5664-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5664-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5664-173">Request</span></span>
<span data-ttu-id="d5664-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5664-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
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

### <a name="response"></a><span data-ttu-id="d5664-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5664-175">Response</span></span>
<span data-ttu-id="d5664-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5664-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









