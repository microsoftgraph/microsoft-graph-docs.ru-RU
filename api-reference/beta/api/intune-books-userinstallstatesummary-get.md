---
title: Get userInstallStateSummary
description: Чтение свойств и связей объекта userInstallStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 91ee89e3d23f81fb3def1291f070bc31c5e85c8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413880"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="3e989-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e989-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="3e989-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e989-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e989-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e989-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e989-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e989-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e989-107">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3e989-107">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e989-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3e989-108">Prerequisites</span></span>
<span data-ttu-id="3e989-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e989-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3e989-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e989-111">Permission type</span></span>|<span data-ttu-id="3e989-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e989-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e989-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e989-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e989-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e989-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3e989-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e989-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e989-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e989-116">Not supported.</span></span>|
|<span data-ttu-id="3e989-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e989-117">Application</span></span>|<span data-ttu-id="3e989-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e989-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e989-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e989-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e989-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e989-120">Optional query parameters</span></span>
<span data-ttu-id="3e989-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e989-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e989-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e989-122">Request headers</span></span>
|<span data-ttu-id="3e989-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e989-123">Header</span></span>|<span data-ttu-id="3e989-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3e989-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e989-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e989-125">Authorization</span></span>|<span data-ttu-id="3e989-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3e989-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e989-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3e989-127">Accept</span></span>|<span data-ttu-id="3e989-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3e989-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e989-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e989-129">Request body</span></span>
<span data-ttu-id="3e989-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e989-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e989-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e989-131">Response</span></span>
<span data-ttu-id="3e989-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e989-132">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e989-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3e989-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e989-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e989-134">Request</span></span>
<span data-ttu-id="3e989-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e989-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="3e989-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e989-136">Response</span></span>
<span data-ttu-id="3e989-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e989-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




