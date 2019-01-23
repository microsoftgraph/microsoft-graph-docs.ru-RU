---
title: Создание объекта androidForWorkAppConfigurationSchema
description: Создание объекта androidForWorkAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dce0e8355ef722a3201585b79352a7458ec0ef9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394854"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="3bbf3-103">Создание объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3bbf3-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="3bbf3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3bbf3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bbf3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bbf3-107">Создание объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="3bbf3-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bbf3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3bbf3-108">Prerequisites</span></span>
<span data-ttu-id="3bbf3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3bbf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3bbf3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bbf3-111">Permission type</span></span>|<span data-ttu-id="3bbf3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bbf3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bbf3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bbf3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bbf3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bbf3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bbf3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bbf3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bbf3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-116">Not supported.</span></span>|
|<span data-ttu-id="3bbf3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bbf3-117">Application</span></span>|<span data-ttu-id="3bbf3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bbf3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bbf3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="3bbf3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bbf3-120">Request headers</span></span>
|<span data-ttu-id="3bbf3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bbf3-121">Header</span></span>|<span data-ttu-id="3bbf3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3bbf3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bbf3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bbf3-123">Authorization</span></span>|<span data-ttu-id="3bbf3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3bbf3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bbf3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3bbf3-125">Accept</span></span>|<span data-ttu-id="3bbf3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bbf3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bbf3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bbf3-127">Request body</span></span>
<span data-ttu-id="3bbf3-128">В тексте запроса добавьте представление объекта androidForWorkAppConfigurationSchema в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="3bbf3-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="3bbf3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bbf3-130">Property</span></span>|<span data-ttu-id="3bbf3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3bbf3-131">Type</span></span>|<span data-ttu-id="3bbf3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3bbf3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bbf3-133">id</span><span class="sxs-lookup"><span data-stu-id="3bbf3-133">id</span></span>|<span data-ttu-id="3bbf3-134">String</span><span class="sxs-lookup"><span data-stu-id="3bbf3-134">String</span></span>|<span data-ttu-id="3bbf3-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="3bbf3-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="3bbf3-136">exampleJson</span></span>|<span data-ttu-id="3bbf3-137">Binary</span><span class="sxs-lookup"><span data-stu-id="3bbf3-137">Binary</span></span>|<span data-ttu-id="3bbf3-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="3bbf3-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="3bbf3-139">schemaItems</span></span>|<span data-ttu-id="3bbf3-140">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="3bbf3-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="3bbf3-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="3bbf3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bbf3-142">Response</span></span>
<span data-ttu-id="3bbf3-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bbf3-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3bbf3-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bbf3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bbf3-145">Request</span></span>
<span data-ttu-id="3bbf3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3bbf3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bbf3-147">Response</span></span>
<span data-ttu-id="3bbf3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3bbf3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




