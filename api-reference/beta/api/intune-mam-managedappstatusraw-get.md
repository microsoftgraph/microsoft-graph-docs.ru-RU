---
title: Get managedAppStatusRaw
description: Считывание свойств и связей объекта managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50b91d137894077da0b07ba8ebc34c40234c2521
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167300"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="769bc-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="769bc-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="769bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="769bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="769bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="769bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="769bc-106">Чтение свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="769bc-106">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="769bc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="769bc-107">Prerequisites</span></span>
<span data-ttu-id="769bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="769bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="769bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="769bc-110">Permission type</span></span>|<span data-ttu-id="769bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="769bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="769bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="769bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="769bc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="769bc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="769bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="769bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="769bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="769bc-115">Not supported.</span></span>|
|<span data-ttu-id="769bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="769bc-116">Application</span></span>|<span data-ttu-id="769bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="769bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="769bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="769bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="769bc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="769bc-119">Optional query parameters</span></span>
<span data-ttu-id="769bc-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="769bc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="769bc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="769bc-121">Request headers</span></span>
|<span data-ttu-id="769bc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="769bc-122">Header</span></span>|<span data-ttu-id="769bc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="769bc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="769bc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="769bc-124">Authorization</span></span>|<span data-ttu-id="769bc-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="769bc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="769bc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="769bc-126">Accept</span></span>|<span data-ttu-id="769bc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="769bc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="769bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="769bc-128">Request body</span></span>
<span data-ttu-id="769bc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="769bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="769bc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="769bc-130">Response</span></span>
<span data-ttu-id="769bc-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="769bc-131">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="769bc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="769bc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="769bc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="769bc-133">Request</span></span>
<span data-ttu-id="769bc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="769bc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="769bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="769bc-135">Response</span></span>
<span data-ttu-id="769bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="769bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```




