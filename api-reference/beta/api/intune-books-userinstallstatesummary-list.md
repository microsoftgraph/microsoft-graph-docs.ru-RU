---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e1e189e51872cbb72b2b270ed72075aeb41cfa3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858727"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="f8fdc-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="f8fdc-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="f8fdc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8fdc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8fdc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8fdc-107">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f8fdc-107">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8fdc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8fdc-108">Prerequisites</span></span>
<span data-ttu-id="f8fdc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8fdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8fdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8fdc-111">Permission type</span></span>|<span data-ttu-id="f8fdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8fdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8fdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8fdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8fdc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8fdc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8fdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8fdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8fdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-116">Not supported.</span></span>|
|<span data-ttu-id="f8fdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8fdc-117">Application</span></span>|<span data-ttu-id="f8fdc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8fdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8fdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="f8fdc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8fdc-120">Request headers</span></span>
|<span data-ttu-id="f8fdc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8fdc-121">Header</span></span>|<span data-ttu-id="f8fdc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8fdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8fdc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8fdc-123">Authorization</span></span>|<span data-ttu-id="f8fdc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f8fdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8fdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8fdc-125">Accept</span></span>|<span data-ttu-id="f8fdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8fdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8fdc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8fdc-127">Request body</span></span>
<span data-ttu-id="f8fdc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8fdc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8fdc-129">Response</span></span>
<span data-ttu-id="f8fdc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-130">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8fdc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8fdc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8fdc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8fdc-132">Request</span></span>
<span data-ttu-id="f8fdc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="f8fdc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8fdc-134">Response</span></span>
<span data-ttu-id="f8fdc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f8fdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





