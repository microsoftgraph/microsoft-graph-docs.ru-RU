---
title: Обновление Андроидманажедстореаппконфигуратионсчема
description: Обновление свойств объекта Андроидманажедстореаппконфигуратионсчема.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fbb21182c5e7651252eaed7098fb2f1aee938a30
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324905"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="1baf4-103">Обновление Андроидманажедстореаппконфигуратионсчема</span><span class="sxs-lookup"><span data-stu-id="1baf4-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="1baf4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1baf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1baf4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1baf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1baf4-106">Обновление свойств объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="1baf4-106">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1baf4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1baf4-107">Prerequisites</span></span>
<span data-ttu-id="1baf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1baf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1baf4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1baf4-110">Permission type</span></span>|<span data-ttu-id="1baf4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1baf4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1baf4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1baf4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1baf4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1baf4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1baf4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1baf4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1baf4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1baf4-115">Not supported.</span></span>|
|<span data-ttu-id="1baf4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1baf4-116">Application</span></span>|<span data-ttu-id="1baf4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1baf4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1baf4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1baf4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="1baf4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1baf4-119">Request headers</span></span>
|<span data-ttu-id="1baf4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1baf4-120">Header</span></span>|<span data-ttu-id="1baf4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1baf4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1baf4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1baf4-122">Authorization</span></span>|<span data-ttu-id="1baf4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1baf4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1baf4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1baf4-124">Accept</span></span>|<span data-ttu-id="1baf4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1baf4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1baf4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1baf4-126">Request body</span></span>
<span data-ttu-id="1baf4-127">В тексте запроса добавьте представление объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1baf4-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="1baf4-128">В следующей таблице приведены свойства, необходимые при создании [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1baf4-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="1baf4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1baf4-129">Property</span></span>|<span data-ttu-id="1baf4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1baf4-130">Type</span></span>|<span data-ttu-id="1baf4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1baf4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1baf4-132">id</span><span class="sxs-lookup"><span data-stu-id="1baf4-132">id</span></span>|<span data-ttu-id="1baf4-133">String</span><span class="sxs-lookup"><span data-stu-id="1baf4-133">String</span></span>|<span data-ttu-id="1baf4-134">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="1baf4-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="1baf4-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="1baf4-135">exampleJson</span></span>|<span data-ttu-id="1baf4-136">Binary</span><span class="sxs-lookup"><span data-stu-id="1baf4-136">Binary</span></span>|<span data-ttu-id="1baf4-137">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="1baf4-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="1baf4-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="1baf4-138">schemaItems</span></span>|<span data-ttu-id="1baf4-139">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="1baf4-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="1baf4-140">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="1baf4-140">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="1baf4-141">Он содержит только конфигурацию корневого уровня.</span><span class="sxs-lookup"><span data-stu-id="1baf4-141">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="1baf4-142">нестедсчемаитемс</span><span class="sxs-lookup"><span data-stu-id="1baf4-142">nestedSchemaItems</span></span>|<span data-ttu-id="1baf4-143">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="1baf4-143">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="1baf4-144">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="1baf4-144">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="1baf4-145">Он содержит плоский список всех конфигураций.</span><span class="sxs-lookup"><span data-stu-id="1baf4-145">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="1baf4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1baf4-146">Response</span></span>
<span data-ttu-id="1baf4-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1baf4-147">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1baf4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="1baf4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="1baf4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1baf4-149">Request</span></span>
<span data-ttu-id="1baf4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1baf4-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1baf4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1baf4-151">Response</span></span>
<span data-ttu-id="1baf4-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1baf4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






