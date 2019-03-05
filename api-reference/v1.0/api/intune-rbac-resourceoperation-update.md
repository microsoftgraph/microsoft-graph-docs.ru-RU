---
title: Обновление объекта resourceOperation
description: Обновляет свойства объекта resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23e822502a8ba64466fd3630eda2acb19bf044f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251113"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="e8262-103">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="e8262-103">Update resourceOperation</span></span>

> <span data-ttu-id="e8262-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8262-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8262-105">Обновляет свойства объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e8262-105">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8262-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8262-106">Prerequisites</span></span>
<span data-ttu-id="e8262-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e8262-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8262-109">Permission type</span></span>|<span data-ttu-id="e8262-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8262-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8262-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8262-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8262-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8262-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e8262-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8262-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8262-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8262-114">Not supported.</span></span>|
|<span data-ttu-id="e8262-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8262-115">Application</span></span>|<span data-ttu-id="e8262-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8262-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8262-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8262-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="e8262-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8262-118">Request headers</span></span>
|<span data-ttu-id="e8262-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8262-119">Header</span></span>|<span data-ttu-id="e8262-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e8262-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8262-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8262-121">Authorization</span></span>|<span data-ttu-id="e8262-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e8262-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8262-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e8262-123">Accept</span></span>|<span data-ttu-id="e8262-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e8262-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8262-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8262-125">Request body</span></span>
<span data-ttu-id="e8262-126">В теле запроса добавьте представление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8262-126">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="e8262-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e8262-127">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="e8262-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8262-128">Property</span></span>|<span data-ttu-id="e8262-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e8262-129">Type</span></span>|<span data-ttu-id="e8262-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e8262-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8262-131">id</span><span class="sxs-lookup"><span data-stu-id="e8262-131">id</span></span>|<span data-ttu-id="e8262-132">String</span><span class="sxs-lookup"><span data-stu-id="e8262-132">String</span></span>|<span data-ttu-id="e8262-133">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="e8262-133">Key of the Resource Operation.</span></span> <span data-ttu-id="e8262-134">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="e8262-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="e8262-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="e8262-135">resourceName</span></span>|<span data-ttu-id="e8262-136">String</span><span class="sxs-lookup"><span data-stu-id="e8262-136">String</span></span>|<span data-ttu-id="e8262-137">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="e8262-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="e8262-138">actionName</span><span class="sxs-lookup"><span data-stu-id="e8262-138">actionName</span></span>|<span data-ttu-id="e8262-139">String</span><span class="sxs-lookup"><span data-stu-id="e8262-139">String</span></span>|<span data-ttu-id="e8262-140">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="e8262-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="e8262-141">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="e8262-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="e8262-142">description</span><span class="sxs-lookup"><span data-stu-id="e8262-142">description</span></span>|<span data-ttu-id="e8262-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e8262-143">String</span></span>|<span data-ttu-id="e8262-144">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="e8262-144">Description of the resource operation.</span></span> <span data-ttu-id="e8262-145">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e8262-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="e8262-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8262-146">Response</span></span>
<span data-ttu-id="e8262-147">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8262-147">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8262-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e8262-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8262-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8262-149">Request</span></span>
<span data-ttu-id="e8262-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8262-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8262-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8262-151">Response</span></span>
<span data-ttu-id="e8262-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8262-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



