---
title: Get managedAppStatus
description: Чтение свойств и связей объекта managedAppStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a4af336721a370160d5087e45bd2e984bbd361c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980690"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="f7615-103">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f7615-103">Get managedAppStatus</span></span>

> <span data-ttu-id="f7615-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7615-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7615-106">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f7615-106">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7615-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f7615-107">Prerequisites</span></span>
<span data-ttu-id="f7615-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7615-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7615-110">Permission type</span></span>|<span data-ttu-id="f7615-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7615-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7615-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7615-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7615-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7615-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f7615-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7615-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7615-115">Not supported.</span></span>|
|<span data-ttu-id="f7615-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7615-116">Application</span></span>|<span data-ttu-id="f7615-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7615-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7615-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7615-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7615-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7615-119">Optional query parameters</span></span>
<span data-ttu-id="f7615-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7615-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7615-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7615-121">Request headers</span></span>
|<span data-ttu-id="f7615-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7615-122">Header</span></span>|<span data-ttu-id="f7615-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f7615-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7615-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7615-124">Authorization</span></span>|<span data-ttu-id="f7615-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7615-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7615-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f7615-126">Accept</span></span>|<span data-ttu-id="f7615-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f7615-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7615-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7615-128">Request body</span></span>
<span data-ttu-id="f7615-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7615-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7615-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7615-130">Response</span></span>
<span data-ttu-id="f7615-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7615-131">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7615-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f7615-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7615-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7615-133">Request</span></span>
<span data-ttu-id="f7615-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7615-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="f7615-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7615-135">Response</span></span>
<span data-ttu-id="f7615-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7615-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatus",
    "displayName": "Display Name value",
    "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
    "version": "Version value"
  }
}
```





