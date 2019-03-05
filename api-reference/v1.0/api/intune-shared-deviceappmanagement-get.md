---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c5d54e1dfeb67192465468a8abe2f26a39c2c50a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257388"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="a20ee-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a20ee-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="a20ee-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a20ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a20ee-105">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a20ee-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a20ee-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a20ee-106">Prerequisites</span></span>

<span data-ttu-id="a20ee-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="a20ee-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a20ee-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a20ee-108">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>  <span data-ttu-id="a20ee-109">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="a20ee-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="a20ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a20ee-110">Permission type</span></span>|<span data-ttu-id="a20ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a20ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a20ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a20ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a20ee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a20ee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="a20ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a20ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a20ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a20ee-115">Not supported.</span></span>|
|<span data-ttu-id="a20ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a20ee-116">Application</span></span>|<span data-ttu-id="a20ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a20ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a20ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a20ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a20ee-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a20ee-119">Optional query parameters</span></span>
<span data-ttu-id="a20ee-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a20ee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a20ee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a20ee-121">Request headers</span></span>
|<span data-ttu-id="a20ee-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a20ee-122">Header</span></span>|<span data-ttu-id="a20ee-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a20ee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a20ee-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a20ee-124">Authorization</span></span>|<span data-ttu-id="a20ee-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a20ee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a20ee-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a20ee-126">Accept</span></span>|<span data-ttu-id="a20ee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a20ee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a20ee-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a20ee-128">Request body</span></span>
<span data-ttu-id="a20ee-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a20ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a20ee-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a20ee-130">Response</span></span>
<span data-ttu-id="a20ee-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a20ee-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="a20ee-132">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="a20ee-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="a20ee-133">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="a20ee-133">Example response</span></span>
<span data-ttu-id="a20ee-134">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a20ee-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a20ee-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a20ee-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



