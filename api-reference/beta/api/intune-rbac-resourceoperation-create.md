---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed4978f42ed8f336720a9bc6458640111590d71f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148479"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="58294-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="58294-103">Create resourceOperation</span></span>

<span data-ttu-id="58294-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58294-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58294-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58294-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58294-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58294-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58294-107">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="58294-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58294-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58294-108">Prerequisites</span></span>
<span data-ttu-id="58294-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58294-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58294-111">Permission type</span></span>|<span data-ttu-id="58294-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58294-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58294-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58294-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58294-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58294-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="58294-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58294-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58294-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58294-116">Not supported.</span></span>|
|<span data-ttu-id="58294-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="58294-117">Application</span></span>|<span data-ttu-id="58294-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58294-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58294-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58294-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="58294-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58294-120">Request headers</span></span>
|<span data-ttu-id="58294-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58294-121">Header</span></span>|<span data-ttu-id="58294-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58294-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58294-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58294-123">Authorization</span></span>|<span data-ttu-id="58294-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58294-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58294-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58294-125">Accept</span></span>|<span data-ttu-id="58294-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58294-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58294-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58294-127">Request body</span></span>
<span data-ttu-id="58294-128">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58294-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="58294-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="58294-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="58294-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="58294-130">Property</span></span>|<span data-ttu-id="58294-131">Тип</span><span class="sxs-lookup"><span data-stu-id="58294-131">Type</span></span>|<span data-ttu-id="58294-132">Описание</span><span class="sxs-lookup"><span data-stu-id="58294-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58294-133">id</span><span class="sxs-lookup"><span data-stu-id="58294-133">id</span></span>|<span data-ttu-id="58294-134">Строка</span><span class="sxs-lookup"><span data-stu-id="58294-134">String</span></span>|<span data-ttu-id="58294-135">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="58294-135">Key of the Resource Operation.</span></span> <span data-ttu-id="58294-136">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="58294-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="58294-137">resource</span><span class="sxs-lookup"><span data-stu-id="58294-137">resource</span></span>|<span data-ttu-id="58294-138">Строка</span><span class="sxs-lookup"><span data-stu-id="58294-138">String</span></span>|<span data-ttu-id="58294-139">Категория ресурсов, к которой относится эта операция.</span><span class="sxs-lookup"><span data-stu-id="58294-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="58294-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="58294-140">resourceName</span></span>|<span data-ttu-id="58294-141">String</span><span class="sxs-lookup"><span data-stu-id="58294-141">String</span></span>|<span data-ttu-id="58294-142">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="58294-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="58294-143">actionName</span><span class="sxs-lookup"><span data-stu-id="58294-143">actionName</span></span>|<span data-ttu-id="58294-144">String</span><span class="sxs-lookup"><span data-stu-id="58294-144">String</span></span>|<span data-ttu-id="58294-145">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="58294-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="58294-146">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="58294-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="58294-147">description</span><span class="sxs-lookup"><span data-stu-id="58294-147">description</span></span>|<span data-ttu-id="58294-148">Строка</span><span class="sxs-lookup"><span data-stu-id="58294-148">String</span></span>|<span data-ttu-id="58294-149">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="58294-149">Description of the resource operation.</span></span> <span data-ttu-id="58294-150">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="58294-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="58294-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="58294-151">enabledForScopeValidation</span></span>|<span data-ttu-id="58294-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="58294-152">Boolean</span></span>|<span data-ttu-id="58294-153">Определяет, проверяется ли разрешение для областей, определенных для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="58294-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="58294-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="58294-154">Response</span></span>
<span data-ttu-id="58294-155">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58294-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58294-156">Пример</span><span class="sxs-lookup"><span data-stu-id="58294-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="58294-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="58294-157">Request</span></span>
<span data-ttu-id="58294-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58294-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="58294-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="58294-159">Response</span></span>
<span data-ttu-id="58294-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58294-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```




