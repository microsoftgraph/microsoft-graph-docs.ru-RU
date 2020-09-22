---
title: Перечисление объектов managedAppStatus
description: Список свойств и связей объектов managedAppStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cda28d64e5b673640353625438aaa48bd7f5ab3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065104"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="29df2-103">Перечисление объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="29df2-103">List managedAppStatuses</span></span>

<span data-ttu-id="29df2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29df2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29df2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29df2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29df2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29df2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29df2-107">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="29df2-107">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29df2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="29df2-108">Prerequisites</span></span>
<span data-ttu-id="29df2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29df2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29df2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29df2-111">Permission type</span></span>|<span data-ttu-id="29df2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29df2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29df2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29df2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29df2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29df2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="29df2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29df2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29df2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29df2-116">Not supported.</span></span>|
|<span data-ttu-id="29df2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29df2-117">Application</span></span>|<span data-ttu-id="29df2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29df2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29df2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29df2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="29df2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="29df2-120">Request headers</span></span>
|<span data-ttu-id="29df2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29df2-121">Header</span></span>|<span data-ttu-id="29df2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="29df2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29df2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29df2-123">Authorization</span></span>|<span data-ttu-id="29df2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29df2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29df2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29df2-125">Accept</span></span>|<span data-ttu-id="29df2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29df2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29df2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29df2-127">Request body</span></span>
<span data-ttu-id="29df2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29df2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29df2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="29df2-129">Response</span></span>
<span data-ttu-id="29df2-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="29df2-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29df2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="29df2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="29df2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="29df2-132">Request</span></span>
<span data-ttu-id="29df2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29df2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="29df2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="29df2-134">Response</span></span>
<span data-ttu-id="29df2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29df2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






