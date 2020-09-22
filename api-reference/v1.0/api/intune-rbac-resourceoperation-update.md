---
title: Обновление объекта resourceOperation
description: Обновляет свойства объекта resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5e05a8b9bd78d6aaa7f11ea8bbf58efb313a22c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059406"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="190af-103">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="190af-103">Update resourceOperation</span></span>

<span data-ttu-id="190af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="190af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="190af-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="190af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="190af-106">Обновляет свойства объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="190af-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="190af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="190af-107">Prerequisites</span></span>
<span data-ttu-id="190af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="190af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="190af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="190af-110">Permission type</span></span>|<span data-ttu-id="190af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="190af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="190af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="190af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="190af-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="190af-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="190af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="190af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="190af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="190af-115">Not supported.</span></span>|
|<span data-ttu-id="190af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="190af-116">Application</span></span>|<span data-ttu-id="190af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="190af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="190af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="190af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="190af-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="190af-119">Request headers</span></span>
|<span data-ttu-id="190af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="190af-120">Header</span></span>|<span data-ttu-id="190af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="190af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="190af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="190af-122">Authorization</span></span>|<span data-ttu-id="190af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="190af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="190af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="190af-124">Accept</span></span>|<span data-ttu-id="190af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="190af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="190af-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="190af-126">Request body</span></span>
<span data-ttu-id="190af-127">В теле запроса добавьте представление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="190af-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="190af-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="190af-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="190af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="190af-129">Property</span></span>|<span data-ttu-id="190af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="190af-130">Type</span></span>|<span data-ttu-id="190af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="190af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="190af-132">id</span><span class="sxs-lookup"><span data-stu-id="190af-132">id</span></span>|<span data-ttu-id="190af-133">String</span><span class="sxs-lookup"><span data-stu-id="190af-133">String</span></span>|<span data-ttu-id="190af-134">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="190af-134">Key of the Resource Operation.</span></span> <span data-ttu-id="190af-135">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="190af-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="190af-136">resourceName</span><span class="sxs-lookup"><span data-stu-id="190af-136">resourceName</span></span>|<span data-ttu-id="190af-137">String</span><span class="sxs-lookup"><span data-stu-id="190af-137">String</span></span>|<span data-ttu-id="190af-138">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="190af-138">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="190af-139">actionName</span><span class="sxs-lookup"><span data-stu-id="190af-139">actionName</span></span>|<span data-ttu-id="190af-140">String</span><span class="sxs-lookup"><span data-stu-id="190af-140">String</span></span>|<span data-ttu-id="190af-141">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="190af-141">Type of action this operation is going to perform.</span></span> <span data-ttu-id="190af-142">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="190af-142">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="190af-143">description</span><span class="sxs-lookup"><span data-stu-id="190af-143">description</span></span>|<span data-ttu-id="190af-144">String</span><span class="sxs-lookup"><span data-stu-id="190af-144">String</span></span>|<span data-ttu-id="190af-145">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="190af-145">Description of the resource operation.</span></span> <span data-ttu-id="190af-146">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="190af-146">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="190af-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="190af-147">Response</span></span>
<span data-ttu-id="190af-148">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="190af-148">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="190af-149">Пример</span><span class="sxs-lookup"><span data-stu-id="190af-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="190af-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="190af-150">Request</span></span>
<span data-ttu-id="190af-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="190af-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="190af-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="190af-152">Response</span></span>
<span data-ttu-id="190af-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="190af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```









