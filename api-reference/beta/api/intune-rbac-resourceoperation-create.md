---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8aa701d51d51d326340ff5ebddc9cc97c5962402
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938666"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="d4201-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="d4201-103">Create resourceOperation</span></span>

> <span data-ttu-id="d4201-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d4201-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4201-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4201-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4201-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d4201-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4201-107">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d4201-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4201-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d4201-108">Prerequisites</span></span>
<span data-ttu-id="d4201-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4201-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4201-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4201-111">Permission type</span></span>|<span data-ttu-id="d4201-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4201-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4201-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4201-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4201-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4201-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d4201-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4201-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4201-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4201-116">Not supported.</span></span>|
|<span data-ttu-id="d4201-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4201-117">Application</span></span>|<span data-ttu-id="d4201-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4201-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4201-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4201-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="d4201-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4201-120">Request headers</span></span>
|<span data-ttu-id="d4201-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4201-121">Header</span></span>|<span data-ttu-id="d4201-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4201-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4201-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4201-123">Authorization</span></span>|<span data-ttu-id="d4201-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d4201-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4201-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4201-125">Accept</span></span>|<span data-ttu-id="d4201-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4201-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4201-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4201-127">Request body</span></span>
<span data-ttu-id="d4201-128">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4201-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="d4201-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="d4201-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="d4201-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4201-130">Property</span></span>|<span data-ttu-id="d4201-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4201-131">Type</span></span>|<span data-ttu-id="d4201-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4201-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4201-133">id</span><span class="sxs-lookup"><span data-stu-id="d4201-133">id</span></span>|<span data-ttu-id="d4201-134">String</span><span class="sxs-lookup"><span data-stu-id="d4201-134">String</span></span>|<span data-ttu-id="d4201-135">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="d4201-135">Key of the Resource Operation.</span></span> <span data-ttu-id="d4201-136">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="d4201-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="d4201-137">resource</span><span class="sxs-lookup"><span data-stu-id="d4201-137">resource</span></span>|<span data-ttu-id="d4201-138">String</span><span class="sxs-lookup"><span data-stu-id="d4201-138">String</span></span>|<span data-ttu-id="d4201-139">Категория ресурсов, к которому относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="d4201-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="d4201-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="d4201-140">resourceName</span></span>|<span data-ttu-id="d4201-141">String</span><span class="sxs-lookup"><span data-stu-id="d4201-141">String</span></span>|<span data-ttu-id="d4201-142">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="d4201-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="d4201-143">actionName</span><span class="sxs-lookup"><span data-stu-id="d4201-143">actionName</span></span>|<span data-ttu-id="d4201-144">String</span><span class="sxs-lookup"><span data-stu-id="d4201-144">String</span></span>|<span data-ttu-id="d4201-145">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="d4201-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="d4201-146">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="d4201-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="d4201-147">описание</span><span class="sxs-lookup"><span data-stu-id="d4201-147">description</span></span>|<span data-ttu-id="d4201-148">String</span><span class="sxs-lookup"><span data-stu-id="d4201-148">String</span></span>|<span data-ttu-id="d4201-149">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="d4201-149">Description of the resource operation.</span></span> <span data-ttu-id="d4201-150">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d4201-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="d4201-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="d4201-151">enabledForScopeValidation</span></span>|<span data-ttu-id="d4201-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4201-152">Boolean</span></span>|<span data-ttu-id="d4201-153">Определяет проверить разрешения для областей, определенных для каждого назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d4201-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="d4201-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4201-154">Response</span></span>
<span data-ttu-id="d4201-155">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4201-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4201-156">Пример</span><span class="sxs-lookup"><span data-stu-id="d4201-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4201-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4201-157">Request</span></span>
<span data-ttu-id="d4201-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4201-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4201-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4201-159">Response</span></span>
<span data-ttu-id="d4201-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d4201-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





