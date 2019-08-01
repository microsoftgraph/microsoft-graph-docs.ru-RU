---
title: Перечисление объектов managedAppStatusRaw
description: Список свойств и связей объектов managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 764b0f66b04abae641731753f8ddba9379b092b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996646"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="6cede-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="6cede-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="6cede-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cede-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cede-105">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="6cede-105">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cede-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6cede-106">Prerequisites</span></span>
<span data-ttu-id="6cede-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cede-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cede-109">Permission type</span></span>|<span data-ttu-id="6cede-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cede-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cede-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cede-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6cede-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cede-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6cede-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cede-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cede-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cede-114">Not supported.</span></span>|
|<span data-ttu-id="6cede-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cede-115">Application</span></span>|<span data-ttu-id="6cede-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cede-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cede-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cede-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6cede-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cede-118">Request headers</span></span>
|<span data-ttu-id="6cede-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cede-119">Header</span></span>|<span data-ttu-id="6cede-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6cede-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cede-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cede-121">Authorization</span></span>|<span data-ttu-id="6cede-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cede-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cede-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6cede-123">Accept</span></span>|<span data-ttu-id="6cede-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6cede-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cede-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6cede-125">Request body</span></span>
<span data-ttu-id="6cede-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6cede-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cede-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cede-127">Response</span></span>
<span data-ttu-id="6cede-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6cede-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cede-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6cede-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cede-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cede-130">Request</span></span>
<span data-ttu-id="6cede-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cede-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="6cede-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cede-132">Response</span></span>
<span data-ttu-id="6cede-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```



