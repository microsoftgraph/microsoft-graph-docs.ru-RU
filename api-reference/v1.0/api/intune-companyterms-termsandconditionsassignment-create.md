---
title: Создание объекта termsAndConditionsAssignment
description: Создание объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a52b60ee00f8565c9ea148c14bdfebbde309536b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257437"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="e6360-103">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e6360-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="e6360-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6360-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6360-105">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e6360-105">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6360-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e6360-106">Prerequisites</span></span>
<span data-ttu-id="e6360-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6360-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6360-109">Permission type</span></span>|<span data-ttu-id="e6360-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6360-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6360-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6360-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6360-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6360-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e6360-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6360-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6360-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6360-114">Not supported.</span></span>|
|<span data-ttu-id="e6360-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6360-115">Application</span></span>|<span data-ttu-id="e6360-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6360-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6360-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6360-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e6360-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6360-118">Request headers</span></span>
|<span data-ttu-id="e6360-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6360-119">Header</span></span>|<span data-ttu-id="e6360-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e6360-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6360-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6360-121">Authorization</span></span>|<span data-ttu-id="e6360-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6360-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6360-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e6360-123">Accept</span></span>|<span data-ttu-id="e6360-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6360-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6360-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6360-125">Request body</span></span>
<span data-ttu-id="e6360-126">В тексте запроса добавьте представление объекта termsAndConditionsAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6360-126">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="e6360-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="e6360-127">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="e6360-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6360-128">Property</span></span>|<span data-ttu-id="e6360-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e6360-129">Type</span></span>|<span data-ttu-id="e6360-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e6360-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6360-131">id</span><span class="sxs-lookup"><span data-stu-id="e6360-131">id</span></span>|<span data-ttu-id="e6360-132">String</span><span class="sxs-lookup"><span data-stu-id="e6360-132">String</span></span>|<span data-ttu-id="e6360-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e6360-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e6360-134">target</span><span class="sxs-lookup"><span data-stu-id="e6360-134">target</span></span>|[<span data-ttu-id="e6360-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e6360-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e6360-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="e6360-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="e6360-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6360-137">Response</span></span>
<span data-ttu-id="e6360-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6360-138">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6360-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e6360-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6360-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6360-140">Request</span></span>
<span data-ttu-id="e6360-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6360-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e6360-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6360-142">Response</span></span>
<span data-ttu-id="e6360-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6360-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



