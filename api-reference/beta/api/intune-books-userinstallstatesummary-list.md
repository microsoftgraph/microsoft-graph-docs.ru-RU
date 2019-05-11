---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7f2eee3154900da9bb98c3fe28bb4f3dc4ca247
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934112"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="2ca21-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="2ca21-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="2ca21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ca21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ca21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ca21-106">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2ca21-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ca21-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2ca21-107">Prerequisites</span></span>
<span data-ttu-id="2ca21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ca21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca21-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ca21-110">Permission type</span></span>|<span data-ttu-id="2ca21-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ca21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ca21-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ca21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ca21-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ca21-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2ca21-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ca21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ca21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca21-115">Not supported.</span></span>|
|<span data-ttu-id="2ca21-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ca21-116">Application</span></span>|<span data-ttu-id="2ca21-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ca21-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ca21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="2ca21-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ca21-119">Request headers</span></span>
|<span data-ttu-id="2ca21-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ca21-120">Header</span></span>|<span data-ttu-id="2ca21-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2ca21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ca21-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ca21-122">Authorization</span></span>|<span data-ttu-id="2ca21-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ca21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ca21-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2ca21-124">Accept</span></span>|<span data-ttu-id="2ca21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ca21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ca21-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ca21-126">Request body</span></span>
<span data-ttu-id="2ca21-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ca21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ca21-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ca21-128">Response</span></span>
<span data-ttu-id="2ca21-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ca21-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ca21-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2ca21-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ca21-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ca21-131">Request</span></span>
<span data-ttu-id="2ca21-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ca21-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="2ca21-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ca21-133">Response</span></span>
<span data-ttu-id="2ca21-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ca21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




