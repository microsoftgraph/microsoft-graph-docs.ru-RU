---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6821b394a1bb526c6e2a34efc07fe04b2105b37f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132956"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="c173c-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="c173c-103">List userInstallStateSummaries</span></span>

<span data-ttu-id="c173c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c173c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c173c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c173c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c173c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c173c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c173c-107">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c173c-107">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c173c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c173c-108">Prerequisites</span></span>
<span data-ttu-id="c173c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c173c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c173c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c173c-111">Permission type</span></span>|<span data-ttu-id="c173c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c173c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c173c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c173c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c173c-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c173c-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c173c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c173c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c173c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c173c-116">Not supported.</span></span>|
|<span data-ttu-id="c173c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c173c-117">Application</span></span>|<span data-ttu-id="c173c-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c173c-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c173c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c173c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c173c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c173c-120">Request headers</span></span>
|<span data-ttu-id="c173c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c173c-121">Header</span></span>|<span data-ttu-id="c173c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c173c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c173c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c173c-123">Authorization</span></span>|<span data-ttu-id="c173c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c173c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c173c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c173c-125">Accept</span></span>|<span data-ttu-id="c173c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c173c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c173c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c173c-127">Request body</span></span>
<span data-ttu-id="c173c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c173c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c173c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173c-129">Response</span></span>
<span data-ttu-id="c173c-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c173c-130">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c173c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c173c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c173c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c173c-132">Request</span></span>
<span data-ttu-id="c173c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c173c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="c173c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173c-134">Response</span></span>
<span data-ttu-id="c173c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c173c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




