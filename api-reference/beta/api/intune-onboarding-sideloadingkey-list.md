---
title: Список sideLoadingKeies
description: Список свойств и связей объектов sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 348d683bf3612edfed068baacba05ea6496494f3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125487"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="bf9b4-103">Список sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="bf9b4-103">List sideLoadingKeies</span></span>

<span data-ttu-id="bf9b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf9b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf9b4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf9b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf9b4-107">Список свойств и связей [объектов sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="bf9b4-107">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf9b4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf9b4-108">Prerequisites</span></span>
<span data-ttu-id="bf9b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9b4-111">Permission type</span></span>|<span data-ttu-id="bf9b4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf9b4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf9b4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf9b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf9b4-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9b4-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf9b4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf9b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf9b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-116">Not supported.</span></span>|
|<span data-ttu-id="bf9b4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf9b4-117">Application</span></span>|<span data-ttu-id="bf9b4-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9b4-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf9b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf9b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="bf9b4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf9b4-120">Request headers</span></span>
|<span data-ttu-id="bf9b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf9b4-121">Header</span></span>|<span data-ttu-id="bf9b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf9b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf9b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf9b4-123">Authorization</span></span>|<span data-ttu-id="bf9b4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf9b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf9b4-125">Accept</span></span>|<span data-ttu-id="bf9b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf9b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf9b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf9b4-127">Request body</span></span>
<span data-ttu-id="bf9b4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf9b4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf9b4-129">Response</span></span>
<span data-ttu-id="bf9b4-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-130">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf9b4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bf9b4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf9b4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf9b4-132">Request</span></span>
<span data-ttu-id="bf9b4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="bf9b4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf9b4-134">Response</span></span>
<span data-ttu-id="bf9b4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf9b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```




