---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойств объекта iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19c5117b6982bbc4d1e12676ddbe2a4878ef0f8e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983185"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="42483-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="42483-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="42483-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42483-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42483-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42483-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42483-106">Обновление свойств объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="42483-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42483-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42483-107">Prerequisites</span></span>
<span data-ttu-id="42483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42483-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42483-110">Permission type</span></span>|<span data-ttu-id="42483-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42483-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42483-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42483-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42483-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42483-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42483-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42483-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42483-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42483-115">Not supported.</span></span>|
|<span data-ttu-id="42483-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42483-116">Application</span></span>|<span data-ttu-id="42483-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42483-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42483-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42483-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42483-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42483-119">Request headers</span></span>
|<span data-ttu-id="42483-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42483-120">Header</span></span>|<span data-ttu-id="42483-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42483-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42483-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42483-122">Authorization</span></span>|<span data-ttu-id="42483-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42483-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42483-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42483-124">Accept</span></span>|<span data-ttu-id="42483-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42483-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42483-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42483-126">Request body</span></span>
<span data-ttu-id="42483-127">В тексте запроса добавьте представление объекта [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42483-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="42483-128">В следующей таблице приведены свойства, необходимые при создании [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42483-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="42483-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="42483-129">Property</span></span>|<span data-ttu-id="42483-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42483-130">Type</span></span>|<span data-ttu-id="42483-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42483-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42483-132">id</span><span class="sxs-lookup"><span data-stu-id="42483-132">id</span></span>|<span data-ttu-id="42483-133">Строка</span><span class="sxs-lookup"><span data-stu-id="42483-133">String</span></span>|<span data-ttu-id="42483-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42483-134">Key of the entity.</span></span>|
|<span data-ttu-id="42483-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="42483-135">expirationDateTime</span></span>|<span data-ttu-id="42483-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42483-136">DateTimeOffset</span></span>|<span data-ttu-id="42483-137">Дата и время неОбязательного окончания срока действия профиля.</span><span class="sxs-lookup"><span data-stu-id="42483-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="42483-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="42483-138">payloadFileName</span></span>|<span data-ttu-id="42483-139">String</span><span class="sxs-lookup"><span data-stu-id="42483-139">String</span></span>|<span data-ttu-id="42483-140">Имя файла полезных данных (\*. мобилепровисион</span><span class="sxs-lookup"><span data-stu-id="42483-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="42483-141">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="42483-141">\*.xml).</span></span>|
|<span data-ttu-id="42483-142">payload</span><span class="sxs-lookup"><span data-stu-id="42483-142">payload</span></span>|<span data-ttu-id="42483-143">Binary</span><span class="sxs-lookup"><span data-stu-id="42483-143">Binary</span></span>|<span data-ttu-id="42483-144">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="42483-144">Payload.</span></span> <span data-ttu-id="42483-145">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="42483-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="42483-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42483-146">roleScopeTagIds</span></span>|<span data-ttu-id="42483-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42483-147">String collection</span></span>|<span data-ttu-id="42483-148">Список тегов областей для данной сущности конфигурации подготовки бизнес-приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="42483-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="42483-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42483-149">createdDateTime</span></span>|<span data-ttu-id="42483-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42483-150">DateTimeOffset</span></span>|<span data-ttu-id="42483-151">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="42483-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="42483-152">description</span><span class="sxs-lookup"><span data-stu-id="42483-152">description</span></span>|<span data-ttu-id="42483-153">String</span><span class="sxs-lookup"><span data-stu-id="42483-153">String</span></span>|<span data-ttu-id="42483-154">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42483-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="42483-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42483-155">lastModifiedDateTime</span></span>|<span data-ttu-id="42483-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42483-156">DateTimeOffset</span></span>|<span data-ttu-id="42483-157">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="42483-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="42483-158">displayName</span><span class="sxs-lookup"><span data-stu-id="42483-158">displayName</span></span>|<span data-ttu-id="42483-159">Строка</span><span class="sxs-lookup"><span data-stu-id="42483-159">String</span></span>|<span data-ttu-id="42483-160">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42483-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="42483-161">version</span><span class="sxs-lookup"><span data-stu-id="42483-161">version</span></span>|<span data-ttu-id="42483-162">Int32</span><span class="sxs-lookup"><span data-stu-id="42483-162">Int32</span></span>|<span data-ttu-id="42483-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42483-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="42483-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="42483-164">Response</span></span>
<span data-ttu-id="42483-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42483-165">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42483-166">Пример</span><span class="sxs-lookup"><span data-stu-id="42483-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="42483-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="42483-167">Request</span></span>
<span data-ttu-id="42483-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42483-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42483-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="42483-169">Response</span></span>
<span data-ttu-id="42483-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42483-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




