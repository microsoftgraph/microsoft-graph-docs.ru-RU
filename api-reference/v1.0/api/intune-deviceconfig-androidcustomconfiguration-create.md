---
title: Создание объекта androidCustomConfiguration
description: Создание объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fde07e19081d270a3c4b433d2c4f32154245cea
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250357"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="3c9d2-103">Создание объекта androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c9d2-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="3c9d2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c9d2-105">Создание объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-105">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c9d2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3c9d2-106">Prerequisites</span></span>
<span data-ttu-id="3c9d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3c9d2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c9d2-109">Permission type</span></span>|<span data-ttu-id="3c9d2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c9d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c9d2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c9d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c9d2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c9d2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c9d2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c9d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c9d2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-114">Not supported.</span></span>|
|<span data-ttu-id="3c9d2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c9d2-115">Application</span></span>|<span data-ttu-id="3c9d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c9d2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c9d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c9d2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c9d2-118">Request headers</span></span>
|<span data-ttu-id="3c9d2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c9d2-119">Header</span></span>|<span data-ttu-id="3c9d2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3c9d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c9d2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c9d2-121">Authorization</span></span>|<span data-ttu-id="3c9d2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c9d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c9d2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3c9d2-123">Accept</span></span>|<span data-ttu-id="3c9d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c9d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c9d2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c9d2-125">Request body</span></span>
<span data-ttu-id="3c9d2-126">В тексте запроса добавьте представление объекта androidCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-126">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="3c9d2-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-127">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="3c9d2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c9d2-128">Property</span></span>|<span data-ttu-id="3c9d2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3c9d2-129">Type</span></span>|<span data-ttu-id="3c9d2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3c9d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c9d2-131">id</span><span class="sxs-lookup"><span data-stu-id="3c9d2-131">id</span></span>|<span data-ttu-id="3c9d2-132">String</span><span class="sxs-lookup"><span data-stu-id="3c9d2-132">String</span></span>|<span data-ttu-id="3c9d2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-133">Key of the entity.</span></span> <span data-ttu-id="3c9d2-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c9d2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c9d2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3c9d2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c9d2-136">DateTimeOffset</span></span>|<span data-ttu-id="3c9d2-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="3c9d2-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c9d2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c9d2-139">createdDateTime</span></span>|<span data-ttu-id="3c9d2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c9d2-140">DateTimeOffset</span></span>|<span data-ttu-id="3c9d2-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-141">DateTime the object was created.</span></span> <span data-ttu-id="3c9d2-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c9d2-143">description</span><span class="sxs-lookup"><span data-stu-id="3c9d2-143">description</span></span>|<span data-ttu-id="3c9d2-144">String</span><span class="sxs-lookup"><span data-stu-id="3c9d2-144">String</span></span>|<span data-ttu-id="3c9d2-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c9d2-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c9d2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3c9d2-147">displayName</span></span>|<span data-ttu-id="3c9d2-148">String</span><span class="sxs-lookup"><span data-stu-id="3c9d2-148">String</span></span>|<span data-ttu-id="3c9d2-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c9d2-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c9d2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c9d2-151">version</span><span class="sxs-lookup"><span data-stu-id="3c9d2-151">version</span></span>|<span data-ttu-id="3c9d2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3c9d2-152">Int32</span></span>|<span data-ttu-id="3c9d2-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-153">Version of the device configuration.</span></span> <span data-ttu-id="3c9d2-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c9d2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c9d2-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="3c9d2-155">omaSettings</span></span>|<span data-ttu-id="3c9d2-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3c9d2-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="3c9d2-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-157">OMA settings.</span></span> <span data-ttu-id="3c9d2-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3c9d2-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c9d2-159">Response</span></span>
<span data-ttu-id="3c9d2-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-160">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c9d2-161">Пример</span><span class="sxs-lookup"><span data-stu-id="3c9d2-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c9d2-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c9d2-162">Request</span></span>
<span data-ttu-id="3c9d2-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3c9d2-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c9d2-164">Response</span></span>
<span data-ttu-id="3c9d2-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c9d2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



