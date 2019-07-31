---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойств объекта iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ac40ea4db07efbece791c9c7e383de0caee5150
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951836"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="6029a-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="6029a-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="6029a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6029a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6029a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6029a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6029a-106">Обновление свойств объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6029a-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6029a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6029a-107">Prerequisites</span></span>
<span data-ttu-id="6029a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6029a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6029a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6029a-110">Permission type</span></span>|<span data-ttu-id="6029a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6029a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6029a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6029a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6029a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6029a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6029a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6029a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6029a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6029a-115">Not supported.</span></span>|
|<span data-ttu-id="6029a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6029a-116">Application</span></span>|<span data-ttu-id="6029a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6029a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6029a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6029a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6029a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6029a-119">Request headers</span></span>
|<span data-ttu-id="6029a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6029a-120">Header</span></span>|<span data-ttu-id="6029a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6029a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6029a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6029a-122">Authorization</span></span>|<span data-ttu-id="6029a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6029a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6029a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6029a-124">Accept</span></span>|<span data-ttu-id="6029a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6029a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6029a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6029a-126">Request body</span></span>
<span data-ttu-id="6029a-127">В тексте запроса добавьте представление объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6029a-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="6029a-128">В следующей таблице приведены свойства, необходимые при создании [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6029a-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="6029a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6029a-129">Property</span></span>|<span data-ttu-id="6029a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6029a-130">Type</span></span>|<span data-ttu-id="6029a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6029a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6029a-132">id</span><span class="sxs-lookup"><span data-stu-id="6029a-132">id</span></span>|<span data-ttu-id="6029a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6029a-133">String</span></span>|<span data-ttu-id="6029a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6029a-134">Key of the entity.</span></span>|
|<span data-ttu-id="6029a-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6029a-135">expirationDateTime</span></span>|<span data-ttu-id="6029a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6029a-136">DateTimeOffset</span></span>|<span data-ttu-id="6029a-137">Дата и время необязательного окончания срока действия профиля.</span><span class="sxs-lookup"><span data-stu-id="6029a-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="6029a-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6029a-138">payloadFileName</span></span>|<span data-ttu-id="6029a-139">String</span><span class="sxs-lookup"><span data-stu-id="6029a-139">String</span></span>|<span data-ttu-id="6029a-140">Имя файла полезных данных (\*. мобилепровисион</span><span class="sxs-lookup"><span data-stu-id="6029a-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="6029a-141">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6029a-141">\*.xml).</span></span>|
|<span data-ttu-id="6029a-142">payload</span><span class="sxs-lookup"><span data-stu-id="6029a-142">payload</span></span>|<span data-ttu-id="6029a-143">Binary</span><span class="sxs-lookup"><span data-stu-id="6029a-143">Binary</span></span>|<span data-ttu-id="6029a-144">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="6029a-144">Payload.</span></span> <span data-ttu-id="6029a-145">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="6029a-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6029a-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6029a-146">roleScopeTagIds</span></span>|<span data-ttu-id="6029a-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6029a-147">String collection</span></span>|<span data-ttu-id="6029a-148">Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="6029a-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="6029a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6029a-149">createdDateTime</span></span>|<span data-ttu-id="6029a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6029a-150">DateTimeOffset</span></span>|<span data-ttu-id="6029a-151">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6029a-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="6029a-152">description</span><span class="sxs-lookup"><span data-stu-id="6029a-152">description</span></span>|<span data-ttu-id="6029a-153">String</span><span class="sxs-lookup"><span data-stu-id="6029a-153">String</span></span>|<span data-ttu-id="6029a-154">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6029a-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="6029a-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6029a-155">lastModifiedDateTime</span></span>|<span data-ttu-id="6029a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6029a-156">DateTimeOffset</span></span>|<span data-ttu-id="6029a-157">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6029a-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6029a-158">displayName</span><span class="sxs-lookup"><span data-stu-id="6029a-158">displayName</span></span>|<span data-ttu-id="6029a-159">Строка</span><span class="sxs-lookup"><span data-stu-id="6029a-159">String</span></span>|<span data-ttu-id="6029a-160">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6029a-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="6029a-161">version</span><span class="sxs-lookup"><span data-stu-id="6029a-161">version</span></span>|<span data-ttu-id="6029a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6029a-162">Int32</span></span>|<span data-ttu-id="6029a-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6029a-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="6029a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="6029a-164">Response</span></span>
<span data-ttu-id="6029a-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6029a-165">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6029a-166">Пример</span><span class="sxs-lookup"><span data-stu-id="6029a-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="6029a-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="6029a-167">Request</span></span>
<span data-ttu-id="6029a-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6029a-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6029a-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="6029a-169">Response</span></span>
<span data-ttu-id="6029a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6029a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





