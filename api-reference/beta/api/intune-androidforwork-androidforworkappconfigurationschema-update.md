---
title: Обновление объекта androidForWorkAppConfigurationSchema
description: Обновление свойств объекта androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09393062a4d23622c10bf87f3fec420fc51c6650
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946520"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="58049-103">Обновление объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="58049-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="58049-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58049-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58049-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58049-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58049-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58049-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58049-107">Обновление свойств объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="58049-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58049-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58049-108">Prerequisites</span></span>
<span data-ttu-id="58049-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58049-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58049-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58049-111">Permission type</span></span>|<span data-ttu-id="58049-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58049-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58049-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58049-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58049-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58049-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58049-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58049-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58049-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58049-116">Not supported.</span></span>|
|<span data-ttu-id="58049-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58049-117">Application</span></span>|<span data-ttu-id="58049-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58049-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58049-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58049-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="58049-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58049-120">Request headers</span></span>
|<span data-ttu-id="58049-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58049-121">Header</span></span>|<span data-ttu-id="58049-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58049-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58049-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58049-123">Authorization</span></span>|<span data-ttu-id="58049-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="58049-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58049-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58049-125">Accept</span></span>|<span data-ttu-id="58049-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58049-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58049-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58049-127">Request body</span></span>
<span data-ttu-id="58049-128">В тексте запроса добавьте представление объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58049-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="58049-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="58049-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="58049-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="58049-130">Property</span></span>|<span data-ttu-id="58049-131">Тип</span><span class="sxs-lookup"><span data-stu-id="58049-131">Type</span></span>|<span data-ttu-id="58049-132">Описание</span><span class="sxs-lookup"><span data-stu-id="58049-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58049-133">id</span><span class="sxs-lookup"><span data-stu-id="58049-133">id</span></span>|<span data-ttu-id="58049-134">String</span><span class="sxs-lookup"><span data-stu-id="58049-134">String</span></span>|<span data-ttu-id="58049-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="58049-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="58049-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="58049-136">exampleJson</span></span>|<span data-ttu-id="58049-137">Binary</span><span class="sxs-lookup"><span data-stu-id="58049-137">Binary</span></span>|<span data-ttu-id="58049-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="58049-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="58049-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="58049-139">schemaItems</span></span>|<span data-ttu-id="58049-140">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="58049-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="58049-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="58049-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="58049-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="58049-142">Response</span></span>
<span data-ttu-id="58049-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58049-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58049-144">Пример</span><span class="sxs-lookup"><span data-stu-id="58049-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="58049-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="58049-145">Request</span></span>
<span data-ttu-id="58049-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58049-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
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

### <a name="response"></a><span data-ttu-id="58049-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="58049-147">Response</span></span>
<span data-ttu-id="58049-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="58049-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





