---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойств объекта iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efeecc86bdb481b3b77871551ced12694c3eb590
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471833"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="68657-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="68657-103">Update iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="68657-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68657-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68657-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68657-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68657-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68657-107">Обновление свойств объекта [iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68657-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68657-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68657-108">Prerequisites</span></span>
<span data-ttu-id="68657-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68657-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68657-111">Permission type</span></span>|<span data-ttu-id="68657-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68657-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68657-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68657-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="68657-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="68657-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="68657-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68657-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="68657-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="68657-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="68657-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68657-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68657-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68657-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68657-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68657-119">Not supported.</span></span>|
|<span data-ttu-id="68657-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68657-120">Application</span></span>||
| <span data-ttu-id="68657-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="68657-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="68657-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68657-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="68657-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="68657-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="68657-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68657-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68657-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68657-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="68657-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68657-126">Request headers</span></span>
|<span data-ttu-id="68657-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68657-127">Header</span></span>|<span data-ttu-id="68657-128">Значение</span><span class="sxs-lookup"><span data-stu-id="68657-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68657-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68657-129">Authorization</span></span>|<span data-ttu-id="68657-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68657-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68657-131">Accept</span><span class="sxs-lookup"><span data-stu-id="68657-131">Accept</span></span>|<span data-ttu-id="68657-132">application/json</span><span class="sxs-lookup"><span data-stu-id="68657-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68657-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68657-133">Request body</span></span>
<span data-ttu-id="68657-134">В теле запроса поставляем представление JSON для [объекта iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68657-134">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="68657-135">В следующей таблице показаны свойства, необходимые при создании [iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68657-135">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="68657-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="68657-136">Property</span></span>|<span data-ttu-id="68657-137">Тип</span><span class="sxs-lookup"><span data-stu-id="68657-137">Type</span></span>|<span data-ttu-id="68657-138">Описание</span><span class="sxs-lookup"><span data-stu-id="68657-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68657-139">id</span><span class="sxs-lookup"><span data-stu-id="68657-139">id</span></span>|<span data-ttu-id="68657-140">String</span><span class="sxs-lookup"><span data-stu-id="68657-140">String</span></span>|<span data-ttu-id="68657-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68657-141">Key of the entity.</span></span>|
|<span data-ttu-id="68657-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="68657-142">expirationDateTime</span></span>|<span data-ttu-id="68657-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68657-143">DateTimeOffset</span></span>|<span data-ttu-id="68657-144">Необязательный срок действия профиля.</span><span class="sxs-lookup"><span data-stu-id="68657-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="68657-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="68657-145">payloadFileName</span></span>|<span data-ttu-id="68657-146">String</span><span class="sxs-lookup"><span data-stu-id="68657-146">String</span></span>|<span data-ttu-id="68657-147">Имя файла полезной нагрузки (\*.mobileprovision \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="68657-147">Payload file name (\*.mobileprovision \| \*.xml).</span></span>|
|<span data-ttu-id="68657-148">payload</span><span class="sxs-lookup"><span data-stu-id="68657-148">payload</span></span>|<span data-ttu-id="68657-149">Binary</span><span class="sxs-lookup"><span data-stu-id="68657-149">Binary</span></span>|<span data-ttu-id="68657-150">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="68657-150">Payload.</span></span> <span data-ttu-id="68657-151">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="68657-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="68657-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="68657-152">roleScopeTagIds</span></span>|<span data-ttu-id="68657-153">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="68657-153">String collection</span></span>|<span data-ttu-id="68657-154">Список тегов области для этого объекта конфигурации конфигурации приложения iOS LOB.</span><span class="sxs-lookup"><span data-stu-id="68657-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="68657-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68657-155">createdDateTime</span></span>|<span data-ttu-id="68657-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68657-156">DateTimeOffset</span></span>|<span data-ttu-id="68657-157">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="68657-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="68657-158">description</span><span class="sxs-lookup"><span data-stu-id="68657-158">description</span></span>|<span data-ttu-id="68657-159">String</span><span class="sxs-lookup"><span data-stu-id="68657-159">String</span></span>|<span data-ttu-id="68657-160">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68657-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="68657-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68657-161">lastModifiedDateTime</span></span>|<span data-ttu-id="68657-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68657-162">DateTimeOffset</span></span>|<span data-ttu-id="68657-163">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="68657-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="68657-164">displayName</span><span class="sxs-lookup"><span data-stu-id="68657-164">displayName</span></span>|<span data-ttu-id="68657-165">String</span><span class="sxs-lookup"><span data-stu-id="68657-165">String</span></span>|<span data-ttu-id="68657-166">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68657-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="68657-167">version</span><span class="sxs-lookup"><span data-stu-id="68657-167">version</span></span>|<span data-ttu-id="68657-168">Int32</span><span class="sxs-lookup"><span data-stu-id="68657-168">Int32</span></span>|<span data-ttu-id="68657-169">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68657-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="68657-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="68657-170">Response</span></span>
<span data-ttu-id="68657-171">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68657-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68657-172">Пример</span><span class="sxs-lookup"><span data-stu-id="68657-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="68657-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="68657-173">Request</span></span>
<span data-ttu-id="68657-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68657-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68657-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="68657-175">Response</span></span>
<span data-ttu-id="68657-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68657-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







