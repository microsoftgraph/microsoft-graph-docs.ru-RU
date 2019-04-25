---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6ffe715dec0ba761f9c5636a7c184c64cf248b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524563"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="66e31-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="66e31-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="66e31-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66e31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e31-105">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="66e31-105">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66e31-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66e31-106">Prerequisites</span></span>
<span data-ttu-id="66e31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66e31-109">Permission type</span></span>|<span data-ttu-id="66e31-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66e31-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66e31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66e31-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66e31-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="66e31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66e31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e31-114">Not supported.</span></span>|
|<span data-ttu-id="66e31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66e31-115">Application</span></span>|<span data-ttu-id="66e31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66e31-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="66e31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66e31-118">Request headers</span></span>
|<span data-ttu-id="66e31-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66e31-119">Header</span></span>|<span data-ttu-id="66e31-120">Значение</span><span class="sxs-lookup"><span data-stu-id="66e31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e31-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66e31-121">Authorization</span></span>|<span data-ttu-id="66e31-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66e31-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e31-123">Accept</span><span class="sxs-lookup"><span data-stu-id="66e31-123">Accept</span></span>|<span data-ttu-id="66e31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66e31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e31-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66e31-125">Request body</span></span>
<span data-ttu-id="66e31-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66e31-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66e31-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e31-127">Response</span></span>
<span data-ttu-id="66e31-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66e31-128">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e31-129">Пример</span><span class="sxs-lookup"><span data-stu-id="66e31-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="66e31-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="66e31-130">Request</span></span>
<span data-ttu-id="66e31-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66e31-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="66e31-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e31-132">Response</span></span>
<span data-ttu-id="66e31-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66e31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



