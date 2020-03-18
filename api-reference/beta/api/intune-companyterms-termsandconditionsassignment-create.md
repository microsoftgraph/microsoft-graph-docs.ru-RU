---
title: Создание объекта termsAndConditionsAssignment
description: Создание объекта termsAndConditionsAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 329bd5b227600dff42c96d54a6a0497f8b978af3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760111"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="75a96-103">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75a96-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="75a96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a96-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75a96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a96-106">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75a96-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75a96-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75a96-107">Prerequisites</span></span>
<span data-ttu-id="75a96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a96-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a96-110">Permission type</span></span>|<span data-ttu-id="75a96-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75a96-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75a96-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a96-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="75a96-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75a96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a96-115">Not supported.</span></span>|
|<span data-ttu-id="75a96-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="75a96-116">Application</span></span>|<span data-ttu-id="75a96-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a96-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75a96-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="75a96-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75a96-119">Request headers</span></span>
|<span data-ttu-id="75a96-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75a96-120">Header</span></span>|<span data-ttu-id="75a96-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75a96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75a96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75a96-122">Authorization</span></span>|<span data-ttu-id="75a96-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75a96-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75a96-124">Accept</span></span>|<span data-ttu-id="75a96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75a96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75a96-126">Request body</span></span>
<span data-ttu-id="75a96-127">В тексте запроса добавьте представление объекта termsAndConditionsAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75a96-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="75a96-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="75a96-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="75a96-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75a96-129">Property</span></span>|<span data-ttu-id="75a96-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75a96-130">Type</span></span>|<span data-ttu-id="75a96-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75a96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a96-132">id</span><span class="sxs-lookup"><span data-stu-id="75a96-132">id</span></span>|<span data-ttu-id="75a96-133">String</span><span class="sxs-lookup"><span data-stu-id="75a96-133">String</span></span>|<span data-ttu-id="75a96-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="75a96-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="75a96-135">target</span><span class="sxs-lookup"><span data-stu-id="75a96-135">target</span></span>|[<span data-ttu-id="75a96-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="75a96-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="75a96-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="75a96-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="75a96-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a96-138">Response</span></span>
<span data-ttu-id="75a96-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75a96-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a96-140">Пример</span><span class="sxs-lookup"><span data-stu-id="75a96-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="75a96-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a96-141">Request</span></span>
<span data-ttu-id="75a96-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75a96-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75a96-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a96-143">Response</span></span>
<span data-ttu-id="75a96-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75a96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




