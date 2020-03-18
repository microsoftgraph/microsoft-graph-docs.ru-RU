---
title: Список объектов telecomExpenseManagementPartner
description: Список свойств и связей объектов telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4689d12089bebe2b222d17ed4d4fe48016907191
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800314"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="9c9bf-103">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="9c9bf-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="9c9bf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c9bf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c9bf-106">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="9c9bf-106">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c9bf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9c9bf-107">Prerequisites</span></span>
<span data-ttu-id="9c9bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c9bf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c9bf-110">Permission type</span></span>|<span data-ttu-id="9c9bf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c9bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c9bf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c9bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c9bf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c9bf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9c9bf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c9bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c9bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-115">Not supported.</span></span>|
|<span data-ttu-id="9c9bf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9c9bf-116">Application</span></span>|<span data-ttu-id="9c9bf-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c9bf-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c9bf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c9bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="9c9bf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9c9bf-119">Request headers</span></span>
|<span data-ttu-id="9c9bf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c9bf-120">Header</span></span>|<span data-ttu-id="9c9bf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9c9bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c9bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c9bf-122">Authorization</span></span>|<span data-ttu-id="9c9bf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c9bf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9c9bf-124">Accept</span></span>|<span data-ttu-id="9c9bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c9bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c9bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c9bf-126">Request body</span></span>
<span data-ttu-id="9c9bf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c9bf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c9bf-128">Response</span></span>
<span data-ttu-id="9c9bf-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-129">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c9bf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9c9bf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c9bf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c9bf-131">Request</span></span>
<span data-ttu-id="9c9bf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="9c9bf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c9bf-133">Response</span></span>
<span data-ttu-id="9c9bf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c9bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```




