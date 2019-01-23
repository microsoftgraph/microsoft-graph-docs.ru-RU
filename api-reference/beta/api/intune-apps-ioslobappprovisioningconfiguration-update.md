---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойства объекта iosLobAppProvisioningConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d98e19b922b1fd9cd2c9205eae89c0637dca9436
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402673"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="2c741-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c741-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="2c741-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c741-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c741-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c741-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c741-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c741-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c741-107">Обновление свойства объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2c741-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c741-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2c741-108">Prerequisites</span></span>
<span data-ttu-id="2c741-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2c741-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2c741-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c741-111">Permission type</span></span>|<span data-ttu-id="2c741-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c741-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c741-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c741-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c741-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c741-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2c741-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c741-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c741-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c741-116">Not supported.</span></span>|
|<span data-ttu-id="2c741-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c741-117">Application</span></span>|<span data-ttu-id="2c741-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c741-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c741-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c741-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2c741-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c741-120">Request headers</span></span>
|<span data-ttu-id="2c741-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c741-121">Header</span></span>|<span data-ttu-id="2c741-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2c741-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c741-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c741-123">Authorization</span></span>|<span data-ttu-id="2c741-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2c741-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c741-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c741-125">Accept</span></span>|<span data-ttu-id="2c741-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c741-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c741-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c741-127">Request body</span></span>
<span data-ttu-id="2c741-128">В тексте запроса укажите представление JSON для объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2c741-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="2c741-129">В следующей таблице показаны свойства, которые необходимы для создания [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c741-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="2c741-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c741-130">Property</span></span>|<span data-ttu-id="2c741-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2c741-131">Type</span></span>|<span data-ttu-id="2c741-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c741-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c741-133">id</span><span class="sxs-lookup"><span data-stu-id="2c741-133">id</span></span>|<span data-ttu-id="2c741-134">String</span><span class="sxs-lookup"><span data-stu-id="2c741-134">String</span></span>|<span data-ttu-id="2c741-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2c741-135">Key of the entity.</span></span>|
|<span data-ttu-id="2c741-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2c741-136">expirationDateTime</span></span>|<span data-ttu-id="2c741-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c741-137">DateTimeOffset</span></span>|<span data-ttu-id="2c741-138">Необязательный профиль истечение срока действия Дата и время.</span><span class="sxs-lookup"><span data-stu-id="2c741-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="2c741-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="2c741-139">payloadFileName</span></span>|<span data-ttu-id="2c741-140">String</span><span class="sxs-lookup"><span data-stu-id="2c741-140">String</span></span>|<span data-ttu-id="2c741-141">Имя файла полезной нагрузки (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="2c741-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="2c741-142">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="2c741-142">\*.xml).</span></span>|
|<span data-ttu-id="2c741-143">payload</span><span class="sxs-lookup"><span data-stu-id="2c741-143">payload</span></span>|<span data-ttu-id="2c741-144">Binary</span><span class="sxs-lookup"><span data-stu-id="2c741-144">Binary</span></span>|<span data-ttu-id="2c741-145">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="2c741-145">Payload.</span></span> <span data-ttu-id="2c741-146">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="2c741-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="2c741-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c741-147">createdDateTime</span></span>|<span data-ttu-id="2c741-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c741-148">DateTimeOffset</span></span>|<span data-ttu-id="2c741-149">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2c741-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="2c741-150">description</span><span class="sxs-lookup"><span data-stu-id="2c741-150">description</span></span>|<span data-ttu-id="2c741-151">String</span><span class="sxs-lookup"><span data-stu-id="2c741-151">String</span></span>|<span data-ttu-id="2c741-152">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c741-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="2c741-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c741-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2c741-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c741-154">DateTimeOffset</span></span>|<span data-ttu-id="2c741-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2c741-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2c741-156">displayName</span><span class="sxs-lookup"><span data-stu-id="2c741-156">displayName</span></span>|<span data-ttu-id="2c741-157">String</span><span class="sxs-lookup"><span data-stu-id="2c741-157">String</span></span>|<span data-ttu-id="2c741-158">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c741-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="2c741-159">version</span><span class="sxs-lookup"><span data-stu-id="2c741-159">version</span></span>|<span data-ttu-id="2c741-160">Int32</span><span class="sxs-lookup"><span data-stu-id="2c741-160">Int32</span></span>|<span data-ttu-id="2c741-161">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c741-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="2c741-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c741-162">Response</span></span>
<span data-ttu-id="2c741-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c741-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c741-164">Пример</span><span class="sxs-lookup"><span data-stu-id="2c741-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c741-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c741-165">Request</span></span>
<span data-ttu-id="2c741-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c741-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="2c741-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c741-167">Response</span></span>
<span data-ttu-id="2c741-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2c741-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




