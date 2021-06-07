---
title: Создание androidWorkProfileCustomConfiguration
description: Создайте новый объект AndroidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bbf81e4004fdccbfa1dbcee9f5ea2df1b8fa8e2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757180"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="b9c76-103">Создание androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9c76-103">Create androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="b9c76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9c76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9c76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9c76-106">Создайте новый [объект AndroidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9c76-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9c76-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9c76-107">Prerequisites</span></span>
<span data-ttu-id="b9c76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c76-110">Permission type</span></span>|<span data-ttu-id="b9c76-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9c76-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9c76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9c76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9c76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c76-115">Not supported.</span></span>|
|<span data-ttu-id="b9c76-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9c76-116">Application</span></span>|<span data-ttu-id="b9c76-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c76-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9c76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b9c76-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b9c76-119">Request headers</span></span>
|<span data-ttu-id="b9c76-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9c76-120">Header</span></span>|<span data-ttu-id="b9c76-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b9c76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c76-122">Authorization</span></span>|<span data-ttu-id="b9c76-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9c76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c76-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b9c76-124">Accept</span></span>|<span data-ttu-id="b9c76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c76-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9c76-126">Request body</span></span>
<span data-ttu-id="b9c76-127">В теле запроса предоставляем представление JSON для объекта AndroidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b9c76-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="b9c76-128">В следующей таблице показаны свойства, необходимые при создании androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b9c76-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="b9c76-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9c76-129">Property</span></span>|<span data-ttu-id="b9c76-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b9c76-130">Type</span></span>|<span data-ttu-id="b9c76-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9c76-132">id</span><span class="sxs-lookup"><span data-stu-id="b9c76-132">id</span></span>|<span data-ttu-id="b9c76-133">String</span><span class="sxs-lookup"><span data-stu-id="b9c76-133">String</span></span>|<span data-ttu-id="b9c76-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9c76-134">Key of the entity.</span></span> <span data-ttu-id="b9c76-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9c76-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9c76-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c76-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b9c76-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c76-137">DateTimeOffset</span></span>|<span data-ttu-id="b9c76-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b9c76-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b9c76-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9c76-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9c76-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c76-140">createdDateTime</span></span>|<span data-ttu-id="b9c76-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c76-141">DateTimeOffset</span></span>|<span data-ttu-id="b9c76-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b9c76-142">DateTime the object was created.</span></span> <span data-ttu-id="b9c76-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9c76-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9c76-144">description</span><span class="sxs-lookup"><span data-stu-id="b9c76-144">description</span></span>|<span data-ttu-id="b9c76-145">String</span><span class="sxs-lookup"><span data-stu-id="b9c76-145">String</span></span>|<span data-ttu-id="b9c76-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9c76-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9c76-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9c76-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9c76-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b9c76-148">displayName</span></span>|<span data-ttu-id="b9c76-149">String</span><span class="sxs-lookup"><span data-stu-id="b9c76-149">String</span></span>|<span data-ttu-id="b9c76-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9c76-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9c76-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9c76-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9c76-152">version</span><span class="sxs-lookup"><span data-stu-id="b9c76-152">version</span></span>|<span data-ttu-id="b9c76-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c76-153">Int32</span></span>|<span data-ttu-id="b9c76-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9c76-154">Version of the device configuration.</span></span> <span data-ttu-id="b9c76-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9c76-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9c76-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="b9c76-156">omaSettings</span></span>|<span data-ttu-id="b9c76-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b9c76-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="b9c76-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="b9c76-158">OMA settings.</span></span> <span data-ttu-id="b9c76-159">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b9c76-159">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b9c76-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9c76-160">Response</span></span>
<span data-ttu-id="b9c76-161">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9c76-161">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c76-162">Пример</span><span class="sxs-lookup"><span data-stu-id="b9c76-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9c76-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9c76-163">Request</span></span>
<span data-ttu-id="b9c76-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9c76-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b9c76-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c76-165">Response</span></span>
<span data-ttu-id="b9c76-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9c76-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 559

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```




