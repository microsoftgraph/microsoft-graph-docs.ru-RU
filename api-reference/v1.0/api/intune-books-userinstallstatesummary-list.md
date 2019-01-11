---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 919d4cfc6aa3c84b6482f82278dd7017e2e78af9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875588"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="40bdc-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="40bdc-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="40bdc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40bdc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40bdc-105">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="40bdc-105">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40bdc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40bdc-106">Prerequisites</span></span>
<span data-ttu-id="40bdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40bdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40bdc-109">Permission type</span></span>|<span data-ttu-id="40bdc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40bdc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40bdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40bdc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40bdc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="40bdc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="40bdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40bdc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40bdc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40bdc-114">Not supported.</span></span>|
|<span data-ttu-id="40bdc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40bdc-115">Application</span></span>|<span data-ttu-id="40bdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40bdc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40bdc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40bdc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="40bdc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40bdc-118">Request headers</span></span>
|<span data-ttu-id="40bdc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40bdc-119">Header</span></span>|<span data-ttu-id="40bdc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="40bdc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40bdc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40bdc-121">Authorization</span></span>|<span data-ttu-id="40bdc-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="40bdc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40bdc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40bdc-123">Accept</span></span>|<span data-ttu-id="40bdc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40bdc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40bdc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40bdc-125">Request body</span></span>
<span data-ttu-id="40bdc-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40bdc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40bdc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="40bdc-127">Response</span></span>
<span data-ttu-id="40bdc-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40bdc-128">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40bdc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="40bdc-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="40bdc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="40bdc-130">Request</span></span>
<span data-ttu-id="40bdc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40bdc-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="40bdc-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="40bdc-132">Response</span></span>
<span data-ttu-id="40bdc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40bdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```



