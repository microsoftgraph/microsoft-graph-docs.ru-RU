---
title: Создание Андроидворкпрофилекустомконфигуратион
description: Создание нового объекта Андроидворкпрофилекустомконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7016f6689d18a6b6b633926c93530cc40e2629d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985407"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="5c6f1-103">Создание Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5c6f1-103">Create androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="5c6f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c6f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c6f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c6f1-106">Создание нового объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5c6f1-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c6f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c6f1-107">Prerequisites</span></span>
<span data-ttu-id="5c6f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c6f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c6f1-110">Permission type</span></span>|<span data-ttu-id="5c6f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c6f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c6f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c6f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c6f1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6f1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c6f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c6f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c6f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-115">Not supported.</span></span>|
|<span data-ttu-id="5c6f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c6f1-116">Application</span></span>|<span data-ttu-id="5c6f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c6f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c6f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c6f1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c6f1-119">Request headers</span></span>
|<span data-ttu-id="5c6f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c6f1-120">Header</span></span>|<span data-ttu-id="5c6f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c6f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c6f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c6f1-122">Authorization</span></span>|<span data-ttu-id="5c6f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c6f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c6f1-124">Accept</span></span>|<span data-ttu-id="5c6f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c6f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c6f1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c6f1-126">Request body</span></span>
<span data-ttu-id="5c6f1-127">В тексте запроса добавьте представление объекта Андроидворкпрофилекустомконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="5c6f1-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилекустомконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="5c6f1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c6f1-129">Property</span></span>|<span data-ttu-id="5c6f1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c6f1-130">Type</span></span>|<span data-ttu-id="5c6f1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c6f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c6f1-132">id</span><span class="sxs-lookup"><span data-stu-id="5c6f1-132">id</span></span>|<span data-ttu-id="5c6f1-133">String</span><span class="sxs-lookup"><span data-stu-id="5c6f1-133">String</span></span>|<span data-ttu-id="5c6f1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-134">Key of the entity.</span></span> <span data-ttu-id="5c6f1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c6f1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c6f1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c6f1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c6f1-137">DateTimeOffset</span></span>|<span data-ttu-id="5c6f1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c6f1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c6f1-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c6f1-140">createdDateTime</span></span>|<span data-ttu-id="5c6f1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c6f1-141">DateTimeOffset</span></span>|<span data-ttu-id="5c6f1-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-142">DateTime the object was created.</span></span> <span data-ttu-id="5c6f1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c6f1-144">description</span><span class="sxs-lookup"><span data-stu-id="5c6f1-144">description</span></span>|<span data-ttu-id="5c6f1-145">String</span><span class="sxs-lookup"><span data-stu-id="5c6f1-145">String</span></span>|<span data-ttu-id="5c6f1-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c6f1-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c6f1-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5c6f1-148">displayName</span></span>|<span data-ttu-id="5c6f1-149">String</span><span class="sxs-lookup"><span data-stu-id="5c6f1-149">String</span></span>|<span data-ttu-id="5c6f1-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c6f1-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c6f1-152">version</span><span class="sxs-lookup"><span data-stu-id="5c6f1-152">version</span></span>|<span data-ttu-id="5c6f1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5c6f1-153">Int32</span></span>|<span data-ttu-id="5c6f1-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-154">Version of the device configuration.</span></span> <span data-ttu-id="5c6f1-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6f1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c6f1-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="5c6f1-156">omaSettings</span></span>|<span data-ttu-id="5c6f1-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5c6f1-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="5c6f1-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-158">OMA settings.</span></span> <span data-ttu-id="5c6f1-159">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-159">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5c6f1-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c6f1-160">Response</span></span>
<span data-ttu-id="5c6f1-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-161">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c6f1-162">Пример</span><span class="sxs-lookup"><span data-stu-id="5c6f1-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c6f1-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c6f1-163">Request</span></span>
<span data-ttu-id="5c6f1-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="5c6f1-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c6f1-165">Response</span></span>
<span data-ttu-id="5c6f1-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c6f1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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









