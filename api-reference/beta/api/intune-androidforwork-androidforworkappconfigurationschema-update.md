---
title: Обновление объекта androidForWorkAppConfigurationSchema
description: Обновление свойств объекта androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72b3847c7e12137b2b04e160ad9d3b41e16ac454
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418300"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="9a58e-103">Обновление объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="9a58e-103">Update androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="9a58e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a58e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a58e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a58e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a58e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a58e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a58e-107">Обновление свойств объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="9a58e-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a58e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9a58e-108">Prerequisites</span></span>
<span data-ttu-id="9a58e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a58e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a58e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a58e-111">Permission type</span></span>|<span data-ttu-id="9a58e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a58e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a58e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a58e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a58e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a58e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a58e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a58e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a58e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a58e-116">Not supported.</span></span>|
|<span data-ttu-id="9a58e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9a58e-117">Application</span></span>|<span data-ttu-id="9a58e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a58e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a58e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a58e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="9a58e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a58e-120">Request headers</span></span>
|<span data-ttu-id="9a58e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a58e-121">Header</span></span>|<span data-ttu-id="9a58e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a58e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a58e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a58e-123">Authorization</span></span>|<span data-ttu-id="9a58e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a58e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a58e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a58e-125">Accept</span></span>|<span data-ttu-id="9a58e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a58e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a58e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a58e-127">Request body</span></span>
<span data-ttu-id="9a58e-128">В тексте запроса добавьте представление объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a58e-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="9a58e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="9a58e-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="9a58e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a58e-130">Property</span></span>|<span data-ttu-id="9a58e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9a58e-131">Type</span></span>|<span data-ttu-id="9a58e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9a58e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a58e-133">id</span><span class="sxs-lookup"><span data-stu-id="9a58e-133">id</span></span>|<span data-ttu-id="9a58e-134">String</span><span class="sxs-lookup"><span data-stu-id="9a58e-134">String</span></span>|<span data-ttu-id="9a58e-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="9a58e-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="9a58e-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="9a58e-136">exampleJson</span></span>|<span data-ttu-id="9a58e-137">Binary</span><span class="sxs-lookup"><span data-stu-id="9a58e-137">Binary</span></span>|<span data-ttu-id="9a58e-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="9a58e-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="9a58e-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="9a58e-139">schemaItems</span></span>|<span data-ttu-id="9a58e-140">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="9a58e-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="9a58e-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="9a58e-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="9a58e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a58e-142">Response</span></span>
<span data-ttu-id="9a58e-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a58e-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a58e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9a58e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a58e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a58e-145">Request</span></span>
<span data-ttu-id="9a58e-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a58e-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9a58e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a58e-147">Response</span></span>
<span data-ttu-id="9a58e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a58e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



