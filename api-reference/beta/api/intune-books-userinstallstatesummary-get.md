---
title: Get userInstallStateSummary
description: Чтение свойств и связей объекта userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: 152160f99220f95c9f743ee637da35c693400d41
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358347"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="b968d-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b968d-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="b968d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b968d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b968d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b968d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b968d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b968d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b968d-107">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b968d-107">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b968d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b968d-108">Prerequisites</span></span>
<span data-ttu-id="b968d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b968d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b968d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b968d-111">Permission type</span></span>|<span data-ttu-id="b968d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b968d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b968d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b968d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b968d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b968d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b968d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b968d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b968d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b968d-116">Not supported.</span></span>|
|<span data-ttu-id="b968d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b968d-117">Application</span></span>|<span data-ttu-id="b968d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b968d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b968d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b968d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b968d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b968d-120">Optional query parameters</span></span>
<span data-ttu-id="b968d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b968d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b968d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b968d-122">Request headers</span></span>
|<span data-ttu-id="b968d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b968d-123">Header</span></span>|<span data-ttu-id="b968d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b968d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b968d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b968d-125">Authorization</span></span>|<span data-ttu-id="b968d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b968d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b968d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b968d-127">Accept</span></span>|<span data-ttu-id="b968d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b968d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b968d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b968d-129">Request body</span></span>
<span data-ttu-id="b968d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b968d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b968d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b968d-131">Response</span></span>
<span data-ttu-id="b968d-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b968d-132">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b968d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b968d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b968d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b968d-134">Request</span></span>
<span data-ttu-id="b968d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b968d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="b968d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b968d-136">Response</span></span>
<span data-ttu-id="b968d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b968d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```





