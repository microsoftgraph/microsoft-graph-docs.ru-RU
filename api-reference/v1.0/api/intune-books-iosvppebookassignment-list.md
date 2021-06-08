---
title: Перечисление объектов iosVppEBookAssignment
description: Список свойств и связей объектов iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b8844796f92ed289bb6ff7afba65923ae312f1a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758458"
---
# <a name="list-iosvppebookassignments"></a><span data-ttu-id="c5091-103">Перечисление объектов iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="c5091-103">List iosVppEBookAssignments</span></span>

<span data-ttu-id="c5091-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5091-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5091-106">Список свойств и связей объектов [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5091-106">List properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5091-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5091-107">Prerequisites</span></span>
<span data-ttu-id="c5091-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5091-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5091-110">Permission type</span></span>|<span data-ttu-id="c5091-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5091-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5091-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5091-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5091-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5091-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5091-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5091-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5091-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5091-115">Not supported.</span></span>|
|<span data-ttu-id="c5091-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c5091-116">Application</span></span>|<span data-ttu-id="c5091-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5091-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5091-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5091-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c5091-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5091-119">Request headers</span></span>
|<span data-ttu-id="c5091-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5091-120">Header</span></span>|<span data-ttu-id="c5091-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c5091-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5091-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5091-122">Authorization</span></span>|<span data-ttu-id="c5091-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5091-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5091-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c5091-124">Accept</span></span>|<span data-ttu-id="c5091-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5091-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5091-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5091-126">Request body</span></span>
<span data-ttu-id="c5091-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5091-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5091-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5091-128">Response</span></span>
<span data-ttu-id="c5091-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5091-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5091-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c5091-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5091-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5091-131">Request</span></span>
<span data-ttu-id="c5091-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5091-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="c5091-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5091-133">Response</span></span>
<span data-ttu-id="c5091-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5091-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
      "id": "48f05789-5789-48f0-8957-f0488957f048",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```




