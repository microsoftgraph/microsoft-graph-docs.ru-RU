---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
ms.openlocfilehash: b73e616735ca3f096c01a9f7eba8a7d751bb7160
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076005"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="3c97d-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="3c97d-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="3c97d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c97d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c97d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c97d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c97d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c97d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c97d-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="3c97d-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c97d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3c97d-108">Prerequisites</span></span>

<span data-ttu-id="3c97d-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="3c97d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3c97d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c97d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="3c97d-111">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="3c97d-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="3c97d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c97d-112">Permission type</span></span>|<span data-ttu-id="3c97d-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c97d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="3c97d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c97d-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="3c97d-115">&nbsp;&nbsp; **Приложений**, **книги**или **адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="3c97d-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="3c97d-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="3c97d-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="3c97d-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="3c97d-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3c97d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c97d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="3c97d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c97d-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c97d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c97d-120">Not supported.</span></span>|
|<span data-ttu-id="3c97d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c97d-121">Application</span></span>|<span data-ttu-id="3c97d-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c97d-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c97d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c97d-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c97d-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c97d-124">Optional query parameters</span></span>

<span data-ttu-id="3c97d-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c97d-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c97d-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c97d-126">Request headers</span></span>

|<span data-ttu-id="3c97d-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c97d-127">Header</span></span>|<span data-ttu-id="3c97d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="3c97d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c97d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c97d-129">Authorization</span></span>|<span data-ttu-id="3c97d-130">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c97d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c97d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="3c97d-131">Accept</span></span>|<span data-ttu-id="3c97d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="3c97d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c97d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c97d-133">Request body</span></span>

<span data-ttu-id="3c97d-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c97d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c97d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c97d-135">Response</span></span>

<span data-ttu-id="3c97d-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c97d-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c97d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="3c97d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c97d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c97d-138">Request</span></span>

<span data-ttu-id="3c97d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c97d-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="3c97d-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c97d-140">Response</span></span>

<span data-ttu-id="3c97d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3c97d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



