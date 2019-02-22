---
title: Создание объекта androidForWorkAppConfigurationSchema
description: Создание объекта androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfbd2d8a1c6cefbde7ea8f14e640aa4ef5a0a5fb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148533"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="83756-103">Создание объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="83756-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="83756-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83756-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83756-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83756-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83756-106">Создание объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83756-106">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83756-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83756-107">Prerequisites</span></span>
<span data-ttu-id="83756-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="83756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83756-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83756-110">Permission type</span></span>|<span data-ttu-id="83756-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83756-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83756-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83756-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83756-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83756-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83756-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83756-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83756-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83756-115">Not supported.</span></span>|
|<span data-ttu-id="83756-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83756-116">Application</span></span>|<span data-ttu-id="83756-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83756-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83756-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83756-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="83756-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83756-119">Request headers</span></span>
|<span data-ttu-id="83756-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83756-120">Header</span></span>|<span data-ttu-id="83756-121">Значение</span><span class="sxs-lookup"><span data-stu-id="83756-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83756-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83756-122">Authorization</span></span>|<span data-ttu-id="83756-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="83756-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83756-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83756-124">Accept</span></span>|<span data-ttu-id="83756-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83756-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83756-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83756-126">Request body</span></span>
<span data-ttu-id="83756-127">В тексте запроса добавьте представление объекта androidForWorkAppConfigurationSchema в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83756-127">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="83756-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="83756-128">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="83756-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="83756-129">Property</span></span>|<span data-ttu-id="83756-130">Тип</span><span class="sxs-lookup"><span data-stu-id="83756-130">Type</span></span>|<span data-ttu-id="83756-131">Описание</span><span class="sxs-lookup"><span data-stu-id="83756-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83756-132">id</span><span class="sxs-lookup"><span data-stu-id="83756-132">id</span></span>|<span data-ttu-id="83756-133">String</span><span class="sxs-lookup"><span data-stu-id="83756-133">String</span></span>|<span data-ttu-id="83756-134">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="83756-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="83756-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="83756-135">exampleJson</span></span>|<span data-ttu-id="83756-136">Binary</span><span class="sxs-lookup"><span data-stu-id="83756-136">Binary</span></span>|<span data-ttu-id="83756-137">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="83756-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="83756-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="83756-138">schemaItems</span></span>|<span data-ttu-id="83756-139">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="83756-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="83756-140">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="83756-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="83756-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="83756-141">Response</span></span>
<span data-ttu-id="83756-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83756-142">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83756-143">Пример</span><span class="sxs-lookup"><span data-stu-id="83756-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="83756-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="83756-144">Request</span></span>
<span data-ttu-id="83756-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83756-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83756-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="83756-146">Response</span></span>
<span data-ttu-id="83756-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83756-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




