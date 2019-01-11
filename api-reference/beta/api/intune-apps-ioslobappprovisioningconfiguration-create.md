---
title: Создание iosLobAppProvisioningConfiguration
description: Создание нового объекта iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7879cc256a041b960f8d4e728e19bfa5f4f0ffe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809102"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="caf34-103">Создание iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="caf34-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="caf34-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="caf34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="caf34-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="caf34-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="caf34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caf34-107">Создание нового объекта [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="caf34-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="caf34-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="caf34-108">Prerequisites</span></span>
<span data-ttu-id="caf34-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caf34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caf34-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caf34-111">Permission type</span></span>|<span data-ttu-id="caf34-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="caf34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caf34-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caf34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="caf34-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf34-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="caf34-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caf34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caf34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf34-116">Not supported.</span></span>|
|<span data-ttu-id="caf34-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caf34-117">Application</span></span>|<span data-ttu-id="caf34-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf34-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caf34-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caf34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="caf34-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caf34-120">Request headers</span></span>
|<span data-ttu-id="caf34-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="caf34-121">Header</span></span>|<span data-ttu-id="caf34-122">Значение</span><span class="sxs-lookup"><span data-stu-id="caf34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caf34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="caf34-123">Authorization</span></span>|<span data-ttu-id="caf34-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="caf34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caf34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="caf34-125">Accept</span></span>|<span data-ttu-id="caf34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="caf34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caf34-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="caf34-127">Request body</span></span>
<span data-ttu-id="caf34-128">В тексте запроса укажите представление JSON для объекта iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="caf34-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="caf34-129">В следующей таблице показаны свойства, которые необходимы для создания iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="caf34-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="caf34-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="caf34-130">Property</span></span>|<span data-ttu-id="caf34-131">Тип</span><span class="sxs-lookup"><span data-stu-id="caf34-131">Type</span></span>|<span data-ttu-id="caf34-132">Описание</span><span class="sxs-lookup"><span data-stu-id="caf34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf34-133">id</span><span class="sxs-lookup"><span data-stu-id="caf34-133">id</span></span>|<span data-ttu-id="caf34-134">Строка</span><span class="sxs-lookup"><span data-stu-id="caf34-134">String</span></span>|<span data-ttu-id="caf34-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="caf34-135">Key of the entity.</span></span>|
|<span data-ttu-id="caf34-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="caf34-136">expirationDateTime</span></span>|<span data-ttu-id="caf34-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf34-137">DateTimeOffset</span></span>|<span data-ttu-id="caf34-138">Необязательный профиль истечение срока действия Дата и время.</span><span class="sxs-lookup"><span data-stu-id="caf34-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="caf34-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="caf34-139">payloadFileName</span></span>|<span data-ttu-id="caf34-140">String</span><span class="sxs-lookup"><span data-stu-id="caf34-140">String</span></span>|<span data-ttu-id="caf34-141">Имя файла полезной нагрузки (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="caf34-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="caf34-142">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="caf34-142">\*.xml).</span></span>|
|<span data-ttu-id="caf34-143">payload</span><span class="sxs-lookup"><span data-stu-id="caf34-143">payload</span></span>|<span data-ttu-id="caf34-144">Binary</span><span class="sxs-lookup"><span data-stu-id="caf34-144">Binary</span></span>|<span data-ttu-id="caf34-145">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="caf34-145">Payload.</span></span> <span data-ttu-id="caf34-146">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="caf34-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="caf34-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caf34-147">createdDateTime</span></span>|<span data-ttu-id="caf34-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf34-148">DateTimeOffset</span></span>|<span data-ttu-id="caf34-149">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="caf34-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="caf34-150">описание</span><span class="sxs-lookup"><span data-stu-id="caf34-150">description</span></span>|<span data-ttu-id="caf34-151">Строка</span><span class="sxs-lookup"><span data-stu-id="caf34-151">String</span></span>|<span data-ttu-id="caf34-152">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="caf34-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="caf34-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caf34-153">lastModifiedDateTime</span></span>|<span data-ttu-id="caf34-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf34-154">DateTimeOffset</span></span>|<span data-ttu-id="caf34-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="caf34-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="caf34-156">displayName</span><span class="sxs-lookup"><span data-stu-id="caf34-156">displayName</span></span>|<span data-ttu-id="caf34-157">Строка</span><span class="sxs-lookup"><span data-stu-id="caf34-157">String</span></span>|<span data-ttu-id="caf34-158">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="caf34-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="caf34-159">version</span><span class="sxs-lookup"><span data-stu-id="caf34-159">version</span></span>|<span data-ttu-id="caf34-160">Int32</span><span class="sxs-lookup"><span data-stu-id="caf34-160">Int32</span></span>|<span data-ttu-id="caf34-161">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="caf34-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="caf34-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="caf34-162">Response</span></span>
<span data-ttu-id="caf34-163">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="caf34-163">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caf34-164">Пример</span><span class="sxs-lookup"><span data-stu-id="caf34-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="caf34-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="caf34-165">Request</span></span>
<span data-ttu-id="caf34-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caf34-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 377

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="caf34-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="caf34-167">Response</span></span>
<span data-ttu-id="caf34-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="caf34-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





