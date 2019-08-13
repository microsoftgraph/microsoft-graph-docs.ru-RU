---
title: Перечисление объектов managedAppStatus
description: Список свойств и связей объектов managedAppStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c264aabc08f7d7b9900b2076bcc25848a97e7ab6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354060"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="d2e17-103">Перечисление объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d2e17-103">List managedAppStatuses</span></span>

> <span data-ttu-id="d2e17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2e17-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2e17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2e17-106">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d2e17-106">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2e17-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d2e17-107">Prerequisites</span></span>
<span data-ttu-id="d2e17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e17-110">Permission type</span></span>|<span data-ttu-id="d2e17-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2e17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2e17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2e17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2e17-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2e17-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2e17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2e17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2e17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e17-115">Not supported.</span></span>|
|<span data-ttu-id="d2e17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2e17-116">Application</span></span>|<span data-ttu-id="d2e17-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2e17-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2e17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2e17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d2e17-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2e17-119">Request headers</span></span>
|<span data-ttu-id="d2e17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2e17-120">Header</span></span>|<span data-ttu-id="d2e17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2e17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2e17-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2e17-122">Authorization</span></span>|<span data-ttu-id="d2e17-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2e17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d2e17-124">Accept</span></span>|<span data-ttu-id="d2e17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2e17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2e17-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2e17-126">Request body</span></span>
<span data-ttu-id="d2e17-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2e17-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2e17-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2e17-128">Response</span></span>
<span data-ttu-id="d2e17-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2e17-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e17-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d2e17-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2e17-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e17-131">Request</span></span>
<span data-ttu-id="d2e17-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e17-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="d2e17-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e17-133">Response</span></span>
<span data-ttu-id="d2e17-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2e17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatus",
      "displayName": "Display Name value",
      "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
      "version": "Version value"
    }
  ]
}
```






