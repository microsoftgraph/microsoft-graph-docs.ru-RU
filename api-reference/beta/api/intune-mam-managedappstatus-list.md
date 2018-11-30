---
title: Перечисление объектов managedAppStatus
description: Список свойств и связей объектов managedAppStatus.
ms.openlocfilehash: ceea2e47688d7bc7d6e6aee0ed682c36fd45fa0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082019"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="129c4-103">Перечисление объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="129c4-103">List managedAppStatuses</span></span>

> <span data-ttu-id="129c4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="129c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="129c4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="129c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="129c4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="129c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="129c4-107">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="129c4-107">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="129c4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="129c4-108">Prerequisites</span></span>
<span data-ttu-id="129c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="129c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="129c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="129c4-111">Permission type</span></span>|<span data-ttu-id="129c4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="129c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="129c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="129c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="129c4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="129c4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="129c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="129c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="129c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="129c4-116">Not supported.</span></span>|
|<span data-ttu-id="129c4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="129c4-117">Application</span></span>|<span data-ttu-id="129c4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="129c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="129c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="129c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="129c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="129c4-120">Request headers</span></span>
|<span data-ttu-id="129c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="129c4-121">Header</span></span>|<span data-ttu-id="129c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="129c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="129c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="129c4-123">Authorization</span></span>|<span data-ttu-id="129c4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="129c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="129c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="129c4-125">Accept</span></span>|<span data-ttu-id="129c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="129c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="129c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="129c4-127">Request body</span></span>
<span data-ttu-id="129c4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="129c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="129c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="129c4-129">Response</span></span>
<span data-ttu-id="129c4-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="129c4-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="129c4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="129c4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="129c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="129c4-132">Request</span></span>
<span data-ttu-id="129c4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="129c4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="129c4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="129c4-134">Response</span></span>
<span data-ttu-id="129c4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="129c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





