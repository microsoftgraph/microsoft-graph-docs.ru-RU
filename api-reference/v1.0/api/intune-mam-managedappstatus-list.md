---
title: Перечисление объектов managedAppStatus
description: Список свойств и связей объектов managedAppStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b5a01f37045c7c9927604a87441ef6d5e007092c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855225"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="2f271-103">Перечисление объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="2f271-103">List managedAppStatuses</span></span>

> <span data-ttu-id="2f271-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f271-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f271-105">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2f271-105">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f271-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f271-106">Prerequisites</span></span>
<span data-ttu-id="2f271-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f271-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f271-109">Permission type</span></span>|<span data-ttu-id="2f271-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f271-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f271-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f271-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f271-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f271-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f271-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f271-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f271-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f271-114">Not supported.</span></span>|
|<span data-ttu-id="2f271-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f271-115">Application</span></span>|<span data-ttu-id="2f271-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f271-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f271-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f271-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2f271-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f271-118">Request headers</span></span>
|<span data-ttu-id="2f271-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f271-119">Header</span></span>|<span data-ttu-id="2f271-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2f271-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f271-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f271-121">Authorization</span></span>|<span data-ttu-id="2f271-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f271-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f271-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f271-123">Accept</span></span>|<span data-ttu-id="2f271-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f271-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f271-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f271-125">Request body</span></span>
<span data-ttu-id="2f271-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f271-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f271-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f271-127">Response</span></span>
<span data-ttu-id="2f271-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f271-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f271-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2f271-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f271-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f271-130">Request</span></span>
<span data-ttu-id="2f271-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f271-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="2f271-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f271-132">Response</span></span>
<span data-ttu-id="2f271-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f271-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatus",
      "displayName": "Display Name value",
      "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
      "version": "Version value"
    }
  ]
}
```



