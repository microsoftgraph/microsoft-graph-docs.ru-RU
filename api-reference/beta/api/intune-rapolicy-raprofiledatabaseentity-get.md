---
title: Получение Рапрофиледатабасинтити
description: Чтение свойств и связей объекта Рапрофиледатабасинтити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0dbd34afd108a50a5e91aac414cc19ecd86282
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124350"
---
# <a name="get-raprofiledatabaseentity"></a><span data-ttu-id="81be0-103">Получение Рапрофиледатабасинтити</span><span class="sxs-lookup"><span data-stu-id="81be0-103">Get raProfileDatabaseEntity</span></span>

<span data-ttu-id="81be0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81be0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81be0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81be0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81be0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81be0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81be0-107">Чтение свойств и связей объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="81be0-107">Read properties and relationships of the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81be0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="81be0-108">Prerequisites</span></span>
<span data-ttu-id="81be0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="81be0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="81be0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81be0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81be0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81be0-111">Permission type</span></span>|<span data-ttu-id="81be0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81be0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81be0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81be0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81be0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="81be0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="81be0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81be0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81be0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81be0-116">Not supported.</span></span>|
|<span data-ttu-id="81be0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81be0-117">Application</span></span>|<span data-ttu-id="81be0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="81be0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81be0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81be0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81be0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81be0-120">Optional query parameters</span></span>
<span data-ttu-id="81be0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81be0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81be0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81be0-122">Request headers</span></span>
|<span data-ttu-id="81be0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81be0-123">Header</span></span>|<span data-ttu-id="81be0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="81be0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81be0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81be0-125">Authorization</span></span>|<span data-ttu-id="81be0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81be0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81be0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="81be0-127">Accept</span></span>|<span data-ttu-id="81be0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="81be0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81be0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81be0-129">Request body</span></span>
<span data-ttu-id="81be0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81be0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81be0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="81be0-131">Response</span></span>
<span data-ttu-id="81be0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81be0-132">If successful, this method returns a `200 OK` response code and [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81be0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="81be0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="81be0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="81be0-134">Request</span></span>
<span data-ttu-id="81be0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81be0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a><span data-ttu-id="81be0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="81be0-136">Response</span></span>
<span data-ttu-id="81be0-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="81be0-137">Here is an example of the response.</span></span> <span data-ttu-id="81be0-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="81be0-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="81be0-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="81be0-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "value": {
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
}
```



