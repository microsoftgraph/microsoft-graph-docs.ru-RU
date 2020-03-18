---
title: Создание объекта androidForWorkAppConfigurationSchema
description: Создание объекта androidForWorkAppConfigurationSchema.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4a668848c58a0399e338aa1f9552b656bd54cf0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815770"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="08bba-103">Создание объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="08bba-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="08bba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08bba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08bba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08bba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08bba-106">Создание объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="08bba-106">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08bba-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08bba-107">Prerequisites</span></span>
<span data-ttu-id="08bba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08bba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08bba-110">Permission type</span></span>|<span data-ttu-id="08bba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08bba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08bba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08bba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08bba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08bba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08bba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08bba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08bba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08bba-115">Not supported.</span></span>|
|<span data-ttu-id="08bba-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="08bba-116">Application</span></span>|<span data-ttu-id="08bba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08bba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08bba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08bba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="08bba-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08bba-119">Request headers</span></span>
|<span data-ttu-id="08bba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08bba-120">Header</span></span>|<span data-ttu-id="08bba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08bba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08bba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08bba-122">Authorization</span></span>|<span data-ttu-id="08bba-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08bba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08bba-124">Accept</span><span class="sxs-lookup"><span data-stu-id="08bba-124">Accept</span></span>|<span data-ttu-id="08bba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08bba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08bba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08bba-126">Request body</span></span>
<span data-ttu-id="08bba-127">В тексте запроса добавьте представление объекта androidForWorkAppConfigurationSchema в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08bba-127">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="08bba-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="08bba-128">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="08bba-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08bba-129">Property</span></span>|<span data-ttu-id="08bba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08bba-130">Type</span></span>|<span data-ttu-id="08bba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08bba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08bba-132">id</span><span class="sxs-lookup"><span data-stu-id="08bba-132">id</span></span>|<span data-ttu-id="08bba-133">String</span><span class="sxs-lookup"><span data-stu-id="08bba-133">String</span></span>|<span data-ttu-id="08bba-134">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="08bba-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="08bba-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="08bba-135">exampleJson</span></span>|<span data-ttu-id="08bba-136">Binary</span><span class="sxs-lookup"><span data-stu-id="08bba-136">Binary</span></span>|<span data-ttu-id="08bba-137">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="08bba-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="08bba-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="08bba-138">schemaItems</span></span>|<span data-ttu-id="08bba-139">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="08bba-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="08bba-140">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="08bba-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="08bba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="08bba-141">Response</span></span>
<span data-ttu-id="08bba-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08bba-142">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08bba-143">Пример</span><span class="sxs-lookup"><span data-stu-id="08bba-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="08bba-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="08bba-144">Request</span></span>
<span data-ttu-id="08bba-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08bba-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08bba-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="08bba-146">Response</span></span>
<span data-ttu-id="08bba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08bba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




