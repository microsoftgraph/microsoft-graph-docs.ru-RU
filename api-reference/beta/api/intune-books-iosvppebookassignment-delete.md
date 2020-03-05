---
title: Удаление объекта iosVppEBookAssignment
description: Удаляет объект iosVppEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ff424ecfc465d7d0d89d29687b4a77dd882204f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450337"
---
# <a name="delete-iosvppebookassignment"></a><span data-ttu-id="0509f-103">Удаление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="0509f-103">Delete iosVppEBookAssignment</span></span>

<span data-ttu-id="0509f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0509f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0509f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0509f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0509f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0509f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0509f-107">Удаляет объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0509f-107">Deletes a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0509f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0509f-108">Prerequisites</span></span>
<span data-ttu-id="0509f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0509f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0509f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0509f-111">Permission type</span></span>|<span data-ttu-id="0509f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0509f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0509f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0509f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0509f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0509f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0509f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0509f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0509f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0509f-116">Not supported.</span></span>|
|<span data-ttu-id="0509f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0509f-117">Application</span></span>|<span data-ttu-id="0509f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0509f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0509f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0509f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0509f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0509f-120">Request headers</span></span>
|<span data-ttu-id="0509f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0509f-121">Header</span></span>|<span data-ttu-id="0509f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0509f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0509f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0509f-123">Authorization</span></span>|<span data-ttu-id="0509f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0509f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0509f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0509f-125">Accept</span></span>|<span data-ttu-id="0509f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0509f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0509f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0509f-127">Request body</span></span>
<span data-ttu-id="0509f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0509f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0509f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0509f-129">Response</span></span>
<span data-ttu-id="0509f-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0509f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0509f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0509f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0509f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0509f-132">Request</span></span>
<span data-ttu-id="0509f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0509f-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0509f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0509f-134">Response</span></span>
<span data-ttu-id="0509f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0509f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





