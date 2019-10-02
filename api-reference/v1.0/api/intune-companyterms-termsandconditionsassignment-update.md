---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97635a00fcf6d527aaa2e8d60a619de9961272c2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354541"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="b9080-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b9080-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="b9080-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9080-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9080-105">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b9080-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9080-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b9080-106">Prerequisites</span></span>
<span data-ttu-id="b9080-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9080-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9080-109">Permission type</span></span>|<span data-ttu-id="b9080-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9080-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9080-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9080-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9080-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9080-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9080-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9080-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9080-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9080-114">Not supported.</span></span>|
|<span data-ttu-id="b9080-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9080-115">Application</span></span>|<span data-ttu-id="b9080-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9080-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9080-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9080-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b9080-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9080-118">Request headers</span></span>
|<span data-ttu-id="b9080-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9080-119">Header</span></span>|<span data-ttu-id="b9080-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b9080-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9080-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9080-121">Authorization</span></span>|<span data-ttu-id="b9080-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9080-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9080-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b9080-123">Accept</span></span>|<span data-ttu-id="b9080-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b9080-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9080-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9080-125">Request body</span></span>
<span data-ttu-id="b9080-126">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9080-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="b9080-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b9080-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="b9080-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9080-128">Property</span></span>|<span data-ttu-id="b9080-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b9080-129">Type</span></span>|<span data-ttu-id="b9080-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b9080-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9080-131">id</span><span class="sxs-lookup"><span data-stu-id="b9080-131">id</span></span>|<span data-ttu-id="b9080-132">String</span><span class="sxs-lookup"><span data-stu-id="b9080-132">String</span></span>|<span data-ttu-id="b9080-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b9080-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b9080-134">target</span><span class="sxs-lookup"><span data-stu-id="b9080-134">target</span></span>|[<span data-ttu-id="b9080-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b9080-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b9080-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="b9080-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="b9080-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9080-137">Response</span></span>
<span data-ttu-id="b9080-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9080-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9080-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b9080-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9080-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9080-140">Request</span></span>
<span data-ttu-id="b9080-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9080-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b9080-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9080-142">Response</span></span>
<span data-ttu-id="b9080-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9080-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




