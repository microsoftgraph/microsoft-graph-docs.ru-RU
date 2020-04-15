---
title: Обновление Андроидворкпрофилекустомконфигуратион
description: Обновление свойств объекта Андроидворкпрофилекустомконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61800aadbb996a64131798e7394e4f581d2b3b6e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401170"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="969fd-103">Обновление Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="969fd-103">Update androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="969fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="969fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="969fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="969fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="969fd-106">Обновление свойств объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="969fd-106">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="969fd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="969fd-107">Prerequisites</span></span>
<span data-ttu-id="969fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="969fd-110">Permission type</span></span>|<span data-ttu-id="969fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="969fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="969fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="969fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="969fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="969fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969fd-115">Not supported.</span></span>|
|<span data-ttu-id="969fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="969fd-116">Application</span></span>|<span data-ttu-id="969fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="969fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="969fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="969fd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="969fd-119">Request headers</span></span>
|<span data-ttu-id="969fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="969fd-120">Header</span></span>|<span data-ttu-id="969fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="969fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="969fd-122">Authorization</span></span>|<span data-ttu-id="969fd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="969fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969fd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="969fd-124">Accept</span></span>|<span data-ttu-id="969fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="969fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969fd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="969fd-126">Request body</span></span>
<span data-ttu-id="969fd-127">В тексте запроса добавьте представление объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="969fd-127">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="969fd-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969fd-128">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="969fd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="969fd-129">Property</span></span>|<span data-ttu-id="969fd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="969fd-130">Type</span></span>|<span data-ttu-id="969fd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="969fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="969fd-132">id</span><span class="sxs-lookup"><span data-stu-id="969fd-132">id</span></span>|<span data-ttu-id="969fd-133">String</span><span class="sxs-lookup"><span data-stu-id="969fd-133">String</span></span>|<span data-ttu-id="969fd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="969fd-134">Key of the entity.</span></span> <span data-ttu-id="969fd-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969fd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="969fd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="969fd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="969fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969fd-137">DateTimeOffset</span></span>|<span data-ttu-id="969fd-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="969fd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="969fd-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969fd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="969fd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="969fd-140">createdDateTime</span></span>|<span data-ttu-id="969fd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969fd-141">DateTimeOffset</span></span>|<span data-ttu-id="969fd-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="969fd-142">DateTime the object was created.</span></span> <span data-ttu-id="969fd-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969fd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="969fd-144">description</span><span class="sxs-lookup"><span data-stu-id="969fd-144">description</span></span>|<span data-ttu-id="969fd-145">String</span><span class="sxs-lookup"><span data-stu-id="969fd-145">String</span></span>|<span data-ttu-id="969fd-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="969fd-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="969fd-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969fd-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="969fd-148">displayName</span><span class="sxs-lookup"><span data-stu-id="969fd-148">displayName</span></span>|<span data-ttu-id="969fd-149">Строка</span><span class="sxs-lookup"><span data-stu-id="969fd-149">String</span></span>|<span data-ttu-id="969fd-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="969fd-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="969fd-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="969fd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="969fd-152">version</span><span class="sxs-lookup"><span data-stu-id="969fd-152">version</span></span>|<span data-ttu-id="969fd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="969fd-153">Int32</span></span>|<span data-ttu-id="969fd-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="969fd-154">Version of the device configuration.</span></span> <span data-ttu-id="969fd-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969fd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="969fd-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="969fd-156">omaSettings</span></span>|<span data-ttu-id="969fd-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="969fd-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="969fd-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="969fd-158">OMA settings.</span></span> <span data-ttu-id="969fd-159">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="969fd-159">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="969fd-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="969fd-160">Response</span></span>
<span data-ttu-id="969fd-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="969fd-161">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969fd-162">Пример</span><span class="sxs-lookup"><span data-stu-id="969fd-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="969fd-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="969fd-163">Request</span></span>
<span data-ttu-id="969fd-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="969fd-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="969fd-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="969fd-165">Response</span></span>
<span data-ttu-id="969fd-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="969fd-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






