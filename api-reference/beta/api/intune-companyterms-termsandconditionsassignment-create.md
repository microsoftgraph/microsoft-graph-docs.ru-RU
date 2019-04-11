---
title: Создание объекта termsAndConditionsAssignment
description: Создание объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af88847ac2ce47b09f5a07304f02a1d1fcce2598
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786506"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="a3c59-103">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a3c59-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="a3c59-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3c59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3c59-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3c59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3c59-106">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a3c59-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3c59-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3c59-107">Prerequisites</span></span>
<span data-ttu-id="a3c59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3c59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3c59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3c59-110">Permission type</span></span>|<span data-ttu-id="a3c59-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3c59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3c59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3c59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3c59-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c59-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a3c59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3c59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3c59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3c59-115">Not supported.</span></span>|
|<span data-ttu-id="a3c59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3c59-116">Application</span></span>|<span data-ttu-id="a3c59-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3c59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3c59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3c59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a3c59-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3c59-119">Request headers</span></span>
|<span data-ttu-id="a3c59-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3c59-120">Header</span></span>|<span data-ttu-id="a3c59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3c59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3c59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3c59-122">Authorization</span></span>|<span data-ttu-id="a3c59-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3c59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3c59-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3c59-124">Accept</span></span>|<span data-ttu-id="a3c59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3c59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3c59-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3c59-126">Request body</span></span>
<span data-ttu-id="a3c59-127">В тексте запроса добавьте представление объекта termsAndConditionsAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3c59-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="a3c59-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="a3c59-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="a3c59-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3c59-129">Property</span></span>|<span data-ttu-id="a3c59-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a3c59-130">Type</span></span>|<span data-ttu-id="a3c59-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a3c59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3c59-132">id</span><span class="sxs-lookup"><span data-stu-id="a3c59-132">id</span></span>|<span data-ttu-id="a3c59-133">String</span><span class="sxs-lookup"><span data-stu-id="a3c59-133">String</span></span>|<span data-ttu-id="a3c59-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="a3c59-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="a3c59-135">target</span><span class="sxs-lookup"><span data-stu-id="a3c59-135">target</span></span>|[<span data-ttu-id="a3c59-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a3c59-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a3c59-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="a3c59-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="a3c59-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3c59-138">Response</span></span>
<span data-ttu-id="a3c59-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3c59-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3c59-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a3c59-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3c59-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3c59-141">Request</span></span>
<span data-ttu-id="a3c59-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3c59-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a3c59-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3c59-143">Response</span></span>
<span data-ttu-id="a3c59-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3c59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





