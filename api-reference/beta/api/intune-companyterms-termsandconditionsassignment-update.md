---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17051c4b665f171d6ce2d2c3fbe4c09acbe3fc45
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964978"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="7f32f-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f32f-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="7f32f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f32f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f32f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f32f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f32f-106">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f32f-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f32f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f32f-107">Prerequisites</span></span>
<span data-ttu-id="7f32f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f32f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f32f-110">Permission type</span></span>|<span data-ttu-id="7f32f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f32f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f32f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f32f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f32f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f32f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f32f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f32f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f32f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f32f-115">Not supported.</span></span>|
|<span data-ttu-id="7f32f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f32f-116">Application</span></span>|<span data-ttu-id="7f32f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f32f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f32f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f32f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7f32f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f32f-119">Request headers</span></span>
|<span data-ttu-id="7f32f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f32f-120">Header</span></span>|<span data-ttu-id="7f32f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7f32f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f32f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f32f-122">Authorization</span></span>|<span data-ttu-id="7f32f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f32f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f32f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7f32f-124">Accept</span></span>|<span data-ttu-id="7f32f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f32f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f32f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f32f-126">Request body</span></span>
<span data-ttu-id="7f32f-127">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f32f-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="7f32f-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f32f-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="7f32f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f32f-129">Property</span></span>|<span data-ttu-id="7f32f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f32f-130">Type</span></span>|<span data-ttu-id="7f32f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f32f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f32f-132">id</span><span class="sxs-lookup"><span data-stu-id="7f32f-132">id</span></span>|<span data-ttu-id="7f32f-133">String</span><span class="sxs-lookup"><span data-stu-id="7f32f-133">String</span></span>|<span data-ttu-id="7f32f-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7f32f-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7f32f-135">target</span><span class="sxs-lookup"><span data-stu-id="7f32f-135">target</span></span>|[<span data-ttu-id="7f32f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f32f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7f32f-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="7f32f-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7f32f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f32f-138">Response</span></span>
<span data-ttu-id="7f32f-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f32f-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f32f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7f32f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f32f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f32f-141">Request</span></span>
<span data-ttu-id="7f32f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f32f-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7f32f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f32f-143">Response</span></span>
<span data-ttu-id="7f32f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f32f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




