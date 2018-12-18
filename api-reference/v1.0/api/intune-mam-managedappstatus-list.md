---
title: Перечисление объектов managedAppStatus
description: Список свойств и связей объектов managedAppStatus.
author: tfitzmac
ms.openlocfilehash: 1cf73098931b4ae0e7f7eddf5169f991d5b3d695
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319238"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="b2188-103">Перечисление объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="b2188-103">List managedAppStatuses</span></span>

> <span data-ttu-id="b2188-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2188-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2188-105">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b2188-105">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2188-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2188-106">Prerequisites</span></span>
<span data-ttu-id="b2188-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2188-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2188-109">Permission type</span></span>|<span data-ttu-id="b2188-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2188-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2188-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2188-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2188-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2188-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b2188-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2188-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2188-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2188-114">Not supported.</span></span>|
|<span data-ttu-id="b2188-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2188-115">Application</span></span>|<span data-ttu-id="b2188-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2188-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2188-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2188-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b2188-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2188-118">Request headers</span></span>
|<span data-ttu-id="b2188-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2188-119">Header</span></span>|<span data-ttu-id="b2188-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b2188-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2188-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2188-121">Authorization</span></span>|<span data-ttu-id="b2188-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2188-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2188-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b2188-123">Accept</span></span>|<span data-ttu-id="b2188-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2188-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2188-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2188-125">Request body</span></span>
<span data-ttu-id="b2188-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2188-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2188-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2188-127">Response</span></span>
<span data-ttu-id="b2188-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2188-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2188-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b2188-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2188-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2188-130">Request</span></span>
<span data-ttu-id="b2188-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2188-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="b2188-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2188-132">Response</span></span>
<span data-ttu-id="b2188-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2188-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



