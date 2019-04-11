---
title: Перечисление объектов managedAppStatusRaw
description: Список свойств и связей объектов managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7d282d6cee917f2ea6a5bd01f5256cad044ffb4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776691"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="57286-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="57286-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="57286-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57286-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57286-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57286-106">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="57286-106">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57286-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="57286-107">Prerequisites</span></span>
<span data-ttu-id="57286-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57286-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57286-110">Permission type</span></span>|<span data-ttu-id="57286-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57286-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57286-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57286-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57286-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="57286-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="57286-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57286-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57286-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57286-115">Not supported.</span></span>|
|<span data-ttu-id="57286-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57286-116">Application</span></span>|<span data-ttu-id="57286-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57286-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57286-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57286-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="57286-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57286-119">Request headers</span></span>
|<span data-ttu-id="57286-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57286-120">Header</span></span>|<span data-ttu-id="57286-121">Значение</span><span class="sxs-lookup"><span data-stu-id="57286-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57286-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57286-122">Authorization</span></span>|<span data-ttu-id="57286-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57286-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57286-124">Accept</span><span class="sxs-lookup"><span data-stu-id="57286-124">Accept</span></span>|<span data-ttu-id="57286-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57286-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57286-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57286-126">Request body</span></span>
<span data-ttu-id="57286-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57286-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57286-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="57286-128">Response</span></span>
<span data-ttu-id="57286-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="57286-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57286-130">Пример</span><span class="sxs-lookup"><span data-stu-id="57286-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="57286-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="57286-131">Request</span></span>
<span data-ttu-id="57286-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57286-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="57286-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="57286-133">Response</span></span>
<span data-ttu-id="57286-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57286-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```





