---
title: Список deviceManagementIntentSettingCategories
description: Список свойств и связей объектов deviceManagementIntentSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c49d8a7467292e2dc4aae412b74fd13ce62b209e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130933"
---
# <a name="list-devicemanagementintentsettingcategories"></a><span data-ttu-id="44cf4-103">Список deviceManagementIntentSettingCategories</span><span class="sxs-lookup"><span data-stu-id="44cf4-103">List deviceManagementIntentSettingCategories</span></span>

<span data-ttu-id="44cf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44cf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44cf4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44cf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44cf4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44cf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44cf4-107">Список свойств и связей [объектов deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="44cf4-107">List properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44cf4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44cf4-108">Prerequisites</span></span>
<span data-ttu-id="44cf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44cf4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44cf4-111">Permission type</span></span>|<span data-ttu-id="44cf4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44cf4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44cf4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44cf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44cf4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cf4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44cf4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44cf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44cf4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44cf4-116">Not supported.</span></span>|
|<span data-ttu-id="44cf4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="44cf4-117">Application</span></span>|<span data-ttu-id="44cf4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cf4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44cf4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44cf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="44cf4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44cf4-120">Request headers</span></span>
|<span data-ttu-id="44cf4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44cf4-121">Header</span></span>|<span data-ttu-id="44cf4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44cf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44cf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44cf4-123">Authorization</span></span>|<span data-ttu-id="44cf4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44cf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44cf4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44cf4-125">Accept</span></span>|<span data-ttu-id="44cf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44cf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44cf4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44cf4-127">Request body</span></span>
<span data-ttu-id="44cf4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44cf4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44cf4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="44cf4-129">Response</span></span>
<span data-ttu-id="44cf4-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44cf4-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44cf4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="44cf4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="44cf4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="44cf4-132">Request</span></span>
<span data-ttu-id="44cf4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44cf4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
```

### <a name="response"></a><span data-ttu-id="44cf4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="44cf4-134">Response</span></span>
<span data-ttu-id="44cf4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44cf4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
      "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
      "displayName": "Display Name value",
      "hasRequiredSetting": true
    }
  ]
}
```




