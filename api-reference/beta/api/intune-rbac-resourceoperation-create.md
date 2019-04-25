---
title: Создание объекта resourceOperation
description: Создание объекта resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd973fa12b4737322cd53d681bfea085731ffc60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527562"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="08ced-103">Создание объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="08ced-103">Create resourceOperation</span></span>

> <span data-ttu-id="08ced-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ced-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08ced-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08ced-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08ced-106">Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="08ced-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08ced-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08ced-107">Prerequisites</span></span>
<span data-ttu-id="08ced-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ced-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08ced-110">Permission type</span></span>|<span data-ttu-id="08ced-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08ced-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08ced-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08ced-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08ced-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08ced-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="08ced-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08ced-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08ced-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ced-115">Not supported.</span></span>|
|<span data-ttu-id="08ced-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08ced-116">Application</span></span>|<span data-ttu-id="08ced-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ced-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08ced-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08ced-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="08ced-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08ced-119">Request headers</span></span>
|<span data-ttu-id="08ced-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08ced-120">Header</span></span>|<span data-ttu-id="08ced-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08ced-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08ced-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08ced-122">Authorization</span></span>|<span data-ttu-id="08ced-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08ced-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08ced-124">Accept</span><span class="sxs-lookup"><span data-stu-id="08ced-124">Accept</span></span>|<span data-ttu-id="08ced-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08ced-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ced-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08ced-126">Request body</span></span>
<span data-ttu-id="08ced-127">В теле запроса добавьте представление объекта resourceOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08ced-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="08ced-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="08ced-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="08ced-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08ced-129">Property</span></span>|<span data-ttu-id="08ced-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08ced-130">Type</span></span>|<span data-ttu-id="08ced-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08ced-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ced-132">id</span><span class="sxs-lookup"><span data-stu-id="08ced-132">id</span></span>|<span data-ttu-id="08ced-133">Строка</span><span class="sxs-lookup"><span data-stu-id="08ced-133">String</span></span>|<span data-ttu-id="08ced-134">Ключ операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="08ced-134">Key of the Resource Operation.</span></span> <span data-ttu-id="08ced-135">Доступен только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="08ced-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="08ced-136">resource</span><span class="sxs-lookup"><span data-stu-id="08ced-136">resource</span></span>|<span data-ttu-id="08ced-137">String</span><span class="sxs-lookup"><span data-stu-id="08ced-137">String</span></span>|<span data-ttu-id="08ced-138">Категория ресурса, к которой относится данная операция.</span><span class="sxs-lookup"><span data-stu-id="08ced-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="08ced-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="08ced-139">resourceName</span></span>|<span data-ttu-id="08ced-140">String</span><span class="sxs-lookup"><span data-stu-id="08ced-140">String</span></span>|<span data-ttu-id="08ced-141">Имя ресурса, с которым выполняется эта операция.</span><span class="sxs-lookup"><span data-stu-id="08ced-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="08ced-142">actionName</span><span class="sxs-lookup"><span data-stu-id="08ced-142">actionName</span></span>|<span data-ttu-id="08ced-143">String</span><span class="sxs-lookup"><span data-stu-id="08ced-143">String</span></span>|<span data-ttu-id="08ced-144">Тип действия, которое выполнит эта операция.</span><span class="sxs-lookup"><span data-stu-id="08ced-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="08ced-145">Свойство actionName должно быть максимально краткое (максимум несколько слов).</span><span class="sxs-lookup"><span data-stu-id="08ced-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="08ced-146">description</span><span class="sxs-lookup"><span data-stu-id="08ced-146">description</span></span>|<span data-ttu-id="08ced-147">String</span><span class="sxs-lookup"><span data-stu-id="08ced-147">String</span></span>|<span data-ttu-id="08ced-148">Описание операции с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="08ced-148">Description of the resource operation.</span></span> <span data-ttu-id="08ced-149">Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="08ced-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="08ced-150">Енабледфорскопевалидатион</span><span class="sxs-lookup"><span data-stu-id="08ced-150">enabledForScopeValidation</span></span>|<span data-ttu-id="08ced-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="08ced-151">Boolean</span></span>|<span data-ttu-id="08ced-152">Определяет, является ли разрешение проверенным для областей, определенных для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="08ced-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="08ced-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="08ced-153">Response</span></span>
<span data-ttu-id="08ced-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08ced-154">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08ced-155">Пример</span><span class="sxs-lookup"><span data-stu-id="08ced-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="08ced-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="08ced-156">Request</span></span>
<span data-ttu-id="08ced-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08ced-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08ced-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="08ced-158">Response</span></span>
<span data-ttu-id="08ced-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08ced-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





