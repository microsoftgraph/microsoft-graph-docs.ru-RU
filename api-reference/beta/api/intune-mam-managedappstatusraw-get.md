---
title: Get managedAppStatusRaw
description: Считывание свойств и связей объекта managedAppStatusRaw.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30bae06ff10b369a83f11ac50f169449e5cc0cc8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399922"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="93290-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="93290-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="93290-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93290-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="93290-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93290-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93290-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93290-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93290-107">Чтение свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="93290-107">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93290-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="93290-108">Prerequisites</span></span>
<span data-ttu-id="93290-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93290-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93290-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93290-111">Permission type</span></span>|<span data-ttu-id="93290-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93290-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93290-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93290-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="93290-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="93290-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93290-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93290-116">Not supported.</span></span>|
|<span data-ttu-id="93290-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93290-117">Application</span></span>|<span data-ttu-id="93290-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93290-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93290-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93290-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93290-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93290-120">Optional query parameters</span></span>
<span data-ttu-id="93290-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="93290-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93290-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93290-122">Request headers</span></span>
|<span data-ttu-id="93290-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93290-123">Header</span></span>|<span data-ttu-id="93290-124">Значение</span><span class="sxs-lookup"><span data-stu-id="93290-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93290-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="93290-125">Authorization</span></span>|<span data-ttu-id="93290-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="93290-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93290-127">Accept</span><span class="sxs-lookup"><span data-stu-id="93290-127">Accept</span></span>|<span data-ttu-id="93290-128">application/json</span><span class="sxs-lookup"><span data-stu-id="93290-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93290-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93290-129">Request body</span></span>
<span data-ttu-id="93290-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93290-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93290-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="93290-131">Response</span></span>
<span data-ttu-id="93290-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93290-132">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93290-133">Пример</span><span class="sxs-lookup"><span data-stu-id="93290-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="93290-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="93290-134">Request</span></span>
<span data-ttu-id="93290-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93290-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="93290-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93290-136">Response</span></span>
<span data-ttu-id="93290-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="93290-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




