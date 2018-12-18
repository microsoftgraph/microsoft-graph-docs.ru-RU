---
title: Обновление androidWorkProfileCustomConfiguration
description: Обновление свойства объекта androidWorkProfileCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 1293ca362719440871576c3976f184ed60e37e43
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302368"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="e5df5-103">Обновление androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5df5-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="e5df5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e5df5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5df5-105">Обновление свойства объекта [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e5df5-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5df5-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5df5-106">Prerequisites</span></span>
<span data-ttu-id="e5df5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5df5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5df5-109">Permission type</span></span>|<span data-ttu-id="e5df5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5df5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5df5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5df5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5df5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5df5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5df5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5df5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5df5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5df5-114">Not supported.</span></span>|
|<span data-ttu-id="e5df5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5df5-115">Application</span></span>|<span data-ttu-id="e5df5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5df5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5df5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5df5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e5df5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5df5-118">Request headers</span></span>
|<span data-ttu-id="e5df5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5df5-119">Header</span></span>|<span data-ttu-id="e5df5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e5df5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5df5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5df5-121">Authorization</span></span>|<span data-ttu-id="e5df5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e5df5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5df5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e5df5-123">Accept</span></span>|<span data-ttu-id="e5df5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e5df5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5df5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5df5-125">Request body</span></span>
<span data-ttu-id="e5df5-126">В тексте запроса укажите представление JSON для объекта [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e5df5-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="e5df5-127">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="e5df5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5df5-128">Property</span></span>|<span data-ttu-id="e5df5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e5df5-129">Type</span></span>|<span data-ttu-id="e5df5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e5df5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5df5-131">id</span><span class="sxs-lookup"><span data-stu-id="e5df5-131">id</span></span>|<span data-ttu-id="e5df5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e5df5-132">String</span></span>|<span data-ttu-id="e5df5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5df5-133">Key of the entity.</span></span> <span data-ttu-id="e5df5-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5df5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5df5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e5df5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5df5-136">DateTimeOffset</span></span>|<span data-ttu-id="e5df5-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e5df5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="e5df5-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5df5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5df5-139">createdDateTime</span></span>|<span data-ttu-id="e5df5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5df5-140">DateTimeOffset</span></span>|<span data-ttu-id="e5df5-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e5df5-141">DateTime the object was created.</span></span> <span data-ttu-id="e5df5-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5df5-143">описание</span><span class="sxs-lookup"><span data-stu-id="e5df5-143">description</span></span>|<span data-ttu-id="e5df5-144">Строка</span><span class="sxs-lookup"><span data-stu-id="e5df5-144">String</span></span>|<span data-ttu-id="e5df5-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5df5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5df5-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5df5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e5df5-147">displayName</span></span>|<span data-ttu-id="e5df5-148">Строка</span><span class="sxs-lookup"><span data-stu-id="e5df5-148">String</span></span>|<span data-ttu-id="e5df5-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5df5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5df5-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5df5-151">version</span><span class="sxs-lookup"><span data-stu-id="e5df5-151">version</span></span>|<span data-ttu-id="e5df5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e5df5-152">Int32</span></span>|<span data-ttu-id="e5df5-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5df5-153">Version of the device configuration.</span></span> <span data-ttu-id="e5df5-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5df5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5df5-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e5df5-155">omaSettings</span></span>|<span data-ttu-id="e5df5-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5df5-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="e5df5-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="e5df5-157">OMA settings.</span></span> <span data-ttu-id="e5df5-158">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e5df5-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e5df5-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5df5-159">Response</span></span>
<span data-ttu-id="e5df5-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5df5-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5df5-161">Пример</span><span class="sxs-lookup"><span data-stu-id="e5df5-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5df5-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5df5-162">Request</span></span>
<span data-ttu-id="e5df5-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5df5-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5df5-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5df5-164">Response</span></span>
<span data-ttu-id="e5df5-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5df5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



