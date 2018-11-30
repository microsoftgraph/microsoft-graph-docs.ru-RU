---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
ms.openlocfilehash: e6febdb32ebb7c0183508b77870d8508bed35d52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080069"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="42465-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="42465-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="42465-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42465-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42465-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42465-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42465-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="42465-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42465-107">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="42465-107">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42465-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="42465-108">Prerequisites</span></span>
<span data-ttu-id="42465-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42465-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42465-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42465-111">Permission type</span></span>|<span data-ttu-id="42465-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42465-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42465-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42465-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42465-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="42465-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="42465-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42465-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42465-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42465-116">Not supported.</span></span>|
|<span data-ttu-id="42465-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42465-117">Application</span></span>|<span data-ttu-id="42465-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42465-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42465-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42465-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42465-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42465-120">Optional query parameters</span></span>
<span data-ttu-id="42465-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42465-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="42465-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42465-122">Request headers</span></span>
|<span data-ttu-id="42465-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42465-123">Header</span></span>|<span data-ttu-id="42465-124">Значение</span><span class="sxs-lookup"><span data-stu-id="42465-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42465-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="42465-125">Authorization</span></span>|<span data-ttu-id="42465-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42465-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42465-127">Accept</span><span class="sxs-lookup"><span data-stu-id="42465-127">Accept</span></span>|<span data-ttu-id="42465-128">application/json</span><span class="sxs-lookup"><span data-stu-id="42465-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42465-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42465-129">Request body</span></span>
<span data-ttu-id="42465-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42465-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42465-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="42465-131">Response</span></span>
<span data-ttu-id="42465-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42465-132">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42465-133">Пример</span><span class="sxs-lookup"><span data-stu-id="42465-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="42465-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="42465-134">Request</span></span>
<span data-ttu-id="42465-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42465-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="42465-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="42465-136">Response</span></span>
<span data-ttu-id="42465-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="42465-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": {
    "@odata.type": "#microsoft.graph.eBookInstallSummary",
    "id": "9708ad78-ad78-9708-78ad-089778ad0897",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notInstalledUserCount": 5
  }
}
```





