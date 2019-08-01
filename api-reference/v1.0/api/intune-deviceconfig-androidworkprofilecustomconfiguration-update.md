---
title: Обновление Андроидворкпрофилекустомконфигуратион
description: Обновление свойств объекта Андроидворкпрофилекустомконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 668304adc0b3dcdfab076603767c1d46e4198d21
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019480"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="2cc83-103">Обновление Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2cc83-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="2cc83-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc83-105">Обновление свойств объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2cc83-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cc83-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2cc83-106">Prerequisites</span></span>
<span data-ttu-id="2cc83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc83-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cc83-109">Permission type</span></span>|<span data-ttu-id="2cc83-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cc83-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc83-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cc83-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc83-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc83-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cc83-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cc83-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc83-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc83-114">Not supported.</span></span>|
|<span data-ttu-id="2cc83-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cc83-115">Application</span></span>|<span data-ttu-id="2cc83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc83-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc83-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cc83-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2cc83-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cc83-118">Request headers</span></span>
|<span data-ttu-id="2cc83-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cc83-119">Header</span></span>|<span data-ttu-id="2cc83-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2cc83-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cc83-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cc83-121">Authorization</span></span>|<span data-ttu-id="2cc83-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cc83-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cc83-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2cc83-123">Accept</span></span>|<span data-ttu-id="2cc83-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2cc83-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc83-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cc83-125">Request body</span></span>
<span data-ttu-id="2cc83-126">В тексте запроса добавьте представление объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cc83-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="2cc83-127">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc83-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="2cc83-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cc83-128">Property</span></span>|<span data-ttu-id="2cc83-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2cc83-129">Type</span></span>|<span data-ttu-id="2cc83-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc83-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc83-131">id</span><span class="sxs-lookup"><span data-stu-id="2cc83-131">id</span></span>|<span data-ttu-id="2cc83-132">String</span><span class="sxs-lookup"><span data-stu-id="2cc83-132">String</span></span>|<span data-ttu-id="2cc83-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2cc83-133">Key of the entity.</span></span> <span data-ttu-id="2cc83-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc83-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc83-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc83-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2cc83-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc83-136">DateTimeOffset</span></span>|<span data-ttu-id="2cc83-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2cc83-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2cc83-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc83-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc83-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc83-139">createdDateTime</span></span>|<span data-ttu-id="2cc83-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc83-140">DateTimeOffset</span></span>|<span data-ttu-id="2cc83-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2cc83-141">DateTime the object was created.</span></span> <span data-ttu-id="2cc83-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc83-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc83-143">description</span><span class="sxs-lookup"><span data-stu-id="2cc83-143">description</span></span>|<span data-ttu-id="2cc83-144">String</span><span class="sxs-lookup"><span data-stu-id="2cc83-144">String</span></span>|<span data-ttu-id="2cc83-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc83-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2cc83-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc83-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc83-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2cc83-147">displayName</span></span>|<span data-ttu-id="2cc83-148">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc83-148">String</span></span>|<span data-ttu-id="2cc83-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc83-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2cc83-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2cc83-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc83-151">version</span><span class="sxs-lookup"><span data-stu-id="2cc83-151">version</span></span>|<span data-ttu-id="2cc83-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2cc83-152">Int32</span></span>|<span data-ttu-id="2cc83-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc83-153">Version of the device configuration.</span></span> <span data-ttu-id="2cc83-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc83-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc83-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="2cc83-155">omaSettings</span></span>|<span data-ttu-id="2cc83-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2cc83-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="2cc83-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="2cc83-157">OMA settings.</span></span> <span data-ttu-id="2cc83-158">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2cc83-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2cc83-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cc83-159">Response</span></span>
<span data-ttu-id="2cc83-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2cc83-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc83-161">Пример</span><span class="sxs-lookup"><span data-stu-id="2cc83-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cc83-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cc83-162">Request</span></span>
<span data-ttu-id="2cc83-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cc83-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2cc83-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc83-164">Response</span></span>
<span data-ttu-id="2cc83-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cc83-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



