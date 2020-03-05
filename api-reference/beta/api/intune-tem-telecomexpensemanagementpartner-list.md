---
title: Список объектов telecomExpenseManagementPartner
description: Список свойств и связей объектов telecomExpenseManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fde3cee253f391340813692d15ef9fab8bf2be2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457792"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="b12fa-103">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b12fa-103">List telecomExpenseManagementPartners</span></span>

<span data-ttu-id="b12fa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b12fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b12fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b12fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b12fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b12fa-107">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b12fa-107">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b12fa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b12fa-108">Prerequisites</span></span>
<span data-ttu-id="b12fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b12fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b12fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b12fa-111">Permission type</span></span>|<span data-ttu-id="b12fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b12fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b12fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b12fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b12fa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b12fa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b12fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b12fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b12fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12fa-116">Not supported.</span></span>|
|<span data-ttu-id="b12fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b12fa-117">Application</span></span>|<span data-ttu-id="b12fa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b12fa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b12fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b12fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="b12fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b12fa-120">Request headers</span></span>
|<span data-ttu-id="b12fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b12fa-121">Header</span></span>|<span data-ttu-id="b12fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b12fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b12fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b12fa-123">Authorization</span></span>|<span data-ttu-id="b12fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b12fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b12fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b12fa-125">Accept</span></span>|<span data-ttu-id="b12fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b12fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b12fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b12fa-127">Request body</span></span>
<span data-ttu-id="b12fa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b12fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b12fa-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b12fa-129">Response</span></span>
<span data-ttu-id="b12fa-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b12fa-130">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b12fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b12fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b12fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b12fa-132">Request</span></span>
<span data-ttu-id="b12fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b12fa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="b12fa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12fa-134">Response</span></span>
<span data-ttu-id="b12fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b12fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





