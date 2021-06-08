---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e82dc695cc018b0d6b4510c2cb3e0109c6180ea7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760723"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="deb7c-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="deb7c-103">List userInstallStateSummaries</span></span>

<span data-ttu-id="deb7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="deb7c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="deb7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deb7c-106">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="deb7c-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deb7c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="deb7c-107">Prerequisites</span></span>
<span data-ttu-id="deb7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb7c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb7c-110">Permission type</span></span>|<span data-ttu-id="deb7c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb7c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb7c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="deb7c-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb7c-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="deb7c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb7c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb7c-115">Not supported.</span></span>|
|<span data-ttu-id="deb7c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="deb7c-116">Application</span></span>|<span data-ttu-id="deb7c-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb7c-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb7c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="deb7c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="deb7c-119">Request headers</span></span>
|<span data-ttu-id="deb7c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="deb7c-120">Header</span></span>|<span data-ttu-id="deb7c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="deb7c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deb7c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb7c-122">Authorization</span></span>|<span data-ttu-id="deb7c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb7c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deb7c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="deb7c-124">Accept</span></span>|<span data-ttu-id="deb7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="deb7c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb7c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deb7c-126">Request body</span></span>
<span data-ttu-id="deb7c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="deb7c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deb7c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb7c-128">Response</span></span>
<span data-ttu-id="deb7c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="deb7c-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deb7c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="deb7c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="deb7c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb7c-131">Request</span></span>
<span data-ttu-id="deb7c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb7c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="deb7c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb7c-133">Response</span></span>
<span data-ttu-id="deb7c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="deb7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




