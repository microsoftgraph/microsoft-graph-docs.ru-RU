---
title: Обновление объекта resourceOperation
description: Обновляет свойства объекта resourceOperation.
author: tfitzmac
ms.openlocfilehash: 8050b91aee679f9dd29e78cbbad62f9f6352343e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317824"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="17b4b-103">Обновление объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="17b4b-103">Update resourceOperation</span></span>

> <span data-ttu-id="17b4b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17b4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17b4b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17b4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17b4b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17b4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17b4b-107">Обновляет свойства объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="17b4b-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17b4b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17b4b-108">Prerequisites</span></span>
<span data-ttu-id="17b4b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b4b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17b4b-111">Permission type</span></span>|<span data-ttu-id="17b4b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17b4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17b4b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17b4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17b4b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b4b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="17b4b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17b4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17b4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17b4b-116">Not supported.</span></span>|
|<span data-ttu-id="17b4b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17b4b-117">Application</span></span>|<span data-ttu-id="17b4b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17b4b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17b4b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17b4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="17b4b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17b4b-120">Request headers</span></span>
|<span data-ttu-id="17b4b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17b4b-121">Header</span></span>|<span data-ttu-id="17b4b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17b4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17b4b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17b4b-123">Authorization</span></span>|<span data-ttu-id="17b4b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="17b4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17b4b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17b4b-125">Accept</span></span>|<span data-ttu-id="17b4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17b4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b4b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17b4b-127">Request body</span></span>
<span data-ttu-id="17b4b-128">В теле запроса добавьте представление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17b4b-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="17b4b-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="17b4b-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="17b4b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17b4b-130">Property</span></span>|<span data-ttu-id="17b4b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17b4b-131">Type</span></span>|<span data-ttu-id="17b4b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17b4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17b4b-133">id</span><span class="sxs-lookup"><span data-stu-id="17b4b-133">id</span></span>|<span data-ttu-id="17b4b-134">String</span><span class="sxs-lookup"><span data-stu-id="17b4b-134">String</span></span>|<span data-ttu-id="17b4b-135">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="17b4b-135">Key of the Resource Operation.</span></span> <span data-ttu-id="17b4b-136">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="17b4b-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="17b4b-137">resource</span><span class="sxs-lookup"><span data-stu-id="17b4b-137">resource</span></span>|<span data-ttu-id="17b4b-138">String.</span><span class="sxs-lookup"><span data-stu-id="17b4b-138">String</span></span>|<span data-ttu-id="17b4b-139">Категория ресурсов, к которому относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="17b4b-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="17b4b-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="17b4b-140">resourceName</span></span>|<span data-ttu-id="17b4b-141">String</span><span class="sxs-lookup"><span data-stu-id="17b4b-141">String</span></span>|<span data-ttu-id="17b4b-142">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="17b4b-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="17b4b-143">actionName</span><span class="sxs-lookup"><span data-stu-id="17b4b-143">actionName</span></span>|<span data-ttu-id="17b4b-144">String</span><span class="sxs-lookup"><span data-stu-id="17b4b-144">String</span></span>|<span data-ttu-id="17b4b-145">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="17b4b-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="17b4b-146">Свойство actionName должно быть максимально кратким (только несколько слов).</span><span class="sxs-lookup"><span data-stu-id="17b4b-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="17b4b-147">описание</span><span class="sxs-lookup"><span data-stu-id="17b4b-147">description</span></span>|<span data-ttu-id="17b4b-148">String</span><span class="sxs-lookup"><span data-stu-id="17b4b-148">String</span></span>|<span data-ttu-id="17b4b-149">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="17b4b-149">Description of the resource operation.</span></span> <span data-ttu-id="17b4b-150">Используется в тексте, который отображается над обозначением операции при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="17b4b-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="17b4b-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="17b4b-151">enabledForScopeValidation</span></span>|<span data-ttu-id="17b4b-152">Boolean.</span><span class="sxs-lookup"><span data-stu-id="17b4b-152">Boolean</span></span>|<span data-ttu-id="17b4b-153">Определяет проверить разрешения для областей, определенных для каждого назначения роли.</span><span class="sxs-lookup"><span data-stu-id="17b4b-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="17b4b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="17b4b-154">Response</span></span>
<span data-ttu-id="17b4b-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="17b4b-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17b4b-156">Пример</span><span class="sxs-lookup"><span data-stu-id="17b4b-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="17b4b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="17b4b-157">Request</span></span>
<span data-ttu-id="17b4b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17b4b-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 193

{
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="17b4b-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="17b4b-159">Response</span></span>
<span data-ttu-id="17b4b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="17b4b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





