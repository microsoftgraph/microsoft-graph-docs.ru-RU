---
title: Создание Андроидманажедстореаппконфигуратионсчема
description: Создание нового объекта Андроидманажедстореаппконфигуратионсчема.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71079de480b0c450873b30ae8127dca6a507a9c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498188"
---
# <a name="create-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="b5349-103">Создание Андроидманажедстореаппконфигуратионсчема</span><span class="sxs-lookup"><span data-stu-id="b5349-103">Create androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="b5349-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5349-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5349-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5349-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5349-106">Создание нового объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="b5349-106">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5349-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5349-107">Prerequisites</span></span>
<span data-ttu-id="b5349-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5349-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5349-110">Permission type</span></span>|<span data-ttu-id="b5349-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5349-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5349-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5349-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5349-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5349-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5349-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5349-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5349-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5349-115">Not supported.</span></span>|
|<span data-ttu-id="b5349-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5349-116">Application</span></span>|<span data-ttu-id="b5349-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5349-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5349-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5349-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="b5349-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5349-119">Request headers</span></span>
|<span data-ttu-id="b5349-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5349-120">Header</span></span>|<span data-ttu-id="b5349-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b5349-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5349-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5349-122">Authorization</span></span>|<span data-ttu-id="b5349-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5349-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5349-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5349-124">Accept</span></span>|<span data-ttu-id="b5349-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5349-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5349-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5349-126">Request body</span></span>
<span data-ttu-id="b5349-127">В тексте запроса добавьте представление объекта Андроидманажедстореаппконфигуратионсчема в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5349-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfigurationSchema object.</span></span>

<span data-ttu-id="b5349-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореаппконфигуратионсчема.</span><span class="sxs-lookup"><span data-stu-id="b5349-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfigurationSchema.</span></span>

|<span data-ttu-id="b5349-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5349-129">Property</span></span>|<span data-ttu-id="b5349-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b5349-130">Type</span></span>|<span data-ttu-id="b5349-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b5349-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5349-132">id</span><span class="sxs-lookup"><span data-stu-id="b5349-132">id</span></span>|<span data-ttu-id="b5349-133">String</span><span class="sxs-lookup"><span data-stu-id="b5349-133">String</span></span>|<span data-ttu-id="b5349-134">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="b5349-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="b5349-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="b5349-135">exampleJson</span></span>|<span data-ttu-id="b5349-136">Binary</span><span class="sxs-lookup"><span data-stu-id="b5349-136">Binary</span></span>|<span data-ttu-id="b5349-137">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="b5349-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="b5349-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="b5349-138">schemaItems</span></span>|<span data-ttu-id="b5349-139">Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5349-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="b5349-140">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="b5349-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="b5349-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5349-141">Response</span></span>
<span data-ttu-id="b5349-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5349-142">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5349-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b5349-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5349-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5349-144">Request</span></span>
<span data-ttu-id="b5349-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5349-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="b5349-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5349-146">Response</span></span>
<span data-ttu-id="b5349-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5349-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





