---
title: Получение объекта telecomExpenseManagementPartner
description: Чтение свойств и связей объекта telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3bcdc2551c1b6beba3347be74d2c9a93677ccd7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457558"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="fff2d-103">Получение объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="fff2d-103">Get telecomExpenseManagementPartner</span></span>

<span data-ttu-id="fff2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fff2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fff2d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fff2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fff2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fff2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fff2d-107">Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="fff2d-107">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fff2d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fff2d-108">Prerequisites</span></span>
<span data-ttu-id="fff2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fff2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fff2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fff2d-111">Permission type</span></span>|<span data-ttu-id="fff2d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fff2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fff2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fff2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fff2d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fff2d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fff2d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fff2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fff2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fff2d-116">Not supported.</span></span>|
|<span data-ttu-id="fff2d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fff2d-117">Application</span></span>|<span data-ttu-id="fff2d-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fff2d-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fff2d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fff2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fff2d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fff2d-120">Optional query parameters</span></span>
<span data-ttu-id="fff2d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fff2d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fff2d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fff2d-122">Request headers</span></span>
|<span data-ttu-id="fff2d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fff2d-123">Header</span></span>|<span data-ttu-id="fff2d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fff2d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fff2d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fff2d-125">Authorization</span></span>|<span data-ttu-id="fff2d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fff2d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fff2d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fff2d-127">Accept</span></span>|<span data-ttu-id="fff2d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fff2d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fff2d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fff2d-129">Request body</span></span>
<span data-ttu-id="fff2d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fff2d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fff2d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fff2d-131">Response</span></span>
<span data-ttu-id="fff2d-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fff2d-132">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fff2d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fff2d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fff2d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fff2d-134">Request</span></span>
<span data-ttu-id="fff2d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fff2d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="fff2d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fff2d-136">Response</span></span>
<span data-ttu-id="fff2d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fff2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



