---
title: Получение объекта softwareUpdateStatusSummary
description: Чтение свойств и связей объекта softwareUpdateStatusSummary.
author: tfitzmac
ms.openlocfilehash: 4f490db4042c03233f2613e44b6a6f90460f9345
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354028"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="97bdd-103">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="97bdd-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="97bdd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="97bdd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97bdd-105">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="97bdd-105">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97bdd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="97bdd-106">Prerequisites</span></span>
<span data-ttu-id="97bdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97bdd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97bdd-109">Permission type</span></span>|<span data-ttu-id="97bdd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97bdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97bdd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97bdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97bdd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97bdd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97bdd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97bdd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97bdd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97bdd-114">Not supported.</span></span>|
|<span data-ttu-id="97bdd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97bdd-115">Application</span></span>|<span data-ttu-id="97bdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97bdd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97bdd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97bdd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97bdd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="97bdd-118">Optional query parameters</span></span>
<span data-ttu-id="97bdd-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97bdd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97bdd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97bdd-120">Request headers</span></span>
|<span data-ttu-id="97bdd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97bdd-121">Header</span></span>|<span data-ttu-id="97bdd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97bdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97bdd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97bdd-123">Authorization</span></span>|<span data-ttu-id="97bdd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="97bdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97bdd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97bdd-125">Accept</span></span>|<span data-ttu-id="97bdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97bdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97bdd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97bdd-127">Request body</span></span>
<span data-ttu-id="97bdd-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97bdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97bdd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="97bdd-129">Response</span></span>
<span data-ttu-id="97bdd-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97bdd-130">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97bdd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="97bdd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="97bdd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="97bdd-132">Request</span></span>
<span data-ttu-id="97bdd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97bdd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="97bdd-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="97bdd-134">Response</span></span>
<span data-ttu-id="97bdd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="97bdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```



