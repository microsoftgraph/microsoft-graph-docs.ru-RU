---
title: Список androidManagedStoreAppConfigurationSchemas
description: Список свойств и связей объектов AndroidManagedStoreAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7808f946bd65f569db1802d60bb2b6d33e829ded
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141122"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a><span data-ttu-id="064ef-103">Список androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="064ef-103">List androidManagedStoreAppConfigurationSchemas</span></span>

<span data-ttu-id="064ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="064ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="064ef-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="064ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="064ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="064ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="064ef-107">Список свойств и связей [объектов AndroidManagedStoreAppConfigurationSchema.](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)</span><span class="sxs-lookup"><span data-stu-id="064ef-107">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="064ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="064ef-108">Prerequisites</span></span>
<span data-ttu-id="064ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="064ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="064ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="064ef-111">Permission type</span></span>|<span data-ttu-id="064ef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="064ef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="064ef-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="064ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="064ef-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="064ef-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="064ef-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="064ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="064ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="064ef-116">Not supported.</span></span>|
|<span data-ttu-id="064ef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="064ef-117">Application</span></span>|<span data-ttu-id="064ef-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="064ef-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="064ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="064ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="064ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="064ef-120">Request headers</span></span>
|<span data-ttu-id="064ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="064ef-121">Header</span></span>|<span data-ttu-id="064ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="064ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="064ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="064ef-123">Authorization</span></span>|<span data-ttu-id="064ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="064ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="064ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="064ef-125">Accept</span></span>|<span data-ttu-id="064ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="064ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="064ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="064ef-127">Request body</span></span>
<span data-ttu-id="064ef-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="064ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="064ef-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="064ef-129">Response</span></span>
<span data-ttu-id="064ef-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [AndroidManagedStoreConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="064ef-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="064ef-131">Пример</span><span class="sxs-lookup"><span data-stu-id="064ef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="064ef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="064ef-132">Request</span></span>
<span data-ttu-id="064ef-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="064ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="064ef-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="064ef-134">Response</span></span>
<span data-ttu-id="064ef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="064ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1871

{
  "value": [
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
  ]
}
```




