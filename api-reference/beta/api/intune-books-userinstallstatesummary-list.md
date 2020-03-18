---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d08e63e63b6d40eaa3ca99211d56e8c73799402
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760328"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="32920-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="32920-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="32920-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32920-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32920-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32920-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32920-106">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="32920-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32920-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32920-107">Prerequisites</span></span>
<span data-ttu-id="32920-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32920-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32920-110">Permission type</span></span>|<span data-ttu-id="32920-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32920-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32920-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32920-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32920-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="32920-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="32920-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32920-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32920-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32920-115">Not supported.</span></span>|
|<span data-ttu-id="32920-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="32920-116">Application</span></span>|<span data-ttu-id="32920-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="32920-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32920-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32920-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="32920-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32920-119">Request headers</span></span>
|<span data-ttu-id="32920-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32920-120">Header</span></span>|<span data-ttu-id="32920-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32920-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32920-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32920-122">Authorization</span></span>|<span data-ttu-id="32920-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32920-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32920-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32920-124">Accept</span></span>|<span data-ttu-id="32920-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32920-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32920-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32920-126">Request body</span></span>
<span data-ttu-id="32920-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32920-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32920-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="32920-128">Response</span></span>
<span data-ttu-id="32920-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32920-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32920-130">Пример</span><span class="sxs-lookup"><span data-stu-id="32920-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="32920-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="32920-131">Request</span></span>
<span data-ttu-id="32920-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32920-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="32920-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="32920-133">Response</span></span>
<span data-ttu-id="32920-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32920-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




