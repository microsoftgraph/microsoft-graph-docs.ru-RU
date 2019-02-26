---
title: Перечисление объектов managedAppStatusRaw
description: Перечисление свойств и связей объектов managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95a0f2dc4387a38f2d9f0d478c349a775b4c0403
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152852"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="9104c-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9104c-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="9104c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9104c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9104c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9104c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9104c-106">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9104c-106">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9104c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9104c-107">Prerequisites</span></span>
<span data-ttu-id="9104c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9104c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9104c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9104c-110">Permission type</span></span>|<span data-ttu-id="9104c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9104c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9104c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9104c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9104c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9104c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9104c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9104c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9104c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9104c-115">Not supported.</span></span>|
|<span data-ttu-id="9104c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9104c-116">Application</span></span>|<span data-ttu-id="9104c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9104c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9104c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9104c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9104c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9104c-119">Request headers</span></span>
|<span data-ttu-id="9104c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9104c-120">Header</span></span>|<span data-ttu-id="9104c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9104c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9104c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9104c-122">Authorization</span></span>|<span data-ttu-id="9104c-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9104c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9104c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9104c-124">Accept</span></span>|<span data-ttu-id="9104c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9104c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9104c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9104c-126">Request body</span></span>
<span data-ttu-id="9104c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9104c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9104c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9104c-128">Response</span></span>
<span data-ttu-id="9104c-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9104c-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9104c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9104c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9104c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9104c-131">Request</span></span>
<span data-ttu-id="9104c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9104c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="9104c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9104c-133">Response</span></span>
<span data-ttu-id="9104c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9104c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




