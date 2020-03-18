---
title: Обновление Андроидманажедстореаппконфигуратионсчема
description: Обновление свойств объекта Андроидманажедстореаппконфигуратионсчема.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95d4da95613f33682d56df2c91a5e3a149d39a08
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762408"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="fe07a-103">Обновление Андроидманажедстореаппконфигуратионсчема</span><span class="sxs-lookup"><span data-stu-id="fe07a-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="fe07a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe07a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe07a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe07a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe07a-106">Обновление свойств объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="fe07a-106">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe07a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe07a-107">Prerequisites</span></span>
<span data-ttu-id="fe07a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe07a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe07a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe07a-110">Permission type</span></span>|<span data-ttu-id="fe07a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe07a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe07a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe07a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe07a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe07a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe07a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe07a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe07a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe07a-115">Not supported.</span></span>|
|<span data-ttu-id="fe07a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe07a-116">Application</span></span>|<span data-ttu-id="fe07a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe07a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe07a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe07a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="fe07a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe07a-119">Request headers</span></span>
|<span data-ttu-id="fe07a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe07a-120">Header</span></span>|<span data-ttu-id="fe07a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fe07a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe07a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe07a-122">Authorization</span></span>|<span data-ttu-id="fe07a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe07a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe07a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe07a-124">Accept</span></span>|<span data-ttu-id="fe07a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe07a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe07a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe07a-126">Request body</span></span>
<span data-ttu-id="fe07a-127">В тексте запроса добавьте представление объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe07a-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="fe07a-128">В следующей таблице приведены свойства, необходимые при создании [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fe07a-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="fe07a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe07a-129">Property</span></span>|<span data-ttu-id="fe07a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fe07a-130">Type</span></span>|<span data-ttu-id="fe07a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fe07a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe07a-132">id</span><span class="sxs-lookup"><span data-stu-id="fe07a-132">id</span></span>|<span data-ttu-id="fe07a-133">String</span><span class="sxs-lookup"><span data-stu-id="fe07a-133">String</span></span>|<span data-ttu-id="fe07a-134">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="fe07a-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="fe07a-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="fe07a-135">exampleJson</span></span>|<span data-ttu-id="fe07a-136">Binary</span><span class="sxs-lookup"><span data-stu-id="fe07a-136">Binary</span></span>|<span data-ttu-id="fe07a-137">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="fe07a-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="fe07a-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="fe07a-138">schemaItems</span></span>|<span data-ttu-id="fe07a-139">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe07a-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="fe07a-140">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="fe07a-140">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="fe07a-141">Он содержит только конфигурацию корневого уровня.</span><span class="sxs-lookup"><span data-stu-id="fe07a-141">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="fe07a-142">нестедсчемаитемс</span><span class="sxs-lookup"><span data-stu-id="fe07a-142">nestedSchemaItems</span></span>|<span data-ttu-id="fe07a-143">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe07a-143">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="fe07a-144">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="fe07a-144">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="fe07a-145">Он содержит плоский список всех конфигураций.</span><span class="sxs-lookup"><span data-stu-id="fe07a-145">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fe07a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe07a-146">Response</span></span>
<span data-ttu-id="fe07a-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe07a-147">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe07a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="fe07a-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe07a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe07a-149">Request</span></span>
<span data-ttu-id="fe07a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe07a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe07a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe07a-151">Response</span></span>
<span data-ttu-id="fe07a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe07a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




