---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86bcd9af52a25e47b3a1fb07ec86f4ff7da0f8ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884709"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="be80a-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="be80a-103">Create resourceOperation</span></span>

> <span data-ttu-id="be80a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be80a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be80a-105">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="be80a-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be80a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="be80a-106">Prerequisites</span></span>
<span data-ttu-id="be80a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be80a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be80a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be80a-109">Permission type</span></span>|<span data-ttu-id="be80a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be80a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be80a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be80a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be80a-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be80a-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="be80a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be80a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be80a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be80a-114">Not supported.</span></span>|
|<span data-ttu-id="be80a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be80a-115">Application</span></span>|<span data-ttu-id="be80a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be80a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be80a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be80a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="be80a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be80a-118">Request headers</span></span>
|<span data-ttu-id="be80a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be80a-119">Header</span></span>|<span data-ttu-id="be80a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="be80a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be80a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be80a-121">Authorization</span></span>|<span data-ttu-id="be80a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be80a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be80a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="be80a-123">Accept</span></span>|<span data-ttu-id="be80a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be80a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be80a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be80a-125">Request body</span></span>
<span data-ttu-id="be80a-126">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be80a-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="be80a-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="be80a-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="be80a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="be80a-128">Property</span></span>|<span data-ttu-id="be80a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="be80a-129">Type</span></span>|<span data-ttu-id="be80a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="be80a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be80a-131">id</span><span class="sxs-lookup"><span data-stu-id="be80a-131">id</span></span>|<span data-ttu-id="be80a-132">String</span><span class="sxs-lookup"><span data-stu-id="be80a-132">String</span></span>|<span data-ttu-id="be80a-133">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="be80a-133">Key of the Resource Operation.</span></span> <span data-ttu-id="be80a-134">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="be80a-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="be80a-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="be80a-135">resourceName</span></span>|<span data-ttu-id="be80a-136">String</span><span class="sxs-lookup"><span data-stu-id="be80a-136">String</span></span>|<span data-ttu-id="be80a-137">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="be80a-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="be80a-138">actionName</span><span class="sxs-lookup"><span data-stu-id="be80a-138">actionName</span></span>|<span data-ttu-id="be80a-139">String</span><span class="sxs-lookup"><span data-stu-id="be80a-139">String</span></span>|<span data-ttu-id="be80a-140">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="be80a-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="be80a-141">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="be80a-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="be80a-142">описание</span><span class="sxs-lookup"><span data-stu-id="be80a-142">description</span></span>|<span data-ttu-id="be80a-143">String</span><span class="sxs-lookup"><span data-stu-id="be80a-143">String</span></span>|<span data-ttu-id="be80a-144">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="be80a-144">Description of the resource operation.</span></span> <span data-ttu-id="be80a-145">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="be80a-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="be80a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="be80a-146">Response</span></span>
<span data-ttu-id="be80a-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be80a-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be80a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="be80a-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="be80a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="be80a-149">Request</span></span>
<span data-ttu-id="be80a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be80a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be80a-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="be80a-151">Response</span></span>
<span data-ttu-id="be80a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be80a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



