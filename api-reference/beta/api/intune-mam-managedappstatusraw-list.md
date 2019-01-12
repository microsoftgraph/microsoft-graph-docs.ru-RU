---
title: Перечисление объектов managedAppStatusRaw
description: Перечисление свойств и связей объектов managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7de00af7883cf141071ea898d0cb62916c1eb7d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913627"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="a7e31-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a7e31-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="a7e31-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7e31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7e31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7e31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a7e31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7e31-107">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a7e31-107">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7e31-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a7e31-108">Prerequisites</span></span>
<span data-ttu-id="a7e31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7e31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7e31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7e31-111">Permission type</span></span>|<span data-ttu-id="a7e31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7e31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7e31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7e31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7e31-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7e31-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a7e31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7e31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7e31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e31-116">Not supported.</span></span>|
|<span data-ttu-id="a7e31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7e31-117">Application</span></span>|<span data-ttu-id="a7e31-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7e31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7e31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a7e31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7e31-120">Request headers</span></span>
|<span data-ttu-id="a7e31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7e31-121">Header</span></span>|<span data-ttu-id="a7e31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7e31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7e31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7e31-123">Authorization</span></span>|<span data-ttu-id="a7e31-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a7e31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7e31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7e31-125">Accept</span></span>|<span data-ttu-id="a7e31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7e31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7e31-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7e31-127">Request body</span></span>
<span data-ttu-id="a7e31-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7e31-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7e31-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7e31-129">Response</span></span>
<span data-ttu-id="a7e31-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a7e31-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7e31-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a7e31-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7e31-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7e31-132">Request</span></span>
<span data-ttu-id="a7e31-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7e31-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="a7e31-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7e31-134">Response</span></span>
<span data-ttu-id="a7e31-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7e31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





