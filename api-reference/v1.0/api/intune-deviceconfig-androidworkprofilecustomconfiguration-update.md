---
title: Обновление Андроидворкпрофилекустомконфигуратион
description: Обновление свойств объекта Андроидворкпрофилекустомконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5a7e7183f2616278569cb595fa443227711da70
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357558"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="4bef4-103">Обновление Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4bef4-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="4bef4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bef4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bef4-105">Обновление свойств объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4bef4-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bef4-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4bef4-106">Prerequisites</span></span>
<span data-ttu-id="4bef4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bef4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bef4-109">Permission type</span></span>|<span data-ttu-id="4bef4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bef4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bef4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bef4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4bef4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bef4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bef4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bef4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bef4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bef4-114">Not supported.</span></span>|
|<span data-ttu-id="4bef4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bef4-115">Application</span></span>|<span data-ttu-id="4bef4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bef4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bef4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bef4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4bef4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bef4-118">Request headers</span></span>
|<span data-ttu-id="4bef4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bef4-119">Header</span></span>|<span data-ttu-id="4bef4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4bef4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bef4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bef4-121">Authorization</span></span>|<span data-ttu-id="4bef4-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bef4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bef4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4bef4-123">Accept</span></span>|<span data-ttu-id="4bef4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4bef4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bef4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bef4-125">Request body</span></span>
<span data-ttu-id="4bef4-126">В тексте запроса добавьте представление объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bef4-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="4bef4-127">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bef4-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="4bef4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bef4-128">Property</span></span>|<span data-ttu-id="4bef4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4bef4-129">Type</span></span>|<span data-ttu-id="4bef4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4bef4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bef4-131">id</span><span class="sxs-lookup"><span data-stu-id="4bef4-131">id</span></span>|<span data-ttu-id="4bef4-132">String</span><span class="sxs-lookup"><span data-stu-id="4bef4-132">String</span></span>|<span data-ttu-id="4bef4-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4bef4-133">Key of the entity.</span></span> <span data-ttu-id="4bef4-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bef4-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bef4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bef4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4bef4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bef4-136">DateTimeOffset</span></span>|<span data-ttu-id="4bef4-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4bef4-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4bef4-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bef4-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bef4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bef4-139">createdDateTime</span></span>|<span data-ttu-id="4bef4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bef4-140">DateTimeOffset</span></span>|<span data-ttu-id="4bef4-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4bef4-141">DateTime the object was created.</span></span> <span data-ttu-id="4bef4-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bef4-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bef4-143">description</span><span class="sxs-lookup"><span data-stu-id="4bef4-143">description</span></span>|<span data-ttu-id="4bef4-144">String</span><span class="sxs-lookup"><span data-stu-id="4bef4-144">String</span></span>|<span data-ttu-id="4bef4-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bef4-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4bef4-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bef4-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bef4-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4bef4-147">displayName</span></span>|<span data-ttu-id="4bef4-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4bef4-148">String</span></span>|<span data-ttu-id="4bef4-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bef4-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4bef4-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bef4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bef4-151">version</span><span class="sxs-lookup"><span data-stu-id="4bef4-151">version</span></span>|<span data-ttu-id="4bef4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4bef4-152">Int32</span></span>|<span data-ttu-id="4bef4-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bef4-153">Version of the device configuration.</span></span> <span data-ttu-id="4bef4-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bef4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bef4-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4bef4-155">omaSettings</span></span>|<span data-ttu-id="4bef4-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4bef4-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="4bef4-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="4bef4-157">OMA settings.</span></span> <span data-ttu-id="4bef4-158">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4bef4-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4bef4-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bef4-159">Response</span></span>
<span data-ttu-id="4bef4-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4bef4-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bef4-161">Пример</span><span class="sxs-lookup"><span data-stu-id="4bef4-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bef4-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bef4-162">Request</span></span>
<span data-ttu-id="4bef4-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bef4-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4bef4-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bef4-164">Response</span></span>
<span data-ttu-id="4bef4-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bef4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




