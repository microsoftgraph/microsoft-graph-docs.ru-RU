---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a66d2ed153a18f62f449a352966f6bec07079d6
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43421151"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="607e3-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="607e3-103">Create resourceOperation</span></span>

<span data-ttu-id="607e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="607e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="607e3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="607e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="607e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="607e3-107">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="607e3-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="607e3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="607e3-108">Prerequisites</span></span>
<span data-ttu-id="607e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="607e3-111">Permission type</span></span>|<span data-ttu-id="607e3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="607e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="607e3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="607e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="607e3-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607e3-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="607e3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="607e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="607e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607e3-116">Not supported.</span></span>|
|<span data-ttu-id="607e3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="607e3-117">Application</span></span>|<span data-ttu-id="607e3-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607e3-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="607e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="607e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="607e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="607e3-120">Request headers</span></span>
|<span data-ttu-id="607e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="607e3-121">Header</span></span>|<span data-ttu-id="607e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="607e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="607e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="607e3-123">Authorization</span></span>|<span data-ttu-id="607e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="607e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="607e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="607e3-125">Accept</span></span>|<span data-ttu-id="607e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="607e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="607e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="607e3-127">Request body</span></span>
<span data-ttu-id="607e3-128">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="607e3-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="607e3-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="607e3-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="607e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="607e3-130">Property</span></span>|<span data-ttu-id="607e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="607e3-131">Type</span></span>|<span data-ttu-id="607e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="607e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="607e3-133">id</span><span class="sxs-lookup"><span data-stu-id="607e3-133">id</span></span>|<span data-ttu-id="607e3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="607e3-134">String</span></span>|<span data-ttu-id="607e3-135">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="607e3-135">Key of the Resource Operation.</span></span> <span data-ttu-id="607e3-136">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="607e3-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="607e3-137">resource</span><span class="sxs-lookup"><span data-stu-id="607e3-137">resource</span></span>|<span data-ttu-id="607e3-138">String</span><span class="sxs-lookup"><span data-stu-id="607e3-138">String</span></span>|<span data-ttu-id="607e3-139">Категория ресурса, к которой относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="607e3-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="607e3-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="607e3-140">resourceName</span></span>|<span data-ttu-id="607e3-141">String</span><span class="sxs-lookup"><span data-stu-id="607e3-141">String</span></span>|<span data-ttu-id="607e3-142">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="607e3-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="607e3-143">actionName</span><span class="sxs-lookup"><span data-stu-id="607e3-143">actionName</span></span>|<span data-ttu-id="607e3-144">String</span><span class="sxs-lookup"><span data-stu-id="607e3-144">String</span></span>|<span data-ttu-id="607e3-145">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="607e3-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="607e3-146">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="607e3-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="607e3-147">description</span><span class="sxs-lookup"><span data-stu-id="607e3-147">description</span></span>|<span data-ttu-id="607e3-148">String</span><span class="sxs-lookup"><span data-stu-id="607e3-148">String</span></span>|<span data-ttu-id="607e3-149">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="607e3-149">Description of the resource operation.</span></span> <span data-ttu-id="607e3-150">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="607e3-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="607e3-151">енабледфорскопевалидатион</span><span class="sxs-lookup"><span data-stu-id="607e3-151">enabledForScopeValidation</span></span>|<span data-ttu-id="607e3-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="607e3-152">Boolean</span></span>|<span data-ttu-id="607e3-153">Определяет, является ли разрешение проверенным для областей, определенных для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="607e3-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="607e3-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="607e3-154">Response</span></span>
<span data-ttu-id="607e3-155">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="607e3-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="607e3-156">Пример</span><span class="sxs-lookup"><span data-stu-id="607e3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="607e3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="607e3-157">Request</span></span>
<span data-ttu-id="607e3-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="607e3-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="607e3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="607e3-159">Response</span></span>
<span data-ttu-id="607e3-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="607e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



