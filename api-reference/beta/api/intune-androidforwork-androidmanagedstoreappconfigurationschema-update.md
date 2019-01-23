---
title: Обновление androidManagedStoreAppConfigurationSchema
description: Обновление свойства объекта androidManagedStoreAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 326f56f497f1086ccc6e37d0171261c50dfb9c77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410135"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="bbb46-103">Обновление androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="bbb46-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="bbb46-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bbb46-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bbb46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbb46-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbb46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbb46-107">Обновление свойства объекта [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="bbb46-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbb46-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bbb46-108">Prerequisites</span></span>
<span data-ttu-id="bbb46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bbb46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bbb46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbb46-111">Permission type</span></span>|<span data-ttu-id="bbb46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbb46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbb46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbb46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbb46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbb46-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbb46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbb46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb46-116">Not supported.</span></span>|
|<span data-ttu-id="bbb46-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbb46-117">Application</span></span>|<span data-ttu-id="bbb46-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbb46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbb46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="bbb46-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbb46-120">Request headers</span></span>
|<span data-ttu-id="bbb46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbb46-121">Header</span></span>|<span data-ttu-id="bbb46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bbb46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbb46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbb46-123">Authorization</span></span>|<span data-ttu-id="bbb46-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bbb46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbb46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bbb46-125">Accept</span></span>|<span data-ttu-id="bbb46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbb46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbb46-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbb46-127">Request body</span></span>
<span data-ttu-id="bbb46-128">В тексте запроса укажите представление JSON для объекта [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="bbb46-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="bbb46-129">В следующей таблице показаны свойства, которые необходимы для создания [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="bbb46-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="bbb46-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbb46-130">Property</span></span>|<span data-ttu-id="bbb46-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bbb46-131">Type</span></span>|<span data-ttu-id="bbb46-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bbb46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb46-133">id</span><span class="sxs-lookup"><span data-stu-id="bbb46-133">id</span></span>|<span data-ttu-id="bbb46-134">String</span><span class="sxs-lookup"><span data-stu-id="bbb46-134">String</span></span>|<span data-ttu-id="bbb46-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="bbb46-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="bbb46-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="bbb46-136">exampleJson</span></span>|<span data-ttu-id="bbb46-137">Binary</span><span class="sxs-lookup"><span data-stu-id="bbb46-137">Binary</span></span>|<span data-ttu-id="bbb46-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="bbb46-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="bbb46-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="bbb46-139">schemaItems</span></span>|<span data-ttu-id="bbb46-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bbb46-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="bbb46-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="bbb46-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="bbb46-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb46-142">Response</span></span>
<span data-ttu-id="bbb46-143">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bbb46-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb46-144">Пример</span><span class="sxs-lookup"><span data-stu-id="bbb46-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbb46-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbb46-145">Request</span></span>
<span data-ttu-id="bbb46-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbb46-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
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
```

### <a name="response"></a><span data-ttu-id="bbb46-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb46-147">Response</span></span>
<span data-ttu-id="bbb46-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bbb46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
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
```




