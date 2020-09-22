---
title: Перечисление объектов managedEBookAssignment
description: Список свойств и связей объектов managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd19e8aefe2ab123f4cffc751028f047f3a3f9e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077809"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="f8818-103">Перечисление объектов managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="f8818-103">List managedEBookAssignments</span></span>

<span data-ttu-id="f8818-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8818-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8818-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8818-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8818-106">Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8818-106">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8818-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8818-107">Prerequisites</span></span>
<span data-ttu-id="f8818-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8818-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8818-110">Permission type</span></span>|<span data-ttu-id="f8818-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8818-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8818-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8818-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8818-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8818-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8818-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8818-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8818-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8818-115">Not supported.</span></span>|
|<span data-ttu-id="f8818-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8818-116">Application</span></span>|<span data-ttu-id="f8818-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8818-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8818-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8818-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f8818-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8818-119">Request headers</span></span>
|<span data-ttu-id="f8818-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8818-120">Header</span></span>|<span data-ttu-id="f8818-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8818-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8818-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8818-122">Authorization</span></span>|<span data-ttu-id="f8818-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8818-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8818-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8818-124">Accept</span></span>|<span data-ttu-id="f8818-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8818-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8818-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8818-126">Request body</span></span>
<span data-ttu-id="f8818-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8818-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8818-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8818-128">Response</span></span>
<span data-ttu-id="f8818-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8818-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8818-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f8818-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8818-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8818-131">Request</span></span>
<span data-ttu-id="f8818-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8818-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="f8818-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8818-133">Response</span></span>
<span data-ttu-id="f8818-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```









