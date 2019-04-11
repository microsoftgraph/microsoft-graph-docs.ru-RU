---
title: Get managedAppStatus
description: Чтение свойств и связей объекта managedAppStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6554b6872f42983881de8aca01306857a2e9276
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773408"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="50403-103">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="50403-103">Get managedAppStatus</span></span>

> <span data-ttu-id="50403-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50403-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50403-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50403-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50403-106">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="50403-106">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50403-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="50403-107">Prerequisites</span></span>
<span data-ttu-id="50403-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50403-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50403-110">Permission type</span></span>|<span data-ttu-id="50403-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50403-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50403-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50403-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50403-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50403-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="50403-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50403-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50403-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50403-115">Not supported.</span></span>|
|<span data-ttu-id="50403-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50403-116">Application</span></span>|<span data-ttu-id="50403-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50403-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50403-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50403-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50403-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50403-119">Optional query parameters</span></span>
<span data-ttu-id="50403-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50403-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50403-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50403-121">Request headers</span></span>
|<span data-ttu-id="50403-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50403-122">Header</span></span>|<span data-ttu-id="50403-123">Значение</span><span class="sxs-lookup"><span data-stu-id="50403-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50403-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50403-124">Authorization</span></span>|<span data-ttu-id="50403-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50403-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50403-126">Accept</span><span class="sxs-lookup"><span data-stu-id="50403-126">Accept</span></span>|<span data-ttu-id="50403-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50403-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50403-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50403-128">Request body</span></span>
<span data-ttu-id="50403-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50403-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50403-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="50403-130">Response</span></span>
<span data-ttu-id="50403-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50403-131">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50403-132">Пример</span><span class="sxs-lookup"><span data-stu-id="50403-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50403-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="50403-133">Request</span></span>
<span data-ttu-id="50403-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50403-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="50403-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="50403-135">Response</span></span>
<span data-ttu-id="50403-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50403-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





