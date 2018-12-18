---
title: Обновление androidManagedStoreAppConfigurationSchema
description: Обновление свойства объекта androidManagedStoreAppConfigurationSchema.
author: tfitzmac
ms.openlocfilehash: fcdacb235de85392ab39fb410b6b936fd7ce0195
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362631"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="0383a-103">Обновление androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="0383a-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="0383a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0383a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0383a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0383a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0383a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0383a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0383a-107">Обновление свойства объекта [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="0383a-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0383a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0383a-108">Prerequisites</span></span>
<span data-ttu-id="0383a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0383a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0383a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0383a-111">Permission type</span></span>|<span data-ttu-id="0383a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0383a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0383a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0383a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0383a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0383a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0383a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0383a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0383a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0383a-116">Not supported.</span></span>|
|<span data-ttu-id="0383a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0383a-117">Application</span></span>|<span data-ttu-id="0383a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0383a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0383a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0383a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="0383a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0383a-120">Request headers</span></span>
|<span data-ttu-id="0383a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0383a-121">Header</span></span>|<span data-ttu-id="0383a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0383a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0383a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0383a-123">Authorization</span></span>|<span data-ttu-id="0383a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0383a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0383a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0383a-125">Accept</span></span>|<span data-ttu-id="0383a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0383a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0383a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0383a-127">Request body</span></span>
<span data-ttu-id="0383a-128">В тексте запроса укажите представление JSON для объекта [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="0383a-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="0383a-129">В следующей таблице показаны свойства, которые необходимы для создания [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0383a-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="0383a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0383a-130">Property</span></span>|<span data-ttu-id="0383a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0383a-131">Type</span></span>|<span data-ttu-id="0383a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0383a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0383a-133">id</span><span class="sxs-lookup"><span data-stu-id="0383a-133">id</span></span>|<span data-ttu-id="0383a-134">String</span><span class="sxs-lookup"><span data-stu-id="0383a-134">String</span></span>|<span data-ttu-id="0383a-135">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="0383a-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="0383a-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="0383a-136">exampleJson</span></span>|<span data-ttu-id="0383a-137">Binary</span><span class="sxs-lookup"><span data-stu-id="0383a-137">Binary</span></span>|<span data-ttu-id="0383a-138">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="0383a-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="0383a-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="0383a-139">schemaItems</span></span>|<span data-ttu-id="0383a-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0383a-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="0383a-141">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="0383a-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="0383a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0383a-142">Response</span></span>
<span data-ttu-id="0383a-143">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0383a-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0383a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="0383a-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="0383a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0383a-145">Request</span></span>
<span data-ttu-id="0383a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0383a-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 725

{
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

### <a name="response"></a><span data-ttu-id="0383a-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="0383a-147">Response</span></span>
<span data-ttu-id="0383a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0383a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





