---
title: Удаление объекта deviceAndAppManagementRoleAssignment
description: Удаление объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd9a05fc6e126a5647a49e5c9d107ae2b857fd3a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158509"
---
# <a name="delete-deviceandappmanagementroleassignment"></a><span data-ttu-id="37727-103">Удаление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="37727-103">Delete deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="37727-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37727-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37727-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37727-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37727-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37727-107">Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37727-107">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37727-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37727-108">Prerequisites</span></span>
<span data-ttu-id="37727-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37727-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37727-111">Permission type</span></span>|<span data-ttu-id="37727-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37727-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37727-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37727-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37727-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="37727-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37727-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37727-116">Not supported.</span></span>|
|<span data-ttu-id="37727-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="37727-117">Application</span></span>|<span data-ttu-id="37727-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37727-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37727-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="37727-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37727-120">Request headers</span></span>
|<span data-ttu-id="37727-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37727-121">Header</span></span>|<span data-ttu-id="37727-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37727-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37727-123">Authorization</span></span>|<span data-ttu-id="37727-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37727-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37727-125">Accept</span></span>|<span data-ttu-id="37727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37727-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37727-127">Request body</span></span>
<span data-ttu-id="37727-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37727-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37727-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="37727-129">Response</span></span>
<span data-ttu-id="37727-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37727-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37727-131">Пример</span><span class="sxs-lookup"><span data-stu-id="37727-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="37727-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="37727-132">Request</span></span>
<span data-ttu-id="37727-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37727-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="37727-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37727-134">Response</span></span>
<span data-ttu-id="37727-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37727-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




