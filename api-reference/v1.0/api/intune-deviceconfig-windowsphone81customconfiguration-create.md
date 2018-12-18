---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 02701baa092b32ecdb2519780d05de42c6c73447
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301353"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="d82d5-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d82d5-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="d82d5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d82d5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d82d5-105">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-105">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d82d5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d82d5-106">Prerequisites</span></span>
<span data-ttu-id="d82d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d82d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d82d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d82d5-109">Permission type</span></span>|<span data-ttu-id="d82d5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d82d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d82d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d82d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d82d5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d82d5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d82d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d82d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d82d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d82d5-114">Not supported.</span></span>|
|<span data-ttu-id="d82d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d82d5-115">Application</span></span>|<span data-ttu-id="d82d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d82d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d82d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d82d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d82d5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d82d5-118">Request headers</span></span>
|<span data-ttu-id="d82d5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d82d5-119">Header</span></span>|<span data-ttu-id="d82d5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d82d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d82d5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d82d5-121">Authorization</span></span>|<span data-ttu-id="d82d5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d82d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d82d5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d82d5-123">Accept</span></span>|<span data-ttu-id="d82d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d82d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d82d5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d82d5-125">Request body</span></span>
<span data-ttu-id="d82d5-126">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d82d5-126">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="d82d5-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d82d5-127">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="d82d5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d82d5-128">Property</span></span>|<span data-ttu-id="d82d5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d82d5-129">Type</span></span>|<span data-ttu-id="d82d5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d82d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82d5-131">id</span><span class="sxs-lookup"><span data-stu-id="d82d5-131">id</span></span>|<span data-ttu-id="d82d5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d82d5-132">String</span></span>|<span data-ttu-id="d82d5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d82d5-133">Key of the entity.</span></span> <span data-ttu-id="d82d5-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d82d5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d82d5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d82d5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d82d5-136">DateTimeOffset</span></span>|<span data-ttu-id="d82d5-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d82d5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d82d5-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d82d5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d82d5-139">createdDateTime</span></span>|<span data-ttu-id="d82d5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d82d5-140">DateTimeOffset</span></span>|<span data-ttu-id="d82d5-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d82d5-141">DateTime the object was created.</span></span> <span data-ttu-id="d82d5-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d82d5-143">описание</span><span class="sxs-lookup"><span data-stu-id="d82d5-143">description</span></span>|<span data-ttu-id="d82d5-144">Строка</span><span class="sxs-lookup"><span data-stu-id="d82d5-144">String</span></span>|<span data-ttu-id="d82d5-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d82d5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d82d5-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d82d5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d82d5-147">displayName</span></span>|<span data-ttu-id="d82d5-148">Строка</span><span class="sxs-lookup"><span data-stu-id="d82d5-148">String</span></span>|<span data-ttu-id="d82d5-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d82d5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d82d5-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d82d5-151">version</span><span class="sxs-lookup"><span data-stu-id="d82d5-151">version</span></span>|<span data-ttu-id="d82d5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d82d5-152">Int32</span></span>|<span data-ttu-id="d82d5-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d82d5-153">Version of the device configuration.</span></span> <span data-ttu-id="d82d5-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d82d5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d82d5-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="d82d5-155">omaSettings</span></span>|<span data-ttu-id="d82d5-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d82d5-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="d82d5-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="d82d5-157">OMA settings.</span></span> <span data-ttu-id="d82d5-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="d82d5-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d82d5-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d82d5-159">Response</span></span>
<span data-ttu-id="d82d5-160">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d82d5-160">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d82d5-161">Пример</span><span class="sxs-lookup"><span data-stu-id="d82d5-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="d82d5-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d82d5-162">Request</span></span>
<span data-ttu-id="d82d5-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d82d5-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d82d5-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="d82d5-164">Response</span></span>
<span data-ttu-id="d82d5-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d82d5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



