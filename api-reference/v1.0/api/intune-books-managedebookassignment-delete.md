---
title: Удаление объекта managedEBookAssignment
description: Удаляет объект managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9cdae4405b288185cb1966d7ee254146d559e8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077872"
---
# <a name="delete-managedebookassignment"></a><span data-ttu-id="2dc95-103">Удаление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="2dc95-103">Delete managedEBookAssignment</span></span>

<span data-ttu-id="2dc95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dc95-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2dc95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dc95-106">Удаляет объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2dc95-106">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dc95-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2dc95-107">Prerequisites</span></span>
<span data-ttu-id="2dc95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dc95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dc95-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2dc95-110">Permission type</span></span>|<span data-ttu-id="2dc95-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2dc95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dc95-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2dc95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2dc95-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dc95-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2dc95-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2dc95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dc95-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dc95-115">Not supported.</span></span>|
|<span data-ttu-id="2dc95-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2dc95-116">Application</span></span>|<span data-ttu-id="2dc95-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dc95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dc95-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2dc95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2dc95-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2dc95-119">Request headers</span></span>
|<span data-ttu-id="2dc95-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2dc95-120">Header</span></span>|<span data-ttu-id="2dc95-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2dc95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dc95-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2dc95-122">Authorization</span></span>|<span data-ttu-id="2dc95-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dc95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dc95-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2dc95-124">Accept</span></span>|<span data-ttu-id="2dc95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2dc95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dc95-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2dc95-126">Request body</span></span>
<span data-ttu-id="2dc95-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2dc95-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dc95-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dc95-128">Response</span></span>
<span data-ttu-id="2dc95-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2dc95-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2dc95-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2dc95-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dc95-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dc95-131">Request</span></span>
<span data-ttu-id="2dc95-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2dc95-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2dc95-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dc95-133">Response</span></span>
<span data-ttu-id="2dc95-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2dc95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









