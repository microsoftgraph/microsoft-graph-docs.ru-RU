---
title: Get managedAppStatus
description: Чтение свойств и связей объекта managedAppStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca3cd4dd40d985998821e5032e77cb9c0c863a9b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49308566"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="d2abc-103">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d2abc-103">Get managedAppStatus</span></span>

<span data-ttu-id="d2abc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2abc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2abc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2abc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2abc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2abc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2abc-107">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d2abc-107">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2abc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d2abc-108">Prerequisites</span></span>
<span data-ttu-id="d2abc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2abc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2abc-111">Permission type</span></span>|<span data-ttu-id="d2abc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2abc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2abc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2abc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2abc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2abc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2abc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2abc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2abc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2abc-116">Not supported.</span></span>|
|<span data-ttu-id="d2abc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2abc-117">Application</span></span>|<span data-ttu-id="d2abc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2abc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2abc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2abc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2abc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2abc-120">Optional query parameters</span></span>
<span data-ttu-id="d2abc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2abc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2abc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2abc-122">Request headers</span></span>
|<span data-ttu-id="d2abc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2abc-123">Header</span></span>|<span data-ttu-id="d2abc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d2abc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2abc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2abc-125">Authorization</span></span>|<span data-ttu-id="d2abc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2abc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2abc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d2abc-127">Accept</span></span>|<span data-ttu-id="d2abc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d2abc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2abc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2abc-129">Request body</span></span>
<span data-ttu-id="d2abc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2abc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2abc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2abc-131">Response</span></span>
<span data-ttu-id="d2abc-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d2abc-132">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2abc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d2abc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2abc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2abc-134">Request</span></span>
<span data-ttu-id="d2abc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2abc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="d2abc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2abc-136">Response</span></span>
<span data-ttu-id="d2abc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2abc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




