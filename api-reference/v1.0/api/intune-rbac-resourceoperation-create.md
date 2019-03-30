---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dafd0dff52fdbded8f6ff0fc8d6743a84dee797
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988338"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="ef945-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ef945-103">Create resourceOperation</span></span>

> <span data-ttu-id="ef945-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef945-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef945-105">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ef945-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef945-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef945-106">Prerequisites</span></span>
<span data-ttu-id="ef945-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef945-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef945-109">Permission type</span></span>|<span data-ttu-id="ef945-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef945-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef945-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef945-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef945-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef945-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ef945-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef945-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef945-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef945-114">Not supported.</span></span>|
|<span data-ttu-id="ef945-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef945-115">Application</span></span>|<span data-ttu-id="ef945-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef945-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef945-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef945-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="ef945-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef945-118">Request headers</span></span>
|<span data-ttu-id="ef945-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef945-119">Header</span></span>|<span data-ttu-id="ef945-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ef945-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef945-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef945-121">Authorization</span></span>|<span data-ttu-id="ef945-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef945-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef945-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ef945-123">Accept</span></span>|<span data-ttu-id="ef945-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ef945-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef945-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef945-125">Request body</span></span>
<span data-ttu-id="ef945-126">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef945-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="ef945-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="ef945-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="ef945-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef945-128">Property</span></span>|<span data-ttu-id="ef945-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ef945-129">Type</span></span>|<span data-ttu-id="ef945-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ef945-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef945-131">id</span><span class="sxs-lookup"><span data-stu-id="ef945-131">id</span></span>|<span data-ttu-id="ef945-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ef945-132">String</span></span>|<span data-ttu-id="ef945-133">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="ef945-133">Key of the Resource Operation.</span></span> <span data-ttu-id="ef945-134">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ef945-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ef945-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="ef945-135">resourceName</span></span>|<span data-ttu-id="ef945-136">String</span><span class="sxs-lookup"><span data-stu-id="ef945-136">String</span></span>|<span data-ttu-id="ef945-137">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="ef945-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ef945-138">actionName</span><span class="sxs-lookup"><span data-stu-id="ef945-138">actionName</span></span>|<span data-ttu-id="ef945-139">String</span><span class="sxs-lookup"><span data-stu-id="ef945-139">String</span></span>|<span data-ttu-id="ef945-140">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="ef945-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ef945-141">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="ef945-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ef945-142">description</span><span class="sxs-lookup"><span data-stu-id="ef945-142">description</span></span>|<span data-ttu-id="ef945-143">String</span><span class="sxs-lookup"><span data-stu-id="ef945-143">String</span></span>|<span data-ttu-id="ef945-144">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="ef945-144">Description of the resource operation.</span></span> <span data-ttu-id="ef945-145">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ef945-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="ef945-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef945-146">Response</span></span>
<span data-ttu-id="ef945-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef945-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef945-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ef945-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef945-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef945-149">Request</span></span>
<span data-ttu-id="ef945-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef945-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef945-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef945-151">Response</span></span>
<span data-ttu-id="ef945-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef945-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



