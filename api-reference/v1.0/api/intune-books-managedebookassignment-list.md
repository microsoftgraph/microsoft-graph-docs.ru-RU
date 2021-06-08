---
title: Перечисление объектов managedEBookAssignment
description: Список свойств и связей объектов managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ae1ea6e8e5e2584237f77f0d4303f44f36fc57f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757243"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="53f69-103">Перечисление объектов managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="53f69-103">List managedEBookAssignments</span></span>

<span data-ttu-id="53f69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53f69-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53f69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f69-106">Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="53f69-106">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53f69-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53f69-107">Prerequisites</span></span>
<span data-ttu-id="53f69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53f69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53f69-110">Permission type</span></span>|<span data-ttu-id="53f69-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53f69-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53f69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53f69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53f69-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f69-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53f69-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53f69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53f69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53f69-115">Not supported.</span></span>|
|<span data-ttu-id="53f69-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="53f69-116">Application</span></span>|<span data-ttu-id="53f69-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f69-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53f69-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53f69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="53f69-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53f69-119">Request headers</span></span>
|<span data-ttu-id="53f69-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53f69-120">Header</span></span>|<span data-ttu-id="53f69-121">Значение</span><span class="sxs-lookup"><span data-stu-id="53f69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53f69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f69-122">Authorization</span></span>|<span data-ttu-id="53f69-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53f69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53f69-124">Accept</span><span class="sxs-lookup"><span data-stu-id="53f69-124">Accept</span></span>|<span data-ttu-id="53f69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53f69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f69-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53f69-126">Request body</span></span>
<span data-ttu-id="53f69-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53f69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53f69-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="53f69-128">Response</span></span>
<span data-ttu-id="53f69-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53f69-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53f69-130">Пример</span><span class="sxs-lookup"><span data-stu-id="53f69-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="53f69-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="53f69-131">Request</span></span>
<span data-ttu-id="53f69-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53f69-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="53f69-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="53f69-133">Response</span></span>
<span data-ttu-id="53f69-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53f69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```




