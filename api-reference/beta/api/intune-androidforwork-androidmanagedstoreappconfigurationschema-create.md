---
title: Создание Андроидманажедстореаппконфигуратионсчема
description: Создание нового объекта Андроидманажедстореаппконфигуратионсчема.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0f743d03e9ce915e5d8bd0f31d94593da01c9ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700964"
---
# <a name="create-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="a9bb1-103">Создание Андроидманажедстореаппконфигуратионсчема</span><span class="sxs-lookup"><span data-stu-id="a9bb1-103">Create androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="a9bb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9bb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9bb1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9bb1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9bb1-107">Создание нового объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="a9bb1-107">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9bb1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9bb1-108">Prerequisites</span></span>
<span data-ttu-id="a9bb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9bb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9bb1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9bb1-111">Permission type</span></span>|<span data-ttu-id="a9bb1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9bb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9bb1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9bb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9bb1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9bb1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9bb1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9bb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9bb1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-116">Not supported.</span></span>|
|<span data-ttu-id="a9bb1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9bb1-117">Application</span></span>|<span data-ttu-id="a9bb1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9bb1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9bb1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9bb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="a9bb1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9bb1-120">Request headers</span></span>
|<span data-ttu-id="a9bb1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9bb1-121">Header</span></span>|<span data-ttu-id="a9bb1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9bb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9bb1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9bb1-123">Authorization</span></span>|<span data-ttu-id="a9bb1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9bb1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9bb1-125">Accept</span></span>|<span data-ttu-id="a9bb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9bb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9bb1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9bb1-127">Request body</span></span>
<span data-ttu-id="a9bb1-128">В тексте запроса добавьте представление объекта Андроидманажедстореаппконфигуратионсчема в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfigurationSchema object.</span></span>

<span data-ttu-id="a9bb1-129">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореаппконфигуратионсчема.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfigurationSchema.</span></span>

|<span data-ttu-id="a9bb1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9bb1-130">Property</span></span>|<span data-ttu-id="a9bb1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9bb1-131">Type</span></span>|<span data-ttu-id="a9bb1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9bb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9bb1-133">id</span><span class="sxs-lookup"><span data-stu-id="a9bb1-133">id</span></span>|<span data-ttu-id="a9bb1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a9bb1-134">String</span></span>|<span data-ttu-id="a9bb1-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="a9bb1-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="a9bb1-136">exampleJson</span></span>|<span data-ttu-id="a9bb1-137">Binary</span><span class="sxs-lookup"><span data-stu-id="a9bb1-137">Binary</span></span>|<span data-ttu-id="a9bb1-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="a9bb1-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="a9bb1-139">schemaItems</span></span>|<span data-ttu-id="a9bb1-140">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="a9bb1-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="a9bb1-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-141">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="a9bb1-142">Он содержит только конфигурацию корневого уровня.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-142">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="a9bb1-143">нестедсчемаитемс</span><span class="sxs-lookup"><span data-stu-id="a9bb1-143">nestedSchemaItems</span></span>|<span data-ttu-id="a9bb1-144">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="a9bb1-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="a9bb1-145">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-145">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="a9bb1-146">Он содержит плоский список всех конфигураций.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-146">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="a9bb1-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9bb1-147">Response</span></span>
<span data-ttu-id="a9bb1-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-148">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9bb1-149">Пример</span><span class="sxs-lookup"><span data-stu-id="a9bb1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9bb1-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9bb1-150">Request</span></span>
<span data-ttu-id="a9bb1-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="a9bb1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9bb1-152">Response</span></span>
<span data-ttu-id="a9bb1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9bb1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





