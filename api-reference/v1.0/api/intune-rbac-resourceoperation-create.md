---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
ms.openlocfilehash: 40f8c7175c5f6ad5e2885fe7e893bba118458be1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026318"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="3f25d-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="3f25d-103">Create resourceOperation</span></span>

> <span data-ttu-id="3f25d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3f25d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f25d-105">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3f25d-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f25d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3f25d-106">Prerequisites</span></span>
<span data-ttu-id="3f25d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f25d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f25d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f25d-109">Permission type</span></span>|<span data-ttu-id="3f25d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f25d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f25d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f25d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f25d-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f25d-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3f25d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f25d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f25d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f25d-114">Not supported.</span></span>|
|<span data-ttu-id="3f25d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f25d-115">Application</span></span>|<span data-ttu-id="3f25d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f25d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f25d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f25d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="3f25d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f25d-118">Request headers</span></span>
|<span data-ttu-id="3f25d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f25d-119">Header</span></span>|<span data-ttu-id="3f25d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3f25d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f25d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f25d-121">Authorization</span></span>|<span data-ttu-id="3f25d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3f25d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f25d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3f25d-123">Accept</span></span>|<span data-ttu-id="3f25d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3f25d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f25d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f25d-125">Request body</span></span>
<span data-ttu-id="3f25d-126">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f25d-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="3f25d-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="3f25d-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="3f25d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f25d-128">Property</span></span>|<span data-ttu-id="3f25d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3f25d-129">Type</span></span>|<span data-ttu-id="3f25d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3f25d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f25d-131">id</span><span class="sxs-lookup"><span data-stu-id="3f25d-131">id</span></span>|<span data-ttu-id="3f25d-132">String</span><span class="sxs-lookup"><span data-stu-id="3f25d-132">String</span></span>|<span data-ttu-id="3f25d-133">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="3f25d-133">Key of the Resource Operation.</span></span> <span data-ttu-id="3f25d-134">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="3f25d-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="3f25d-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="3f25d-135">resourceName</span></span>|<span data-ttu-id="3f25d-136">String</span><span class="sxs-lookup"><span data-stu-id="3f25d-136">String</span></span>|<span data-ttu-id="3f25d-137">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="3f25d-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="3f25d-138">actionName</span><span class="sxs-lookup"><span data-stu-id="3f25d-138">actionName</span></span>|<span data-ttu-id="3f25d-139">String</span><span class="sxs-lookup"><span data-stu-id="3f25d-139">String</span></span>|<span data-ttu-id="3f25d-140">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="3f25d-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="3f25d-141">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="3f25d-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="3f25d-142">описание</span><span class="sxs-lookup"><span data-stu-id="3f25d-142">description</span></span>|<span data-ttu-id="3f25d-143">String</span><span class="sxs-lookup"><span data-stu-id="3f25d-143">String</span></span>|<span data-ttu-id="3f25d-144">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="3f25d-144">Description of the resource operation.</span></span> <span data-ttu-id="3f25d-145">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3f25d-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="3f25d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f25d-146">Response</span></span>
<span data-ttu-id="3f25d-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3f25d-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f25d-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3f25d-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f25d-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f25d-149">Request</span></span>
<span data-ttu-id="3f25d-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f25d-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f25d-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f25d-151">Response</span></span>
<span data-ttu-id="3f25d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3f25d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



