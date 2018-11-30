---
title: Создание объекта windows10CustomConfiguration
description: Создание объекта windows10CustomConfiguration.
ms.openlocfilehash: c7c180b26cd5e25aba9ff36d0190ab455000f839
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026542"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="c7250-103">Создание объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7250-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="c7250-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c7250-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7250-105">Создание объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-105">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7250-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c7250-106">Prerequisites</span></span>
<span data-ttu-id="c7250-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7250-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7250-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7250-109">Permission type</span></span>|<span data-ttu-id="c7250-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7250-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7250-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7250-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7250-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7250-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7250-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7250-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7250-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7250-114">Not supported.</span></span>|
|<span data-ttu-id="c7250-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7250-115">Application</span></span>|<span data-ttu-id="c7250-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7250-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7250-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7250-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7250-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7250-118">Request headers</span></span>
|<span data-ttu-id="c7250-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7250-119">Header</span></span>|<span data-ttu-id="c7250-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c7250-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7250-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7250-121">Authorization</span></span>|<span data-ttu-id="c7250-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7250-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7250-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c7250-123">Accept</span></span>|<span data-ttu-id="c7250-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c7250-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7250-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7250-125">Request body</span></span>
<span data-ttu-id="c7250-126">В тексте запроса добавьте представление объекта windows10CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7250-126">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="c7250-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7250-127">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="c7250-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7250-128">Property</span></span>|<span data-ttu-id="c7250-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c7250-129">Type</span></span>|<span data-ttu-id="c7250-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c7250-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7250-131">id</span><span class="sxs-lookup"><span data-stu-id="c7250-131">id</span></span>|<span data-ttu-id="c7250-132">String</span><span class="sxs-lookup"><span data-stu-id="c7250-132">String</span></span>|<span data-ttu-id="c7250-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7250-133">Key of the entity.</span></span> <span data-ttu-id="c7250-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7250-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7250-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c7250-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7250-136">DateTimeOffset</span></span>|<span data-ttu-id="c7250-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7250-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c7250-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7250-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7250-139">createdDateTime</span></span>|<span data-ttu-id="c7250-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7250-140">DateTimeOffset</span></span>|<span data-ttu-id="c7250-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c7250-141">DateTime the object was created.</span></span> <span data-ttu-id="c7250-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7250-143">описание</span><span class="sxs-lookup"><span data-stu-id="c7250-143">description</span></span>|<span data-ttu-id="c7250-144">String</span><span class="sxs-lookup"><span data-stu-id="c7250-144">String</span></span>|<span data-ttu-id="c7250-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7250-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7250-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7250-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c7250-147">displayName</span></span>|<span data-ttu-id="c7250-148">String</span><span class="sxs-lookup"><span data-stu-id="c7250-148">String</span></span>|<span data-ttu-id="c7250-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7250-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7250-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7250-151">version</span><span class="sxs-lookup"><span data-stu-id="c7250-151">version</span></span>|<span data-ttu-id="c7250-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c7250-152">Int32</span></span>|<span data-ttu-id="c7250-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7250-153">Version of the device configuration.</span></span> <span data-ttu-id="c7250-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7250-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7250-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c7250-155">omaSettings</span></span>|<span data-ttu-id="c7250-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7250-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c7250-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="c7250-157">OMA settings.</span></span> <span data-ttu-id="c7250-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c7250-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c7250-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7250-159">Response</span></span>
<span data-ttu-id="c7250-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7250-160">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7250-161">Пример</span><span class="sxs-lookup"><span data-stu-id="c7250-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7250-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7250-162">Request</span></span>
<span data-ttu-id="c7250-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7250-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="c7250-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7250-164">Response</span></span>
<span data-ttu-id="c7250-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c7250-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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



