---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92e1026e18c00978da8a1ac115e5d524adde75e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459788"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="2b53a-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="2b53a-103">Create resourceOperation</span></span>

<span data-ttu-id="2b53a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b53a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b53a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b53a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b53a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b53a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b53a-107">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2b53a-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b53a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b53a-108">Prerequisites</span></span>
<span data-ttu-id="2b53a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b53a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b53a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b53a-111">Permission type</span></span>|<span data-ttu-id="2b53a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b53a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b53a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b53a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b53a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b53a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2b53a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b53a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b53a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b53a-116">Not supported.</span></span>|
|<span data-ttu-id="2b53a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b53a-117">Application</span></span>|<span data-ttu-id="2b53a-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b53a-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b53a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b53a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="2b53a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b53a-120">Request headers</span></span>
|<span data-ttu-id="2b53a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b53a-121">Header</span></span>|<span data-ttu-id="2b53a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b53a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b53a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b53a-123">Authorization</span></span>|<span data-ttu-id="2b53a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b53a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b53a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b53a-125">Accept</span></span>|<span data-ttu-id="2b53a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b53a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b53a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b53a-127">Request body</span></span>
<span data-ttu-id="2b53a-128">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b53a-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="2b53a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="2b53a-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="2b53a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b53a-130">Property</span></span>|<span data-ttu-id="2b53a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b53a-131">Type</span></span>|<span data-ttu-id="2b53a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b53a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b53a-133">id</span><span class="sxs-lookup"><span data-stu-id="2b53a-133">id</span></span>|<span data-ttu-id="2b53a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2b53a-134">String</span></span>|<span data-ttu-id="2b53a-135">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="2b53a-135">Key of the Resource Operation.</span></span> <span data-ttu-id="2b53a-136">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="2b53a-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="2b53a-137">resource</span><span class="sxs-lookup"><span data-stu-id="2b53a-137">resource</span></span>|<span data-ttu-id="2b53a-138">String</span><span class="sxs-lookup"><span data-stu-id="2b53a-138">String</span></span>|<span data-ttu-id="2b53a-139">Категория ресурса, к которой относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="2b53a-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="2b53a-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="2b53a-140">resourceName</span></span>|<span data-ttu-id="2b53a-141">String</span><span class="sxs-lookup"><span data-stu-id="2b53a-141">String</span></span>|<span data-ttu-id="2b53a-142">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="2b53a-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="2b53a-143">actionName</span><span class="sxs-lookup"><span data-stu-id="2b53a-143">actionName</span></span>|<span data-ttu-id="2b53a-144">String</span><span class="sxs-lookup"><span data-stu-id="2b53a-144">String</span></span>|<span data-ttu-id="2b53a-145">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="2b53a-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="2b53a-146">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="2b53a-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="2b53a-147">description</span><span class="sxs-lookup"><span data-stu-id="2b53a-147">description</span></span>|<span data-ttu-id="2b53a-148">String</span><span class="sxs-lookup"><span data-stu-id="2b53a-148">String</span></span>|<span data-ttu-id="2b53a-149">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="2b53a-149">Description of the resource operation.</span></span> <span data-ttu-id="2b53a-150">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2b53a-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="2b53a-151">енабледфорскопевалидатион</span><span class="sxs-lookup"><span data-stu-id="2b53a-151">enabledForScopeValidation</span></span>|<span data-ttu-id="2b53a-152">Логический</span><span class="sxs-lookup"><span data-stu-id="2b53a-152">Boolean</span></span>|<span data-ttu-id="2b53a-153">Определяет, является ли разрешение проверенным для областей, определенных для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="2b53a-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="2b53a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b53a-154">Response</span></span>
<span data-ttu-id="2b53a-155">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b53a-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b53a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="2b53a-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b53a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b53a-157">Request</span></span>
<span data-ttu-id="2b53a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b53a-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b53a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b53a-159">Response</span></span>
<span data-ttu-id="2b53a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b53a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





