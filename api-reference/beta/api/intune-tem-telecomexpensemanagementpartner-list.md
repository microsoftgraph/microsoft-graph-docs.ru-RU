---
title: Список объектов telecomExpenseManagementPartner
description: Список свойств и связей объектов telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40da54b31579d85bbab320b7c81aca09afa3f3e1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200535"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="c8b72-103">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c8b72-103">List telecomExpenseManagementPartners</span></span>

<span data-ttu-id="c8b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8b72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8b72-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8b72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8b72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8b72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8b72-107">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c8b72-107">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8b72-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8b72-108">Prerequisites</span></span>
<span data-ttu-id="c8b72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8b72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8b72-111">Permission type</span></span>|<span data-ttu-id="c8b72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8b72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8b72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8b72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8b72-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8b72-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c8b72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8b72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8b72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8b72-116">Not supported.</span></span>|
|<span data-ttu-id="c8b72-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8b72-117">Application</span></span>|<span data-ttu-id="c8b72-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8b72-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8b72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8b72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c8b72-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8b72-120">Request headers</span></span>
|<span data-ttu-id="c8b72-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8b72-121">Header</span></span>|<span data-ttu-id="c8b72-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8b72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8b72-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8b72-123">Authorization</span></span>|<span data-ttu-id="c8b72-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8b72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8b72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8b72-125">Accept</span></span>|<span data-ttu-id="c8b72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8b72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8b72-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8b72-127">Request body</span></span>
<span data-ttu-id="c8b72-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8b72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8b72-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8b72-129">Response</span></span>
<span data-ttu-id="c8b72-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c8b72-130">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8b72-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c8b72-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8b72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8b72-132">Request</span></span>
<span data-ttu-id="c8b72-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8b72-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="c8b72-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8b72-134">Response</span></span>
<span data-ttu-id="c8b72-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8b72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




