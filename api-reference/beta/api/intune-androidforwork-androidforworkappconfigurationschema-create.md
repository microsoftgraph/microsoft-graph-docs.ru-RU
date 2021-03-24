---
title: Создание объекта androidForWorkAppConfigurationSchema
description: Создание объекта androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f437116abe7a16be72f075ed73d116203e4627fb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141325"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="8e36c-103">Создание объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="8e36c-103">Create androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="8e36c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e36c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e36c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e36c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e36c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e36c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e36c-107">Создание объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8e36c-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e36c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e36c-108">Prerequisites</span></span>
<span data-ttu-id="8e36c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e36c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e36c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e36c-111">Permission type</span></span>|<span data-ttu-id="8e36c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e36c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e36c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e36c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e36c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e36c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e36c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e36c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e36c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e36c-116">Not supported.</span></span>|
|<span data-ttu-id="8e36c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e36c-117">Application</span></span>|<span data-ttu-id="8e36c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e36c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e36c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e36c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="8e36c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8e36c-120">Request headers</span></span>
|<span data-ttu-id="8e36c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e36c-121">Header</span></span>|<span data-ttu-id="8e36c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e36c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e36c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e36c-123">Authorization</span></span>|<span data-ttu-id="8e36c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e36c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e36c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e36c-125">Accept</span></span>|<span data-ttu-id="8e36c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e36c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e36c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e36c-127">Request body</span></span>
<span data-ttu-id="8e36c-128">В тексте запроса добавьте представление объекта androidForWorkAppConfigurationSchema в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e36c-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="8e36c-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="8e36c-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="8e36c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e36c-130">Property</span></span>|<span data-ttu-id="8e36c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e36c-131">Type</span></span>|<span data-ttu-id="8e36c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e36c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e36c-133">id</span><span class="sxs-lookup"><span data-stu-id="8e36c-133">id</span></span>|<span data-ttu-id="8e36c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8e36c-134">String</span></span>|<span data-ttu-id="8e36c-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="8e36c-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="8e36c-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="8e36c-136">exampleJson</span></span>|<span data-ttu-id="8e36c-137">Binary</span><span class="sxs-lookup"><span data-stu-id="8e36c-137">Binary</span></span>|<span data-ttu-id="8e36c-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="8e36c-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="8e36c-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="8e36c-139">schemaItems</span></span>|<span data-ttu-id="8e36c-140">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="8e36c-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="8e36c-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="8e36c-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="8e36c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e36c-142">Response</span></span>
<span data-ttu-id="8e36c-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e36c-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e36c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8e36c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e36c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e36c-145">Request</span></span>
<span data-ttu-id="8e36c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e36c-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="8e36c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e36c-147">Response</span></span>
<span data-ttu-id="8e36c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e36c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




