---
title: Обновление Рбакаппликатионмултипле
description: Обновление свойств объекта Рбакаппликатионмултипле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be552b43bb1e2add4f01d93c17a243e988f8ac95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031979"
---
# <a name="update-rbacapplicationmultiple"></a><span data-ttu-id="86450-103">Обновление Рбакаппликатионмултипле</span><span class="sxs-lookup"><span data-stu-id="86450-103">Update rbacApplicationMultiple</span></span>

<span data-ttu-id="86450-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86450-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86450-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86450-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86450-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86450-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86450-107">Обновление свойств объекта [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="86450-107">Update the properties of a [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86450-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86450-108">Prerequisites</span></span>
<span data-ttu-id="86450-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86450-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86450-111">Permission type</span></span>|<span data-ttu-id="86450-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86450-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86450-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86450-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86450-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86450-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="86450-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86450-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86450-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86450-116">Not supported.</span></span>|
|<span data-ttu-id="86450-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86450-117">Application</span></span>|<span data-ttu-id="86450-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86450-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86450-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86450-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="86450-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86450-120">Request headers</span></span>
|<span data-ttu-id="86450-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86450-121">Header</span></span>|<span data-ttu-id="86450-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86450-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86450-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86450-123">Authorization</span></span>|<span data-ttu-id="86450-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86450-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86450-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86450-125">Accept</span></span>|<span data-ttu-id="86450-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86450-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86450-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86450-127">Request body</span></span>
<span data-ttu-id="86450-128">В тексте запроса добавьте представление объекта [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86450-128">In the request body, supply a JSON representation for the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

<span data-ttu-id="86450-129">В следующей таблице приведены свойства, необходимые при создании [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md).</span><span class="sxs-lookup"><span data-stu-id="86450-129">The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span></span>

|<span data-ttu-id="86450-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86450-130">Property</span></span>|<span data-ttu-id="86450-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86450-131">Type</span></span>|<span data-ttu-id="86450-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86450-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86450-133">id</span><span class="sxs-lookup"><span data-stu-id="86450-133">id</span></span>|<span data-ttu-id="86450-134">String</span><span class="sxs-lookup"><span data-stu-id="86450-134">String</span></span>|<span data-ttu-id="86450-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="86450-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86450-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="86450-136">Response</span></span>
<span data-ttu-id="86450-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86450-137">If successful, this method returns a `200 OK` response code and an updated [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86450-138">Пример</span><span class="sxs-lookup"><span data-stu-id="86450-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="86450-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="86450-139">Request</span></span>
<span data-ttu-id="86450-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86450-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a><span data-ttu-id="86450-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="86450-141">Response</span></span>
<span data-ttu-id="86450-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86450-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```






