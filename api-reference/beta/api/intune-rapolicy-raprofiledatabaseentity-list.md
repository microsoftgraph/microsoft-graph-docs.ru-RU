---
title: Список Рапрофиледатабасинтитиес
description: Список свойств и связей объектов Рапрофиледатабасинтити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca8a822b0a79d1e9144261b6cd2f219ee01cbcbb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124349"
---
# <a name="list-raprofiledatabaseentities"></a><span data-ttu-id="ad6d5-103">Список Рапрофиледатабасинтитиес</span><span class="sxs-lookup"><span data-stu-id="ad6d5-103">List raProfileDatabaseEntities</span></span>

<span data-ttu-id="ad6d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad6d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad6d5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad6d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad6d5-107">Список свойств и связей объектов [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="ad6d5-107">List properties and relationships of the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad6d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad6d5-108">Prerequisites</span></span>
<span data-ttu-id="ad6d5-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ad6d5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad6d5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad6d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad6d5-111">Permission type</span></span>|<span data-ttu-id="ad6d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad6d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad6d5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad6d5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ad6d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad6d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad6d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-116">Not supported.</span></span>|
|<span data-ttu-id="ad6d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad6d5-117">Application</span></span>|<span data-ttu-id="ad6d5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad6d5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad6d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad6d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities
```

## <a name="request-headers"></a><span data-ttu-id="ad6d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad6d5-120">Request headers</span></span>
|<span data-ttu-id="ad6d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad6d5-121">Header</span></span>|<span data-ttu-id="ad6d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad6d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad6d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad6d5-123">Authorization</span></span>|<span data-ttu-id="ad6d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad6d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad6d5-125">Accept</span></span>|<span data-ttu-id="ad6d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad6d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad6d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad6d5-127">Request body</span></span>
<span data-ttu-id="ad6d5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad6d5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad6d5-129">Response</span></span>
<span data-ttu-id="ad6d5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-130">If successful, this method returns a `200 OK` response code and a collection of [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad6d5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad6d5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad6d5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad6d5-132">Request</span></span>
<span data-ttu-id="ad6d5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities
```

### <a name="response"></a><span data-ttu-id="ad6d5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad6d5-134">Response</span></span>
<span data-ttu-id="ad6d5-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-135">Here is an example of the response.</span></span> <span data-ttu-id="ad6d5-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ad6d5-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ad6d5-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
      "version": 7,
      "isDeleted": true,
      "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
      "displayName": "Display Name value",
      "linkedProfileIds": [
        "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
      ],
      "profileTypeName": "Profile Type Name value",
      "profileBody": "Profile Body value",
      "profileBodyHash": "Profile Body Hash value",
      "platformType": 12,
      "transformedProfileBody": "Transformed Profile Body value",
      "transformedProfileBodyHash": "Transformed Profile Body Hash value",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "profileId": "6389d896-d896-6389-96d8-896396d88963",
      "eTag": "ETag value",
      "schemaVersion": "betaStart",
      "lastModified": "2017-01-01T00:03:14.6651031-08:00"
    }
  ]
}
```



