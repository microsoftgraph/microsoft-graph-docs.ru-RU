---
title: Список remoteActionAudits
description: Свойства списка и связей объектов remoteActionAudit.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6de4fdfd13e750fa06afa1436db1d4140152e312
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847449"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="23201-103">Список remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="23201-103">List remoteActionAudits</span></span>

> <span data-ttu-id="23201-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23201-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23201-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23201-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23201-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23201-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23201-107">Свойства списка и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="23201-107">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23201-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23201-108">Prerequisites</span></span>
<span data-ttu-id="23201-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23201-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23201-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23201-111">Permission type</span></span>|<span data-ttu-id="23201-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23201-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23201-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23201-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23201-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="23201-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="23201-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23201-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23201-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23201-116">Not supported.</span></span>|
|<span data-ttu-id="23201-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23201-117">Application</span></span>|<span data-ttu-id="23201-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23201-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23201-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23201-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="23201-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23201-120">Request headers</span></span>
|<span data-ttu-id="23201-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23201-121">Header</span></span>|<span data-ttu-id="23201-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23201-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23201-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23201-123">Authorization</span></span>|<span data-ttu-id="23201-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="23201-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23201-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23201-125">Accept</span></span>|<span data-ttu-id="23201-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23201-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23201-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23201-127">Request body</span></span>
<span data-ttu-id="23201-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23201-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23201-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="23201-129">Response</span></span>
<span data-ttu-id="23201-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="23201-130">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23201-131">Пример</span><span class="sxs-lookup"><span data-stu-id="23201-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="23201-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="23201-132">Request</span></span>
<span data-ttu-id="23201-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23201-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="23201-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="23201-134">Response</span></span>
<span data-ttu-id="23201-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23201-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteActionAudit",
      "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
      "action": "factoryReset",
      "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
      "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
      "deviceIMEI": "Device IMEI value",
      "actionState": "pending"
    }
  ]
}
```





