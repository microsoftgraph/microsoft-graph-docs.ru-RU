---
title: Удаление Команажементелигибледевице
description: Удаляет объект Команажементелигибледевице.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d263ad2bfed8de4331253ce4cbd04b529cace0bb
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792543"
---
# <a name="delete-comanagementeligibledevice"></a><span data-ttu-id="3f249-103">Удаление Команажементелигибледевице</span><span class="sxs-lookup"><span data-stu-id="3f249-103">Delete comanagementEligibleDevice</span></span>

<span data-ttu-id="3f249-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f249-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f249-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f249-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f249-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f249-107">Удаляет объект [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md).</span><span class="sxs-lookup"><span data-stu-id="3f249-107">Deletes a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f249-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f249-108">Prerequisites</span></span>
<span data-ttu-id="3f249-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3f249-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3f249-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f249-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f249-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f249-111">Permission type</span></span>|<span data-ttu-id="3f249-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f249-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f249-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f249-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f249-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f249-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3f249-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f249-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f249-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f249-116">Not supported.</span></span>|
|<span data-ttu-id="3f249-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f249-117">Application</span></span>|<span data-ttu-id="3f249-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f249-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f249-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f249-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="3f249-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f249-120">Request headers</span></span>
|<span data-ttu-id="3f249-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f249-121">Header</span></span>|<span data-ttu-id="3f249-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f249-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f249-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f249-123">Authorization</span></span>|<span data-ttu-id="3f249-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f249-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f249-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f249-125">Accept</span></span>|<span data-ttu-id="3f249-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f249-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f249-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f249-127">Request body</span></span>
<span data-ttu-id="3f249-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f249-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f249-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f249-129">Response</span></span>
<span data-ttu-id="3f249-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3f249-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3f249-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3f249-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f249-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f249-132">Request</span></span>
<span data-ttu-id="3f249-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f249-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

### <a name="response"></a><span data-ttu-id="3f249-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f249-134">Response</span></span>
<span data-ttu-id="3f249-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3f249-135">Here is an example of the response.</span></span> <span data-ttu-id="3f249-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3f249-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3f249-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3f249-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



