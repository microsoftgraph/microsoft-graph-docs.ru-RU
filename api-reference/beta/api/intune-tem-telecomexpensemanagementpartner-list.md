---
title: Список объектов telecomExpenseManagementPartner
description: Список свойств и связей объектов telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b9cf187a68ca3350884279fb2569f890deec41c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082184"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="26dea-103">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="26dea-103">List telecomExpenseManagementPartners</span></span>

<span data-ttu-id="26dea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26dea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26dea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26dea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26dea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26dea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26dea-107">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="26dea-107">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26dea-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="26dea-108">Prerequisites</span></span>
<span data-ttu-id="26dea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26dea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26dea-111">Permission type</span></span>|<span data-ttu-id="26dea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26dea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26dea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26dea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26dea-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="26dea-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="26dea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26dea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26dea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26dea-116">Not supported.</span></span>|
|<span data-ttu-id="26dea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26dea-117">Application</span></span>|<span data-ttu-id="26dea-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="26dea-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26dea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26dea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="26dea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26dea-120">Request headers</span></span>
|<span data-ttu-id="26dea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26dea-121">Header</span></span>|<span data-ttu-id="26dea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26dea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26dea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26dea-123">Authorization</span></span>|<span data-ttu-id="26dea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26dea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26dea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26dea-125">Accept</span></span>|<span data-ttu-id="26dea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26dea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26dea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26dea-127">Request body</span></span>
<span data-ttu-id="26dea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26dea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26dea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26dea-129">Response</span></span>
<span data-ttu-id="26dea-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26dea-130">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26dea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="26dea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="26dea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26dea-132">Request</span></span>
<span data-ttu-id="26dea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26dea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="26dea-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="26dea-134">Response</span></span>
<span data-ttu-id="26dea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26dea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






