---
title: Обновление объекта androidForWorkAppConfigurationSchema
description: Обновление свойств объекта androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5e29e3d061f136c6917e23d56052333b869978a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001395"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="8e314-103">Обновление объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="8e314-103">Update androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="8e314-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e314-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e314-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e314-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e314-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e314-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e314-107">Обновление свойств объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8e314-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e314-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e314-108">Prerequisites</span></span>
<span data-ttu-id="8e314-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e314-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e314-111">Permission type</span></span>|<span data-ttu-id="8e314-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e314-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e314-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e314-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e314-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e314-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e314-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e314-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e314-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e314-116">Not supported.</span></span>|
|<span data-ttu-id="8e314-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e314-117">Application</span></span>|<span data-ttu-id="8e314-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e314-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e314-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e314-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="8e314-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8e314-120">Request headers</span></span>
|<span data-ttu-id="8e314-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e314-121">Header</span></span>|<span data-ttu-id="8e314-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e314-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e314-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e314-123">Authorization</span></span>|<span data-ttu-id="8e314-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e314-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e314-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e314-125">Accept</span></span>|<span data-ttu-id="8e314-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e314-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e314-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e314-127">Request body</span></span>
<span data-ttu-id="8e314-128">В тексте запроса добавьте представление объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e314-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="8e314-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8e314-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="8e314-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e314-130">Property</span></span>|<span data-ttu-id="8e314-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e314-131">Type</span></span>|<span data-ttu-id="8e314-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e314-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e314-133">id</span><span class="sxs-lookup"><span data-stu-id="8e314-133">id</span></span>|<span data-ttu-id="8e314-134">String</span><span class="sxs-lookup"><span data-stu-id="8e314-134">String</span></span>|<span data-ttu-id="8e314-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="8e314-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="8e314-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="8e314-136">exampleJson</span></span>|<span data-ttu-id="8e314-137">Binary</span><span class="sxs-lookup"><span data-stu-id="8e314-137">Binary</span></span>|<span data-ttu-id="8e314-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="8e314-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="8e314-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="8e314-139">schemaItems</span></span>|<span data-ttu-id="8e314-140">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="8e314-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="8e314-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="8e314-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="8e314-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e314-142">Response</span></span>
<span data-ttu-id="8e314-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e314-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e314-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8e314-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e314-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e314-145">Request</span></span>
<span data-ttu-id="8e314-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e314-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e314-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e314-147">Response</span></span>
<span data-ttu-id="8e314-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e314-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






