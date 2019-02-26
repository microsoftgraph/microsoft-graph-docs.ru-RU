---
title: Обновление Андроидворкпрофилекустомконфигуратион
description: Обновление свойств объекта Андроидворкпрофилекустомконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8da7ceee5827bc97e628a8991682f951daf40964
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256751"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="ab6d3-103">Обновление Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ab6d3-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="ab6d3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab6d3-105">Обновление свойств объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab6d3-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab6d3-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab6d3-106">Prerequisites</span></span>
<span data-ttu-id="ab6d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ab6d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab6d3-109">Permission type</span></span>|<span data-ttu-id="ab6d3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab6d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab6d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab6d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab6d3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab6d3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab6d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab6d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab6d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-114">Not supported.</span></span>|
|<span data-ttu-id="ab6d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab6d3-115">Application</span></span>|<span data-ttu-id="ab6d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab6d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab6d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab6d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab6d3-118">Request headers</span></span>
|<span data-ttu-id="ab6d3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab6d3-119">Header</span></span>|<span data-ttu-id="ab6d3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ab6d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab6d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab6d3-121">Authorization</span></span>|<span data-ttu-id="ab6d3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab6d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab6d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ab6d3-123">Accept</span></span>|<span data-ttu-id="ab6d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab6d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab6d3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab6d3-125">Request body</span></span>
<span data-ttu-id="ab6d3-126">В тексте запроса добавьте представление объекта [Андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="ab6d3-127">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="ab6d3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab6d3-128">Property</span></span>|<span data-ttu-id="ab6d3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ab6d3-129">Type</span></span>|<span data-ttu-id="ab6d3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ab6d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab6d3-131">id</span><span class="sxs-lookup"><span data-stu-id="ab6d3-131">id</span></span>|<span data-ttu-id="ab6d3-132">String</span><span class="sxs-lookup"><span data-stu-id="ab6d3-132">String</span></span>|<span data-ttu-id="ab6d3-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-133">Key of the entity.</span></span> <span data-ttu-id="ab6d3-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab6d3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab6d3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ab6d3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab6d3-136">DateTimeOffset</span></span>|<span data-ttu-id="ab6d3-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ab6d3-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab6d3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab6d3-139">createdDateTime</span></span>|<span data-ttu-id="ab6d3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab6d3-140">DateTimeOffset</span></span>|<span data-ttu-id="ab6d3-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-141">DateTime the object was created.</span></span> <span data-ttu-id="ab6d3-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab6d3-143">description</span><span class="sxs-lookup"><span data-stu-id="ab6d3-143">description</span></span>|<span data-ttu-id="ab6d3-144">String</span><span class="sxs-lookup"><span data-stu-id="ab6d3-144">String</span></span>|<span data-ttu-id="ab6d3-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab6d3-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab6d3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ab6d3-147">displayName</span></span>|<span data-ttu-id="ab6d3-148">String</span><span class="sxs-lookup"><span data-stu-id="ab6d3-148">String</span></span>|<span data-ttu-id="ab6d3-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab6d3-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab6d3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab6d3-151">version</span><span class="sxs-lookup"><span data-stu-id="ab6d3-151">version</span></span>|<span data-ttu-id="ab6d3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ab6d3-152">Int32</span></span>|<span data-ttu-id="ab6d3-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-153">Version of the device configuration.</span></span> <span data-ttu-id="ab6d3-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab6d3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab6d3-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ab6d3-155">omaSettings</span></span>|<span data-ttu-id="ab6d3-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ab6d3-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ab6d3-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-157">OMA settings.</span></span> <span data-ttu-id="ab6d3-158">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ab6d3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab6d3-159">Response</span></span>
<span data-ttu-id="ab6d3-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab6d3-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ab6d3-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab6d3-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab6d3-162">Request</span></span>
<span data-ttu-id="ab6d3-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab6d3-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab6d3-164">Response</span></span>
<span data-ttu-id="ab6d3-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab6d3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



