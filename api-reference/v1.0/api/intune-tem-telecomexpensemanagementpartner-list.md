---
title: Список объектов telecomExpenseManagementPartner
description: Список свойств и связей объектов telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3b587403176ba3dff028a7895eb766c1541b50a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576614"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="8cbb9-103">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8cbb9-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="8cbb9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cbb9-105">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8cbb9-105">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cbb9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8cbb9-106">Prerequisites</span></span>
<span data-ttu-id="8cbb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cbb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cbb9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cbb9-109">Permission type</span></span>|<span data-ttu-id="8cbb9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cbb9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cbb9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cbb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cbb9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cbb9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8cbb9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cbb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cbb9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-114">Not supported.</span></span>|
|<span data-ttu-id="8cbb9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cbb9-115">Application</span></span>|<span data-ttu-id="8cbb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cbb9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cbb9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8cbb9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cbb9-118">Request headers</span></span>
|<span data-ttu-id="8cbb9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cbb9-119">Header</span></span>|<span data-ttu-id="8cbb9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8cbb9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cbb9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cbb9-121">Authorization</span></span>|<span data-ttu-id="8cbb9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cbb9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8cbb9-123">Accept</span></span>|<span data-ttu-id="8cbb9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8cbb9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cbb9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cbb9-125">Request body</span></span>
<span data-ttu-id="8cbb9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cbb9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cbb9-127">Response</span></span>
<span data-ttu-id="8cbb9-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-128">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cbb9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8cbb9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cbb9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cbb9-130">Request</span></span>
<span data-ttu-id="8cbb9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="8cbb9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cbb9-132">Response</span></span>
<span data-ttu-id="8cbb9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cbb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



