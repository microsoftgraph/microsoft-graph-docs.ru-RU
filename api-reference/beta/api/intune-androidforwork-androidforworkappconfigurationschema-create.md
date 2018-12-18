---
title: Создание объекта androidForWorkAppConfigurationSchema
description: Создание объекта androidForWorkAppConfigurationSchema.
author: tfitzmac
ms.openlocfilehash: 92974019e98a1dc8403d5672f631de7849caebc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353188"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="d9dfc-103">Создание объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="d9dfc-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="d9dfc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9dfc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9dfc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9dfc-107">Создание объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d9dfc-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9dfc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d9dfc-108">Prerequisites</span></span>
<span data-ttu-id="d9dfc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9dfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9dfc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9dfc-111">Permission type</span></span>|<span data-ttu-id="d9dfc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9dfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9dfc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9dfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9dfc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9dfc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9dfc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9dfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9dfc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-116">Not supported.</span></span>|
|<span data-ttu-id="d9dfc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9dfc-117">Application</span></span>|<span data-ttu-id="d9dfc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9dfc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9dfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="d9dfc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9dfc-120">Request headers</span></span>
|<span data-ttu-id="d9dfc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9dfc-121">Header</span></span>|<span data-ttu-id="d9dfc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9dfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9dfc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9dfc-123">Authorization</span></span>|<span data-ttu-id="d9dfc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d9dfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9dfc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9dfc-125">Accept</span></span>|<span data-ttu-id="d9dfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9dfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9dfc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9dfc-127">Request body</span></span>
<span data-ttu-id="d9dfc-128">В тексте запроса добавьте представление объекта androidForWorkAppConfigurationSchema в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="d9dfc-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="d9dfc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9dfc-130">Property</span></span>|<span data-ttu-id="d9dfc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9dfc-131">Type</span></span>|<span data-ttu-id="d9dfc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9dfc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9dfc-133">id</span><span class="sxs-lookup"><span data-stu-id="d9dfc-133">id</span></span>|<span data-ttu-id="d9dfc-134">String</span><span class="sxs-lookup"><span data-stu-id="d9dfc-134">String</span></span>|<span data-ttu-id="d9dfc-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="d9dfc-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="d9dfc-136">exampleJson</span></span>|<span data-ttu-id="d9dfc-137">Binary</span><span class="sxs-lookup"><span data-stu-id="d9dfc-137">Binary</span></span>|<span data-ttu-id="d9dfc-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="d9dfc-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="d9dfc-139">schemaItems</span></span>|<span data-ttu-id="d9dfc-140">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9dfc-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="d9dfc-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="d9dfc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9dfc-142">Response</span></span>
<span data-ttu-id="d9dfc-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9dfc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d9dfc-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9dfc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9dfc-145">Request</span></span>
<span data-ttu-id="d9dfc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9dfc-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9dfc-147">Response</span></span>
<span data-ttu-id="d9dfc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d9dfc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





