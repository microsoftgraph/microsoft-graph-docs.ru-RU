---
title: Создание iosLobAppProvisioningConfiguration
description: Создание нового объекта iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6b260334bfc2a81d48df06107a864c4a0efa018
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939860"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="bd73d-103">Создание iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd73d-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="bd73d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd73d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd73d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd73d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd73d-106">Создание нового объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd73d-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd73d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd73d-107">Prerequisites</span></span>
<span data-ttu-id="bd73d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd73d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd73d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd73d-110">Permission type</span></span>|<span data-ttu-id="bd73d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd73d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd73d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd73d-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bd73d-113">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="bd73d-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bd73d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd73d-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="bd73d-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="bd73d-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="bd73d-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd73d-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd73d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd73d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd73d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd73d-118">Not supported.</span></span>|
|<span data-ttu-id="bd73d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd73d-119">Application</span></span>||
| <span data-ttu-id="bd73d-120">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="bd73d-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bd73d-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd73d-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="bd73d-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="bd73d-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="bd73d-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd73d-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd73d-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd73d-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd73d-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bd73d-125">Request headers</span></span>
|<span data-ttu-id="bd73d-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd73d-126">Header</span></span>|<span data-ttu-id="bd73d-127">Значение</span><span class="sxs-lookup"><span data-stu-id="bd73d-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd73d-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd73d-128">Authorization</span></span>|<span data-ttu-id="bd73d-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd73d-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd73d-130">Accept</span><span class="sxs-lookup"><span data-stu-id="bd73d-130">Accept</span></span>|<span data-ttu-id="bd73d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bd73d-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd73d-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd73d-132">Request body</span></span>
<span data-ttu-id="bd73d-133">В тексте запроса добавьте представление объекта iosLobAppProvisioningConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd73d-133">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="bd73d-134">В следующей таблице приведены свойства, необходимые при создании iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd73d-134">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="bd73d-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd73d-135">Property</span></span>|<span data-ttu-id="bd73d-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bd73d-136">Type</span></span>|<span data-ttu-id="bd73d-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bd73d-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd73d-138">id</span><span class="sxs-lookup"><span data-stu-id="bd73d-138">id</span></span>|<span data-ttu-id="bd73d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="bd73d-139">String</span></span>|<span data-ttu-id="bd73d-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd73d-140">Key of the entity.</span></span>|
|<span data-ttu-id="bd73d-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bd73d-141">expirationDateTime</span></span>|<span data-ttu-id="bd73d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd73d-142">DateTimeOffset</span></span>|<span data-ttu-id="bd73d-143">Дата и время необязательного окончания срока действия профиля.</span><span class="sxs-lookup"><span data-stu-id="bd73d-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="bd73d-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="bd73d-144">payloadFileName</span></span>|<span data-ttu-id="bd73d-145">String</span><span class="sxs-lookup"><span data-stu-id="bd73d-145">String</span></span>|<span data-ttu-id="bd73d-146">Имя файла полезных данных (\*. мобилепровисион</span><span class="sxs-lookup"><span data-stu-id="bd73d-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="bd73d-147">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="bd73d-147">\*.xml).</span></span>|
|<span data-ttu-id="bd73d-148">payload</span><span class="sxs-lookup"><span data-stu-id="bd73d-148">payload</span></span>|<span data-ttu-id="bd73d-149">Binary</span><span class="sxs-lookup"><span data-stu-id="bd73d-149">Binary</span></span>|<span data-ttu-id="bd73d-150">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="bd73d-150">Payload.</span></span> <span data-ttu-id="bd73d-151">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="bd73d-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="bd73d-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd73d-152">roleScopeTagIds</span></span>|<span data-ttu-id="bd73d-153">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd73d-153">String collection</span></span>|<span data-ttu-id="bd73d-154">Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="bd73d-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="bd73d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd73d-155">createdDateTime</span></span>|<span data-ttu-id="bd73d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd73d-156">DateTimeOffset</span></span>|<span data-ttu-id="bd73d-157">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bd73d-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="bd73d-158">description</span><span class="sxs-lookup"><span data-stu-id="bd73d-158">description</span></span>|<span data-ttu-id="bd73d-159">String</span><span class="sxs-lookup"><span data-stu-id="bd73d-159">String</span></span>|<span data-ttu-id="bd73d-160">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd73d-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="bd73d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd73d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="bd73d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd73d-162">DateTimeOffset</span></span>|<span data-ttu-id="bd73d-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bd73d-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bd73d-164">displayName</span><span class="sxs-lookup"><span data-stu-id="bd73d-164">displayName</span></span>|<span data-ttu-id="bd73d-165">Строка</span><span class="sxs-lookup"><span data-stu-id="bd73d-165">String</span></span>|<span data-ttu-id="bd73d-166">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd73d-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="bd73d-167">version</span><span class="sxs-lookup"><span data-stu-id="bd73d-167">version</span></span>|<span data-ttu-id="bd73d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="bd73d-168">Int32</span></span>|<span data-ttu-id="bd73d-169">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd73d-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="bd73d-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd73d-170">Response</span></span>
<span data-ttu-id="bd73d-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd73d-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd73d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="bd73d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd73d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd73d-173">Request</span></span>
<span data-ttu-id="bd73d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd73d-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd73d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd73d-175">Response</span></span>
<span data-ttu-id="bd73d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd73d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








