---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойства объекта iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 637c1052f4097c3a33ff4c8fc4949ef48773ce68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859320"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="20f93-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="20f93-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="20f93-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20f93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20f93-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20f93-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="20f93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20f93-107">Обновление свойства объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="20f93-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20f93-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20f93-108">Prerequisites</span></span>
<span data-ttu-id="20f93-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20f93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20f93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20f93-111">Permission type</span></span>|<span data-ttu-id="20f93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20f93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20f93-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f93-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20f93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20f93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f93-116">Not supported.</span></span>|
|<span data-ttu-id="20f93-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20f93-117">Application</span></span>|<span data-ttu-id="20f93-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20f93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="20f93-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20f93-120">Request headers</span></span>
|<span data-ttu-id="20f93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20f93-121">Header</span></span>|<span data-ttu-id="20f93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20f93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20f93-123">Authorization</span></span>|<span data-ttu-id="20f93-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20f93-125">Accept</span></span>|<span data-ttu-id="20f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20f93-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20f93-127">Request body</span></span>
<span data-ttu-id="20f93-128">В тексте запроса укажите представление JSON для объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="20f93-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="20f93-129">В следующей таблице показаны свойства, которые необходимы для создания [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20f93-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="20f93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20f93-130">Property</span></span>|<span data-ttu-id="20f93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20f93-131">Type</span></span>|<span data-ttu-id="20f93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20f93-133">id</span><span class="sxs-lookup"><span data-stu-id="20f93-133">id</span></span>|<span data-ttu-id="20f93-134">Строка</span><span class="sxs-lookup"><span data-stu-id="20f93-134">String</span></span>|<span data-ttu-id="20f93-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20f93-135">Key of the entity.</span></span>|
|<span data-ttu-id="20f93-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="20f93-136">expirationDateTime</span></span>|<span data-ttu-id="20f93-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f93-137">DateTimeOffset</span></span>|<span data-ttu-id="20f93-138">Необязательный профиль истечение срока действия Дата и время.</span><span class="sxs-lookup"><span data-stu-id="20f93-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="20f93-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="20f93-139">payloadFileName</span></span>|<span data-ttu-id="20f93-140">String</span><span class="sxs-lookup"><span data-stu-id="20f93-140">String</span></span>|<span data-ttu-id="20f93-141">Имя файла полезной нагрузки (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="20f93-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="20f93-142">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="20f93-142">\*.xml).</span></span>|
|<span data-ttu-id="20f93-143">payload</span><span class="sxs-lookup"><span data-stu-id="20f93-143">payload</span></span>|<span data-ttu-id="20f93-144">Binary</span><span class="sxs-lookup"><span data-stu-id="20f93-144">Binary</span></span>|<span data-ttu-id="20f93-145">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="20f93-145">Payload.</span></span> <span data-ttu-id="20f93-146">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="20f93-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="20f93-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20f93-147">createdDateTime</span></span>|<span data-ttu-id="20f93-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f93-148">DateTimeOffset</span></span>|<span data-ttu-id="20f93-149">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="20f93-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="20f93-150">описание</span><span class="sxs-lookup"><span data-stu-id="20f93-150">description</span></span>|<span data-ttu-id="20f93-151">Строка</span><span class="sxs-lookup"><span data-stu-id="20f93-151">String</span></span>|<span data-ttu-id="20f93-152">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20f93-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="20f93-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20f93-153">lastModifiedDateTime</span></span>|<span data-ttu-id="20f93-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f93-154">DateTimeOffset</span></span>|<span data-ttu-id="20f93-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="20f93-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="20f93-156">displayName</span><span class="sxs-lookup"><span data-stu-id="20f93-156">displayName</span></span>|<span data-ttu-id="20f93-157">Строка</span><span class="sxs-lookup"><span data-stu-id="20f93-157">String</span></span>|<span data-ttu-id="20f93-158">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20f93-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="20f93-159">version</span><span class="sxs-lookup"><span data-stu-id="20f93-159">version</span></span>|<span data-ttu-id="20f93-160">Int32</span><span class="sxs-lookup"><span data-stu-id="20f93-160">Int32</span></span>|<span data-ttu-id="20f93-161">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20f93-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="20f93-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="20f93-162">Response</span></span>
<span data-ttu-id="20f93-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="20f93-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20f93-164">Пример</span><span class="sxs-lookup"><span data-stu-id="20f93-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="20f93-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="20f93-165">Request</span></span>
<span data-ttu-id="20f93-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20f93-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 304

{
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="20f93-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="20f93-167">Response</span></span>
<span data-ttu-id="20f93-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20f93-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





