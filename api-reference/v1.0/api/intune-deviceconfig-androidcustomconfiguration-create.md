---
title: Создание объекта androidCustomConfiguration
description: Создание объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 969fcb3ffadf038871c35e3d82ce2dbb7859e0d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872658"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="fdead-103">Создание объекта androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="fdead-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="fdead-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fdead-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdead-105">Создание объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-105">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdead-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fdead-106">Prerequisites</span></span>
<span data-ttu-id="fdead-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdead-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdead-109">Permission type</span></span>|<span data-ttu-id="fdead-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdead-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdead-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdead-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fdead-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdead-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdead-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdead-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdead-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdead-114">Not supported.</span></span>|
|<span data-ttu-id="fdead-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdead-115">Application</span></span>|<span data-ttu-id="fdead-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdead-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdead-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdead-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fdead-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdead-118">Request headers</span></span>
|<span data-ttu-id="fdead-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdead-119">Header</span></span>|<span data-ttu-id="fdead-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fdead-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdead-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdead-121">Authorization</span></span>|<span data-ttu-id="fdead-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fdead-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdead-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fdead-123">Accept</span></span>|<span data-ttu-id="fdead-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fdead-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdead-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdead-125">Request body</span></span>
<span data-ttu-id="fdead-126">В тексте запроса добавьте представление объекта androidCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdead-126">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="fdead-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fdead-127">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="fdead-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdead-128">Property</span></span>|<span data-ttu-id="fdead-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fdead-129">Type</span></span>|<span data-ttu-id="fdead-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fdead-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdead-131">id</span><span class="sxs-lookup"><span data-stu-id="fdead-131">id</span></span>|<span data-ttu-id="fdead-132">Строка</span><span class="sxs-lookup"><span data-stu-id="fdead-132">String</span></span>|<span data-ttu-id="fdead-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fdead-133">Key of the entity.</span></span> <span data-ttu-id="fdead-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdead-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdead-135">lastModifiedDateTime</span></span>|<span data-ttu-id="fdead-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdead-136">DateTimeOffset</span></span>|<span data-ttu-id="fdead-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fdead-137">DateTime the object was last modified.</span></span> <span data-ttu-id="fdead-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdead-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdead-139">createdDateTime</span></span>|<span data-ttu-id="fdead-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdead-140">DateTimeOffset</span></span>|<span data-ttu-id="fdead-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fdead-141">DateTime the object was created.</span></span> <span data-ttu-id="fdead-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdead-143">описание</span><span class="sxs-lookup"><span data-stu-id="fdead-143">description</span></span>|<span data-ttu-id="fdead-144">Строка</span><span class="sxs-lookup"><span data-stu-id="fdead-144">String</span></span>|<span data-ttu-id="fdead-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdead-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fdead-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdead-147">displayName</span><span class="sxs-lookup"><span data-stu-id="fdead-147">displayName</span></span>|<span data-ttu-id="fdead-148">Строка</span><span class="sxs-lookup"><span data-stu-id="fdead-148">String</span></span>|<span data-ttu-id="fdead-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdead-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fdead-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdead-151">version</span><span class="sxs-lookup"><span data-stu-id="fdead-151">version</span></span>|<span data-ttu-id="fdead-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fdead-152">Int32</span></span>|<span data-ttu-id="fdead-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdead-153">Version of the device configuration.</span></span> <span data-ttu-id="fdead-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdead-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdead-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="fdead-155">omaSettings</span></span>|<span data-ttu-id="fdead-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fdead-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="fdead-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="fdead-157">OMA settings.</span></span> <span data-ttu-id="fdead-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fdead-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fdead-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdead-159">Response</span></span>
<span data-ttu-id="fdead-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdead-160">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdead-161">Пример</span><span class="sxs-lookup"><span data-stu-id="fdead-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdead-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdead-162">Request</span></span>
<span data-ttu-id="fdead-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdead-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="fdead-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdead-164">Response</span></span>
<span data-ttu-id="fdead-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fdead-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



