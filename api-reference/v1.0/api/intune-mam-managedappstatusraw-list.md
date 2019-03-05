---
title: Перечисление объектов managedAppStatusRaw
description: Перечисление свойств и связей объектов managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdbb95f771c28ec9723362e823537b2f2f34f005
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254718"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="2f322-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="2f322-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="2f322-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f322-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f322-105">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="2f322-105">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f322-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f322-106">Prerequisites</span></span>
<span data-ttu-id="2f322-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f322-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f322-109">Permission type</span></span>|<span data-ttu-id="2f322-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f322-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f322-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f322-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f322-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f322-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f322-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f322-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f322-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f322-114">Not supported.</span></span>|
|<span data-ttu-id="2f322-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f322-115">Application</span></span>|<span data-ttu-id="2f322-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f322-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f322-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f322-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2f322-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f322-118">Request headers</span></span>
|<span data-ttu-id="2f322-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f322-119">Header</span></span>|<span data-ttu-id="2f322-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2f322-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f322-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f322-121">Authorization</span></span>|<span data-ttu-id="2f322-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f322-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f322-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f322-123">Accept</span></span>|<span data-ttu-id="2f322-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f322-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f322-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f322-125">Request body</span></span>
<span data-ttu-id="2f322-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f322-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f322-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f322-127">Response</span></span>
<span data-ttu-id="2f322-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f322-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f322-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2f322-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f322-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f322-130">Request</span></span>
<span data-ttu-id="2f322-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f322-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="2f322-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f322-132">Response</span></span>
<span data-ttu-id="2f322-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f322-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



