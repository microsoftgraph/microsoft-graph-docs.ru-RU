---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a8ce11c97defe387d98f2b8391077d51e7047698
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755539"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="47791-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="47791-103">Get deviceManagement</span></span>

<span data-ttu-id="47791-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47791-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47791-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47791-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47791-106">Чтение свойств и связей объекта [deviceManagement](../resources/intune-notification-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="47791-106">Read properties and relationships of the [deviceManagement](../resources/intune-notification-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47791-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47791-107">Prerequisites</span></span>
<span data-ttu-id="47791-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47791-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47791-110">Permission type</span></span>|<span data-ttu-id="47791-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47791-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47791-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47791-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47791-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47791-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47791-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47791-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47791-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47791-115">Not supported.</span></span>|
|<span data-ttu-id="47791-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="47791-116">Application</span></span>|<span data-ttu-id="47791-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47791-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47791-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47791-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47791-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47791-119">Optional query parameters</span></span>
<span data-ttu-id="47791-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47791-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47791-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47791-121">Request headers</span></span>
|<span data-ttu-id="47791-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47791-122">Header</span></span>|<span data-ttu-id="47791-123">Значение</span><span class="sxs-lookup"><span data-stu-id="47791-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47791-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47791-124">Authorization</span></span>|<span data-ttu-id="47791-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47791-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47791-126">Accept</span><span class="sxs-lookup"><span data-stu-id="47791-126">Accept</span></span>|<span data-ttu-id="47791-127">application/json</span><span class="sxs-lookup"><span data-stu-id="47791-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47791-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47791-128">Request body</span></span>
<span data-ttu-id="47791-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47791-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47791-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="47791-130">Response</span></span>
<span data-ttu-id="47791-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-notification-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47791-131">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-notification-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47791-132">Пример</span><span class="sxs-lookup"><span data-stu-id="47791-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="47791-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="47791-133">Request</span></span>
<span data-ttu-id="47791-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47791-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="47791-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="47791-135">Response</span></span>
<span data-ttu-id="47791-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47791-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```




