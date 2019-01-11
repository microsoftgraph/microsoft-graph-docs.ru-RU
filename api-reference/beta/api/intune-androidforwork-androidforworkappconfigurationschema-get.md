---
title: Get androidForWorkAppConfigurationSchema
description: Чтение свойств и связей объекта androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb6c18d633d9194e692a374e2e551ee482d69cb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823830"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="fdadd-103">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="fdadd-103">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="fdadd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fdadd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdadd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdadd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdadd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fdadd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdadd-107">Чтение свойств и связей объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fdadd-107">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdadd-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fdadd-108">Prerequisites</span></span>
<span data-ttu-id="fdadd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdadd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdadd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdadd-111">Permission type</span></span>|<span data-ttu-id="fdadd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdadd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdadd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdadd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdadd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdadd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fdadd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdadd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdadd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdadd-116">Not supported.</span></span>|
|<span data-ttu-id="fdadd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdadd-117">Application</span></span>|<span data-ttu-id="fdadd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdadd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdadd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdadd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdadd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fdadd-120">Optional query parameters</span></span>
<span data-ttu-id="fdadd-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fdadd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fdadd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdadd-122">Request headers</span></span>
|<span data-ttu-id="fdadd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdadd-123">Header</span></span>|<span data-ttu-id="fdadd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fdadd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdadd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdadd-125">Authorization</span></span>|<span data-ttu-id="fdadd-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fdadd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdadd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fdadd-127">Accept</span></span>|<span data-ttu-id="fdadd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fdadd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdadd-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdadd-129">Request body</span></span>
<span data-ttu-id="fdadd-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdadd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdadd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdadd-131">Response</span></span>
<span data-ttu-id="fdadd-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fdadd-132">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdadd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fdadd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdadd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdadd-134">Request</span></span>
<span data-ttu-id="fdadd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdadd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="fdadd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdadd-136">Response</span></span>
<span data-ttu-id="fdadd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fdadd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 913

{
  "value": {
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
}
```





