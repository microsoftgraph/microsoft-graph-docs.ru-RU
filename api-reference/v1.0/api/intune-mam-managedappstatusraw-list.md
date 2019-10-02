---
title: Перечисление объектов managedAppStatusRaw
description: Список свойств и связей объектов managedAppStatusRaw.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef3f88e1e6798dca3e03640ce9eacf2929a19a3b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363460"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="f72a2-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="f72a2-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="f72a2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f72a2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f72a2-105">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="f72a2-105">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f72a2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f72a2-106">Prerequisites</span></span>
<span data-ttu-id="f72a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f72a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f72a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f72a2-109">Permission type</span></span>|<span data-ttu-id="f72a2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f72a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f72a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f72a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f72a2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f72a2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f72a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f72a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f72a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f72a2-114">Not supported.</span></span>|
|<span data-ttu-id="f72a2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f72a2-115">Application</span></span>|<span data-ttu-id="f72a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f72a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f72a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f72a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f72a2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f72a2-118">Request headers</span></span>
|<span data-ttu-id="f72a2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f72a2-119">Header</span></span>|<span data-ttu-id="f72a2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f72a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f72a2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f72a2-121">Authorization</span></span>|<span data-ttu-id="f72a2-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f72a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f72a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f72a2-123">Accept</span></span>|<span data-ttu-id="f72a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f72a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f72a2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f72a2-125">Request body</span></span>
<span data-ttu-id="f72a2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f72a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f72a2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f72a2-127">Response</span></span>
<span data-ttu-id="f72a2-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f72a2-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f72a2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f72a2-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f72a2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f72a2-130">Request</span></span>
<span data-ttu-id="f72a2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f72a2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="f72a2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f72a2-132">Response</span></span>
<span data-ttu-id="f72a2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f72a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




