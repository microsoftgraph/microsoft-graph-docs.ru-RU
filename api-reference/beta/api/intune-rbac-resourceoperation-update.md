---
title: Обновление объекта resourceOperation
description: Обновляет свойства объекта resourceOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f8856bd02bc7ed92906225bc8d7608718f65d4d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940571"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="62567-103">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="62567-103">Update resourceOperation</span></span>

> <span data-ttu-id="62567-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62567-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62567-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62567-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62567-106">Обновляет свойства объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="62567-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62567-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="62567-107">Prerequisites</span></span>
<span data-ttu-id="62567-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62567-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62567-110">Permission type</span></span>|<span data-ttu-id="62567-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62567-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62567-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62567-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62567-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62567-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="62567-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62567-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62567-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62567-115">Not supported.</span></span>|
|<span data-ttu-id="62567-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62567-116">Application</span></span>|<span data-ttu-id="62567-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62567-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62567-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62567-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="62567-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="62567-119">Request headers</span></span>
|<span data-ttu-id="62567-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62567-120">Header</span></span>|<span data-ttu-id="62567-121">Значение</span><span class="sxs-lookup"><span data-stu-id="62567-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62567-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62567-122">Authorization</span></span>|<span data-ttu-id="62567-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62567-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62567-124">Accept</span><span class="sxs-lookup"><span data-stu-id="62567-124">Accept</span></span>|<span data-ttu-id="62567-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62567-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62567-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62567-126">Request body</span></span>
<span data-ttu-id="62567-127">В теле запроса добавьте представление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62567-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="62567-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="62567-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="62567-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="62567-129">Property</span></span>|<span data-ttu-id="62567-130">Тип</span><span class="sxs-lookup"><span data-stu-id="62567-130">Type</span></span>|<span data-ttu-id="62567-131">Описание</span><span class="sxs-lookup"><span data-stu-id="62567-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62567-132">id</span><span class="sxs-lookup"><span data-stu-id="62567-132">id</span></span>|<span data-ttu-id="62567-133">Строка</span><span class="sxs-lookup"><span data-stu-id="62567-133">String</span></span>|<span data-ttu-id="62567-134">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="62567-134">Key of the Resource Operation.</span></span> <span data-ttu-id="62567-135">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="62567-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="62567-136">resource</span><span class="sxs-lookup"><span data-stu-id="62567-136">resource</span></span>|<span data-ttu-id="62567-137">Строка</span><span class="sxs-lookup"><span data-stu-id="62567-137">String</span></span>|<span data-ttu-id="62567-138">Категория ресурса, к которой относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="62567-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="62567-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="62567-139">resourceName</span></span>|<span data-ttu-id="62567-140">String</span><span class="sxs-lookup"><span data-stu-id="62567-140">String</span></span>|<span data-ttu-id="62567-141">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="62567-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="62567-142">actionName</span><span class="sxs-lookup"><span data-stu-id="62567-142">actionName</span></span>|<span data-ttu-id="62567-143">String</span><span class="sxs-lookup"><span data-stu-id="62567-143">String</span></span>|<span data-ttu-id="62567-144">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="62567-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="62567-145">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="62567-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="62567-146">description</span><span class="sxs-lookup"><span data-stu-id="62567-146">description</span></span>|<span data-ttu-id="62567-147">String</span><span class="sxs-lookup"><span data-stu-id="62567-147">String</span></span>|<span data-ttu-id="62567-148">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="62567-148">Description of the resource operation.</span></span> <span data-ttu-id="62567-149">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="62567-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="62567-150">енабледфорскопевалидатион</span><span class="sxs-lookup"><span data-stu-id="62567-150">enabledForScopeValidation</span></span>|<span data-ttu-id="62567-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="62567-151">Boolean</span></span>|<span data-ttu-id="62567-152">Определяет, является ли разрешение проверенным для областей, определенных для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="62567-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="62567-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="62567-153">Response</span></span>
<span data-ttu-id="62567-154">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="62567-154">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62567-155">Пример</span><span class="sxs-lookup"><span data-stu-id="62567-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="62567-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="62567-156">Request</span></span>
<span data-ttu-id="62567-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62567-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62567-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="62567-158">Response</span></span>
<span data-ttu-id="62567-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62567-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





