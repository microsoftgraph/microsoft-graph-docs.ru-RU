---
title: Получение androidManagedStoreAppConfigurationSchema
description: Чтение свойства и связи объекта androidManagedStoreAppConfigurationSchema.
ms.openlocfilehash: dc0da9d8cf92a6c346178e44ee8fe08b81ce9f4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077565"
---
# <a name="get-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="7f6d8-103">Получение androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="7f6d8-103">Get androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="7f6d8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f6d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f6d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f6d8-107">Чтение свойства и связи объекта [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="7f6d8-107">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f6d8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f6d8-108">Prerequisites</span></span>
<span data-ttu-id="7f6d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f6d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f6d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f6d8-111">Permission type</span></span>|<span data-ttu-id="7f6d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f6d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f6d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f6d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f6d8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f6d8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f6d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f6d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f6d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-116">Not supported.</span></span>|
|<span data-ttu-id="7f6d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f6d8-117">Application</span></span>|<span data-ttu-id="7f6d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f6d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f6d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f6d8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f6d8-120">Optional query parameters</span></span>
<span data-ttu-id="7f6d8-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f6d8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f6d8-122">Request headers</span></span>
|<span data-ttu-id="7f6d8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f6d8-123">Header</span></span>|<span data-ttu-id="7f6d8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7f6d8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f6d8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f6d8-125">Authorization</span></span>|<span data-ttu-id="7f6d8-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f6d8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f6d8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7f6d8-127">Accept</span></span>|<span data-ttu-id="7f6d8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f6d8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f6d8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f6d8-129">Request body</span></span>
<span data-ttu-id="7f6d8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f6d8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f6d8-131">Response</span></span>
<span data-ttu-id="7f6d8-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f6d8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7f6d8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f6d8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f6d8-134">Request</span></span>
<span data-ttu-id="7f6d8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f6d8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="7f6d8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f6d8-136">Response</span></span>
<span data-ttu-id="7f6d8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7f6d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 923

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
    "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
    "exampleJson": "ZXhhbXBsZUpzb24=",
    "schemaItems": [
      {
        "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





