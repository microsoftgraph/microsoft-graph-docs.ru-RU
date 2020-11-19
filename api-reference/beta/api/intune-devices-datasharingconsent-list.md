---
title: Список Даташарингконсентс
description: Список свойств и связей объектов Даташарингконсент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 309ce59e023c8af14b001e4a24e5058e0353066f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229214"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="961ea-103">Список Даташарингконсентс</span><span class="sxs-lookup"><span data-stu-id="961ea-103">List dataSharingConsents</span></span>

<span data-ttu-id="961ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="961ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="961ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="961ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="961ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="961ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="961ea-107">Список свойств и связей объектов [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="961ea-107">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="961ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="961ea-108">Prerequisites</span></span>
<span data-ttu-id="961ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="961ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="961ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="961ea-111">Permission type</span></span>|<span data-ttu-id="961ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="961ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="961ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="961ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="961ea-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="961ea-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="961ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="961ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="961ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="961ea-116">Not supported.</span></span>|
|<span data-ttu-id="961ea-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="961ea-117">Application</span></span>|<span data-ttu-id="961ea-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="961ea-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="961ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="961ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="961ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="961ea-120">Request headers</span></span>
|<span data-ttu-id="961ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="961ea-121">Header</span></span>|<span data-ttu-id="961ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="961ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="961ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="961ea-123">Authorization</span></span>|<span data-ttu-id="961ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="961ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="961ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="961ea-125">Accept</span></span>|<span data-ttu-id="961ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="961ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="961ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="961ea-127">Request body</span></span>
<span data-ttu-id="961ea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="961ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="961ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="961ea-129">Response</span></span>
<span data-ttu-id="961ea-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [даташарингконсент](../resources/intune-devices-datasharingconsent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="961ea-130">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="961ea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="961ea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="961ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="961ea-132">Request</span></span>
<span data-ttu-id="961ea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="961ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="961ea-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="961ea-134">Response</span></span>
<span data-ttu-id="961ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="961ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataSharingConsent",
      "id": "333387f7-87f7-3333-f787-3333f7873333",
      "serviceDisplayName": "Service Display Name value",
      "termsUrl": "https://example.com/termsUrl/",
      "granted": true,
      "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
      "grantedByUpn": "Granted By Upn value",
      "grantedByUserId": "Granted By User Id value"
    }
  ]
}
```




