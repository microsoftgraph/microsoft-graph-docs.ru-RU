---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38d3822bcc48312a8e7b5093b889cdd308dceedf
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43452619"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="66eba-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="66eba-103">Create resourceOperation</span></span>

<span data-ttu-id="66eba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66eba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66eba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66eba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66eba-106">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="66eba-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66eba-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66eba-107">Prerequisites</span></span>
<span data-ttu-id="66eba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66eba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66eba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66eba-110">Permission type</span></span>|<span data-ttu-id="66eba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66eba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66eba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66eba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66eba-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66eba-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="66eba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66eba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66eba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66eba-115">Not supported.</span></span>|
|<span data-ttu-id="66eba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66eba-116">Application</span></span>|<span data-ttu-id="66eba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66eba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66eba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66eba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="66eba-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66eba-119">Request headers</span></span>
|<span data-ttu-id="66eba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66eba-120">Header</span></span>|<span data-ttu-id="66eba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="66eba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66eba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66eba-122">Authorization</span></span>|<span data-ttu-id="66eba-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66eba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66eba-124">Accept</span><span class="sxs-lookup"><span data-stu-id="66eba-124">Accept</span></span>|<span data-ttu-id="66eba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66eba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66eba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66eba-126">Request body</span></span>
<span data-ttu-id="66eba-127">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66eba-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="66eba-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="66eba-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="66eba-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="66eba-129">Property</span></span>|<span data-ttu-id="66eba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="66eba-130">Type</span></span>|<span data-ttu-id="66eba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="66eba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66eba-132">id</span><span class="sxs-lookup"><span data-stu-id="66eba-132">id</span></span>|<span data-ttu-id="66eba-133">Строка</span><span class="sxs-lookup"><span data-stu-id="66eba-133">String</span></span>|<span data-ttu-id="66eba-134">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="66eba-134">Key of the Resource Operation.</span></span> <span data-ttu-id="66eba-135">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="66eba-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="66eba-136">resourceName</span><span class="sxs-lookup"><span data-stu-id="66eba-136">resourceName</span></span>|<span data-ttu-id="66eba-137">String</span><span class="sxs-lookup"><span data-stu-id="66eba-137">String</span></span>|<span data-ttu-id="66eba-138">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="66eba-138">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="66eba-139">actionName</span><span class="sxs-lookup"><span data-stu-id="66eba-139">actionName</span></span>|<span data-ttu-id="66eba-140">String</span><span class="sxs-lookup"><span data-stu-id="66eba-140">String</span></span>|<span data-ttu-id="66eba-141">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="66eba-141">Type of action this operation is going to perform.</span></span> <span data-ttu-id="66eba-142">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="66eba-142">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="66eba-143">description</span><span class="sxs-lookup"><span data-stu-id="66eba-143">description</span></span>|<span data-ttu-id="66eba-144">String</span><span class="sxs-lookup"><span data-stu-id="66eba-144">String</span></span>|<span data-ttu-id="66eba-145">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="66eba-145">Description of the resource operation.</span></span> <span data-ttu-id="66eba-146">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="66eba-146">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="66eba-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="66eba-147">Response</span></span>
<span data-ttu-id="66eba-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="66eba-148">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66eba-149">Пример</span><span class="sxs-lookup"><span data-stu-id="66eba-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="66eba-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="66eba-150">Request</span></span>
<span data-ttu-id="66eba-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66eba-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="66eba-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="66eba-152">Response</span></span>
<span data-ttu-id="66eba-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66eba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






