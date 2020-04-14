---
title: Обновление Андроидманажедстореаппконфигуратионсчема
description: Обновление свойств объекта Андроидманажедстореаппконфигуратионсчема.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 399ebecdbed9942ebb5ca828c815aa6ad03befea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395501"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="8e957-103">Обновление Андроидманажедстореаппконфигуратионсчема</span><span class="sxs-lookup"><span data-stu-id="8e957-103">Update androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="8e957-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e957-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e957-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e957-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e957-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e957-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e957-107">Обновление свойств объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="8e957-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e957-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e957-108">Prerequisites</span></span>
<span data-ttu-id="8e957-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e957-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e957-111">Permission type</span></span>|<span data-ttu-id="8e957-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e957-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e957-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e957-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e957-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e957-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e957-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e957-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e957-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e957-116">Not supported.</span></span>|
|<span data-ttu-id="8e957-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8e957-117">Application</span></span>|<span data-ttu-id="8e957-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e957-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e957-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e957-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="8e957-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8e957-120">Request headers</span></span>
|<span data-ttu-id="8e957-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e957-121">Header</span></span>|<span data-ttu-id="8e957-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e957-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e957-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e957-123">Authorization</span></span>|<span data-ttu-id="8e957-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e957-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e957-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e957-125">Accept</span></span>|<span data-ttu-id="8e957-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e957-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e957-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e957-127">Request body</span></span>
<span data-ttu-id="8e957-128">В тексте запроса добавьте представление объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e957-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="8e957-129">В следующей таблице приведены свойства, необходимые при создании [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8e957-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="8e957-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e957-130">Property</span></span>|<span data-ttu-id="8e957-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e957-131">Type</span></span>|<span data-ttu-id="8e957-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e957-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e957-133">id</span><span class="sxs-lookup"><span data-stu-id="8e957-133">id</span></span>|<span data-ttu-id="8e957-134">String</span><span class="sxs-lookup"><span data-stu-id="8e957-134">String</span></span>|<span data-ttu-id="8e957-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="8e957-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="8e957-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="8e957-136">exampleJson</span></span>|<span data-ttu-id="8e957-137">Binary</span><span class="sxs-lookup"><span data-stu-id="8e957-137">Binary</span></span>|<span data-ttu-id="8e957-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="8e957-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="8e957-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="8e957-139">schemaItems</span></span>|<span data-ttu-id="8e957-140">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="8e957-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="8e957-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="8e957-141">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="8e957-142">Он содержит только конфигурацию корневого уровня.</span><span class="sxs-lookup"><span data-stu-id="8e957-142">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="8e957-143">нестедсчемаитемс</span><span class="sxs-lookup"><span data-stu-id="8e957-143">nestedSchemaItems</span></span>|<span data-ttu-id="8e957-144">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="8e957-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="8e957-145">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="8e957-145">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="8e957-146">Он содержит плоский список всех конфигураций.</span><span class="sxs-lookup"><span data-stu-id="8e957-146">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="8e957-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e957-147">Response</span></span>
<span data-ttu-id="8e957-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e957-148">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e957-149">Пример</span><span class="sxs-lookup"><span data-stu-id="8e957-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e957-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e957-150">Request</span></span>
<span data-ttu-id="8e957-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e957-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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

### <a name="response"></a><span data-ttu-id="8e957-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e957-152">Response</span></span>
<span data-ttu-id="8e957-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e957-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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



