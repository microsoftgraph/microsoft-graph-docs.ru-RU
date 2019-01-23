---
title: Перечисление объектов androidForWorkAppConfigurationSchema
description: Список свойств и связей объектов androidForWorkAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79961f2955b2cc866ba858b765a27e77dda43407
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395050"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="1d3b3-103">Перечисление объектов androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="1d3b3-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="1d3b3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d3b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d3b3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d3b3-107">Список свойств и связей объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1d3b3-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d3b3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1d3b3-108">Prerequisites</span></span>
<span data-ttu-id="1d3b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d3b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d3b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d3b3-111">Permission type</span></span>|<span data-ttu-id="1d3b3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d3b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d3b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d3b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d3b3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d3b3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1d3b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d3b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d3b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-116">Not supported.</span></span>|
|<span data-ttu-id="1d3b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d3b3-117">Application</span></span>|<span data-ttu-id="1d3b3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d3b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d3b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="1d3b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d3b3-120">Request headers</span></span>
|<span data-ttu-id="1d3b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d3b3-121">Header</span></span>|<span data-ttu-id="1d3b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d3b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d3b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d3b3-123">Authorization</span></span>|<span data-ttu-id="1d3b3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1d3b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d3b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d3b3-125">Accept</span></span>|<span data-ttu-id="1d3b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d3b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d3b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d3b3-127">Request body</span></span>
<span data-ttu-id="1d3b3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d3b3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d3b3-129">Response</span></span>
<span data-ttu-id="1d3b3-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d3b3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1d3b3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d3b3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d3b3-132">Request</span></span>
<span data-ttu-id="1d3b3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="1d3b3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d3b3-134">Response</span></span>
<span data-ttu-id="1d3b3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d3b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
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
  ]
}
```




