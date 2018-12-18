---
title: Get userInstallStateSummary
description: Чтение свойств и связей объекта userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: 4d0506b9d0e4736479d6bdd70e4176ffd82ea87c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346608"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="61a5f-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="61a5f-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="61a5f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="61a5f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61a5f-105">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="61a5f-105">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61a5f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="61a5f-106">Prerequisites</span></span>
<span data-ttu-id="61a5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61a5f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61a5f-109">Permission type</span></span>|<span data-ttu-id="61a5f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61a5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61a5f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61a5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61a5f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="61a5f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="61a5f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61a5f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61a5f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61a5f-114">Not supported.</span></span>|
|<span data-ttu-id="61a5f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61a5f-115">Application</span></span>|<span data-ttu-id="61a5f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61a5f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61a5f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61a5f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61a5f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61a5f-118">Optional query parameters</span></span>
<span data-ttu-id="61a5f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="61a5f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="61a5f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61a5f-120">Request headers</span></span>
|<span data-ttu-id="61a5f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61a5f-121">Header</span></span>|<span data-ttu-id="61a5f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="61a5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61a5f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61a5f-123">Authorization</span></span>|<span data-ttu-id="61a5f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="61a5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61a5f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="61a5f-125">Accept</span></span>|<span data-ttu-id="61a5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61a5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61a5f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61a5f-127">Request body</span></span>
<span data-ttu-id="61a5f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61a5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61a5f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="61a5f-129">Response</span></span>
<span data-ttu-id="61a5f-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="61a5f-130">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a5f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="61a5f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="61a5f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="61a5f-132">Request</span></span>
<span data-ttu-id="61a5f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61a5f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="61a5f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="61a5f-134">Response</span></span>
<span data-ttu-id="61a5f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="61a5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



