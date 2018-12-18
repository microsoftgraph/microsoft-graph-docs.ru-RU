---
title: Обновление iosLobAppProvisioningConfiguration
description: Обновление свойства объекта iosLobAppProvisioningConfiguration.
author: tfitzmac
ms.openlocfilehash: df3cc8d27bb242998d513e98b8ce9b7ebfb24fd1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313323"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="9f945-103">Обновление iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f945-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="9f945-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f945-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f945-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f945-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f945-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f945-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f945-107">Обновление свойства объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9f945-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f945-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f945-108">Prerequisites</span></span>
<span data-ttu-id="9f945-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f945-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f945-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f945-111">Permission type</span></span>|<span data-ttu-id="9f945-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f945-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f945-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f945-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f945-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f945-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f945-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f945-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f945-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f945-116">Not supported.</span></span>|
|<span data-ttu-id="9f945-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f945-117">Application</span></span>|<span data-ttu-id="9f945-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f945-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f945-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f945-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f945-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f945-120">Request headers</span></span>
|<span data-ttu-id="9f945-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f945-121">Header</span></span>|<span data-ttu-id="9f945-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f945-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f945-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f945-123">Authorization</span></span>|<span data-ttu-id="9f945-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9f945-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f945-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f945-125">Accept</span></span>|<span data-ttu-id="9f945-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f945-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f945-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f945-127">Request body</span></span>
<span data-ttu-id="9f945-128">В тексте запроса укажите представление JSON для объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9f945-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="9f945-129">В следующей таблице показаны свойства, которые необходимы для создания [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f945-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="9f945-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f945-130">Property</span></span>|<span data-ttu-id="9f945-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f945-131">Type</span></span>|<span data-ttu-id="9f945-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f945-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f945-133">id</span><span class="sxs-lookup"><span data-stu-id="9f945-133">id</span></span>|<span data-ttu-id="9f945-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9f945-134">String</span></span>|<span data-ttu-id="9f945-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f945-135">Key of the entity.</span></span>|
|<span data-ttu-id="9f945-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9f945-136">expirationDateTime</span></span>|<span data-ttu-id="9f945-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f945-137">DateTimeOffset</span></span>|<span data-ttu-id="9f945-138">Необязательный профиль истечение срока действия Дата и время.</span><span class="sxs-lookup"><span data-stu-id="9f945-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="9f945-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="9f945-139">payloadFileName</span></span>|<span data-ttu-id="9f945-140">String</span><span class="sxs-lookup"><span data-stu-id="9f945-140">String</span></span>|<span data-ttu-id="9f945-141">Имя файла полезной нагрузки (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="9f945-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="9f945-142">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="9f945-142">\*.xml).</span></span>|
|<span data-ttu-id="9f945-143">payload</span><span class="sxs-lookup"><span data-stu-id="9f945-143">payload</span></span>|<span data-ttu-id="9f945-144">Binary</span><span class="sxs-lookup"><span data-stu-id="9f945-144">Binary</span></span>|<span data-ttu-id="9f945-145">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="9f945-145">Payload.</span></span> <span data-ttu-id="9f945-146">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="9f945-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="9f945-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f945-147">createdDateTime</span></span>|<span data-ttu-id="9f945-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f945-148">DateTimeOffset</span></span>|<span data-ttu-id="9f945-149">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9f945-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="9f945-150">описание</span><span class="sxs-lookup"><span data-stu-id="9f945-150">description</span></span>|<span data-ttu-id="9f945-151">Строка</span><span class="sxs-lookup"><span data-stu-id="9f945-151">String</span></span>|<span data-ttu-id="9f945-152">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f945-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="9f945-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f945-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9f945-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f945-154">DateTimeOffset</span></span>|<span data-ttu-id="9f945-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9f945-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9f945-156">displayName</span><span class="sxs-lookup"><span data-stu-id="9f945-156">displayName</span></span>|<span data-ttu-id="9f945-157">Строка</span><span class="sxs-lookup"><span data-stu-id="9f945-157">String</span></span>|<span data-ttu-id="9f945-158">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f945-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="9f945-159">version</span><span class="sxs-lookup"><span data-stu-id="9f945-159">version</span></span>|<span data-ttu-id="9f945-160">Int32</span><span class="sxs-lookup"><span data-stu-id="9f945-160">Int32</span></span>|<span data-ttu-id="9f945-161">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f945-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="9f945-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f945-162">Response</span></span>
<span data-ttu-id="9f945-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f945-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f945-164">Пример</span><span class="sxs-lookup"><span data-stu-id="9f945-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f945-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f945-165">Request</span></span>
<span data-ttu-id="9f945-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f945-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f945-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f945-167">Response</span></span>
<span data-ttu-id="9f945-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9f945-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





