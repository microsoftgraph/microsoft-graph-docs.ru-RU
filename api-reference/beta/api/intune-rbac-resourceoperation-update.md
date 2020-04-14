---
title: Обновление объекта resourceOperation
description: Обновляет свойства объекта resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6afbcc8a3b6adc0ade92e17588377e220c247f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421090"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="68831-103">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="68831-103">Update resourceOperation</span></span>

<span data-ttu-id="68831-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68831-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68831-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68831-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68831-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68831-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68831-107">Обновляет свойства объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="68831-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68831-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68831-108">Prerequisites</span></span>
<span data-ttu-id="68831-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68831-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68831-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68831-111">Permission type</span></span>|<span data-ttu-id="68831-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68831-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68831-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68831-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68831-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68831-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="68831-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68831-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68831-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68831-116">Not supported.</span></span>|
|<span data-ttu-id="68831-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="68831-117">Application</span></span>|<span data-ttu-id="68831-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68831-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68831-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68831-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="68831-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68831-120">Request headers</span></span>
|<span data-ttu-id="68831-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68831-121">Header</span></span>|<span data-ttu-id="68831-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68831-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68831-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68831-123">Authorization</span></span>|<span data-ttu-id="68831-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68831-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68831-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68831-125">Accept</span></span>|<span data-ttu-id="68831-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68831-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68831-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68831-127">Request body</span></span>
<span data-ttu-id="68831-128">В теле запроса добавьте представление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68831-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="68831-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="68831-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="68831-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68831-130">Property</span></span>|<span data-ttu-id="68831-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68831-131">Type</span></span>|<span data-ttu-id="68831-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68831-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68831-133">id</span><span class="sxs-lookup"><span data-stu-id="68831-133">id</span></span>|<span data-ttu-id="68831-134">Строка</span><span class="sxs-lookup"><span data-stu-id="68831-134">String</span></span>|<span data-ttu-id="68831-135">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="68831-135">Key of the Resource Operation.</span></span> <span data-ttu-id="68831-136">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="68831-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="68831-137">resource</span><span class="sxs-lookup"><span data-stu-id="68831-137">resource</span></span>|<span data-ttu-id="68831-138">String</span><span class="sxs-lookup"><span data-stu-id="68831-138">String</span></span>|<span data-ttu-id="68831-139">Категория ресурса, к которой относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="68831-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="68831-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="68831-140">resourceName</span></span>|<span data-ttu-id="68831-141">String</span><span class="sxs-lookup"><span data-stu-id="68831-141">String</span></span>|<span data-ttu-id="68831-142">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="68831-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="68831-143">actionName</span><span class="sxs-lookup"><span data-stu-id="68831-143">actionName</span></span>|<span data-ttu-id="68831-144">String</span><span class="sxs-lookup"><span data-stu-id="68831-144">String</span></span>|<span data-ttu-id="68831-145">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="68831-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="68831-146">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="68831-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="68831-147">description</span><span class="sxs-lookup"><span data-stu-id="68831-147">description</span></span>|<span data-ttu-id="68831-148">String</span><span class="sxs-lookup"><span data-stu-id="68831-148">String</span></span>|<span data-ttu-id="68831-149">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="68831-149">Description of the resource operation.</span></span> <span data-ttu-id="68831-150">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="68831-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="68831-151">енабледфорскопевалидатион</span><span class="sxs-lookup"><span data-stu-id="68831-151">enabledForScopeValidation</span></span>|<span data-ttu-id="68831-152">Логическое</span><span class="sxs-lookup"><span data-stu-id="68831-152">Boolean</span></span>|<span data-ttu-id="68831-153">Определяет, является ли разрешение проверенным для областей, определенных для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="68831-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="68831-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="68831-154">Response</span></span>
<span data-ttu-id="68831-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="68831-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68831-156">Пример</span><span class="sxs-lookup"><span data-stu-id="68831-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="68831-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="68831-157">Request</span></span>
<span data-ttu-id="68831-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68831-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
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

### <a name="response"></a><span data-ttu-id="68831-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="68831-159">Response</span></span>
<span data-ttu-id="68831-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68831-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



