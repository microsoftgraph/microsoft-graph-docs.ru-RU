---
title: проверка действияFilter
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b07fd067ababeb40ff290ff7047b6be125acdf03
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125242"
---
# <a name="validatefilter-action"></a><span data-ttu-id="483e2-103">проверка действияFilter</span><span class="sxs-lookup"><span data-stu-id="483e2-103">validateFilter action</span></span>

<span data-ttu-id="483e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="483e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="483e2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="483e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="483e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="483e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="483e2-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="483e2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="483e2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="483e2-108">Prerequisites</span></span>
<span data-ttu-id="483e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="483e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="483e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="483e2-111">Permission type</span></span>|<span data-ttu-id="483e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="483e2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="483e2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="483e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="483e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="483e2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="483e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="483e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="483e2-116">Not supported.</span></span>|
|<span data-ttu-id="483e2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="483e2-117">Application</span></span>|<span data-ttu-id="483e2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483e2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="483e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="483e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters/validateFilter
```

## <a name="request-headers"></a><span data-ttu-id="483e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="483e2-120">Request headers</span></span>
|<span data-ttu-id="483e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="483e2-121">Header</span></span>|<span data-ttu-id="483e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="483e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="483e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="483e2-123">Authorization</span></span>|<span data-ttu-id="483e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="483e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="483e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="483e2-125">Accept</span></span>|<span data-ttu-id="483e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="483e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="483e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="483e2-127">Request body</span></span>
<span data-ttu-id="483e2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="483e2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="483e2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="483e2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="483e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="483e2-130">Property</span></span>|<span data-ttu-id="483e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="483e2-131">Type</span></span>|<span data-ttu-id="483e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="483e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="483e2-133">deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="483e2-133">deviceAndAppManagementAssignmentFilter</span></span>|[<span data-ttu-id="483e2-134">deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="483e2-134">deviceAndAppManagementAssignmentFilter</span></span>](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|<span data-ttu-id="483e2-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="483e2-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="483e2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="483e2-136">Response</span></span>
<span data-ttu-id="483e2-137">В случае успешного выполнения это действие возвращает код ответа и `200 OK` [назначениеFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="483e2-137">If successful, this action returns a `200 OK` response code and a [assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483e2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="483e2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="483e2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="483e2-139">Request</span></span>
<span data-ttu-id="483e2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="483e2-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/validateFilter

Content-type: application/json
Content-length: 520

{
  "deviceAndAppManagementAssignmentFilter": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
    "id": "819818db-18db-8198-db18-9881db189881",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "platform": "androidForWork",
    "rule": "Rule value",
    "roleScopeTags": [
      "Role Scope Tags value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="483e2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="483e2-141">Response</span></span>
<span data-ttu-id="483e2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="483e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterValidationResult",
    "isValidRule": true
  }
}
```




