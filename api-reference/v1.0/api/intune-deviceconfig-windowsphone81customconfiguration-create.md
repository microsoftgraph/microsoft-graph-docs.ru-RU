---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65e9f8dfd631fed0fb8ae3d8cf5c232ec83ab4f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932422"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="ecff7-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecff7-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="ecff7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ecff7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecff7-105">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-105">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecff7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ecff7-106">Prerequisites</span></span>
<span data-ttu-id="ecff7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecff7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecff7-109">Permission type</span></span>|<span data-ttu-id="ecff7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecff7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecff7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecff7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecff7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecff7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ecff7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecff7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecff7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecff7-114">Not supported.</span></span>|
|<span data-ttu-id="ecff7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecff7-115">Application</span></span>|<span data-ttu-id="ecff7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecff7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecff7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecff7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ecff7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecff7-118">Request headers</span></span>
|<span data-ttu-id="ecff7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ecff7-119">Header</span></span>|<span data-ttu-id="ecff7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ecff7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecff7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecff7-121">Authorization</span></span>|<span data-ttu-id="ecff7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ecff7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecff7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ecff7-123">Accept</span></span>|<span data-ttu-id="ecff7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ecff7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecff7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ecff7-125">Request body</span></span>
<span data-ttu-id="ecff7-126">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecff7-126">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="ecff7-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ecff7-127">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="ecff7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecff7-128">Property</span></span>|<span data-ttu-id="ecff7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ecff7-129">Type</span></span>|<span data-ttu-id="ecff7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ecff7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecff7-131">id</span><span class="sxs-lookup"><span data-stu-id="ecff7-131">id</span></span>|<span data-ttu-id="ecff7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ecff7-132">String</span></span>|<span data-ttu-id="ecff7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ecff7-133">Key of the entity.</span></span> <span data-ttu-id="ecff7-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecff7-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecff7-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ecff7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecff7-136">DateTimeOffset</span></span>|<span data-ttu-id="ecff7-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ecff7-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ecff7-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecff7-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecff7-139">createdDateTime</span></span>|<span data-ttu-id="ecff7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecff7-140">DateTimeOffset</span></span>|<span data-ttu-id="ecff7-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ecff7-141">DateTime the object was created.</span></span> <span data-ttu-id="ecff7-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecff7-143">описание</span><span class="sxs-lookup"><span data-stu-id="ecff7-143">description</span></span>|<span data-ttu-id="ecff7-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ecff7-144">String</span></span>|<span data-ttu-id="ecff7-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ecff7-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ecff7-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecff7-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ecff7-147">displayName</span></span>|<span data-ttu-id="ecff7-148">Строка</span><span class="sxs-lookup"><span data-stu-id="ecff7-148">String</span></span>|<span data-ttu-id="ecff7-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ecff7-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ecff7-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecff7-151">version</span><span class="sxs-lookup"><span data-stu-id="ecff7-151">version</span></span>|<span data-ttu-id="ecff7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ecff7-152">Int32</span></span>|<span data-ttu-id="ecff7-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ecff7-153">Version of the device configuration.</span></span> <span data-ttu-id="ecff7-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecff7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecff7-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ecff7-155">omaSettings</span></span>|<span data-ttu-id="ecff7-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ecff7-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ecff7-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="ecff7-157">OMA settings.</span></span> <span data-ttu-id="ecff7-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ecff7-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ecff7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecff7-159">Response</span></span>
<span data-ttu-id="ecff7-160">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ecff7-160">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecff7-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ecff7-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecff7-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecff7-162">Request</span></span>
<span data-ttu-id="ecff7-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecff7-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ecff7-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecff7-164">Response</span></span>
<span data-ttu-id="ecff7-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ecff7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



