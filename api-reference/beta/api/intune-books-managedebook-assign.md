---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbe825eae1ac6fe8d5af5cef347a30fe3340956b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793215"
---
# <a name="assign-action"></a><span data-ttu-id="7a7e2-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="7a7e2-103">assign action</span></span>

<span data-ttu-id="7a7e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a7e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a7e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a7e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a7e2-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a7e2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7a7e2-108">Prerequisites</span></span>
<span data-ttu-id="7a7e2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7a7e2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a7e2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a7e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a7e2-111">Permission type</span></span>|<span data-ttu-id="7a7e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a7e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a7e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a7e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a7e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a7e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a7e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a7e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a7e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-116">Not supported.</span></span>|
|<span data-ttu-id="7a7e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a7e2-117">Application</span></span>|<span data-ttu-id="7a7e2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a7e2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a7e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a7e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7a7e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a7e2-120">Request headers</span></span>
|<span data-ttu-id="7a7e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a7e2-121">Header</span></span>|<span data-ttu-id="7a7e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a7e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a7e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a7e2-123">Authorization</span></span>|<span data-ttu-id="7a7e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a7e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a7e2-125">Accept</span></span>|<span data-ttu-id="7a7e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a7e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a7e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a7e2-127">Request body</span></span>
<span data-ttu-id="7a7e2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7a7e2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7a7e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a7e2-130">Property</span></span>|<span data-ttu-id="7a7e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a7e2-131">Type</span></span>|<span data-ttu-id="7a7e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a7e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a7e2-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="7a7e2-133">managedEBookAssignments</span></span>|<span data-ttu-id="7a7e2-134">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7a7e2-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="7a7e2-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7a7e2-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7a7e2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a7e2-136">Response</span></span>
<span data-ttu-id="7a7e2-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a7e2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7a7e2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a7e2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a7e2-139">Request</span></span>
<span data-ttu-id="7a7e2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 487

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7a7e2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a7e2-141">Response</span></span>
<span data-ttu-id="7a7e2-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-142">Here is an example of the response.</span></span> <span data-ttu-id="7a7e2-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7a7e2-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7a7e2-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



