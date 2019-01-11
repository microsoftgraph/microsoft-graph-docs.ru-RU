---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 79b8595015496605711d2304d22381171ef3ef34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851459"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="2f630-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2f630-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="2f630-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f630-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f630-105">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f630-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f630-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f630-106">Prerequisites</span></span>
<span data-ttu-id="2f630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f630-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f630-109">Permission type</span></span>|<span data-ttu-id="2f630-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f630-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f630-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f630-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f630-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f630-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f630-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f630-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f630-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f630-114">Not supported.</span></span>|
|<span data-ttu-id="2f630-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f630-115">Application</span></span>|<span data-ttu-id="2f630-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f630-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f630-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f630-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2f630-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f630-118">Request headers</span></span>
|<span data-ttu-id="2f630-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f630-119">Header</span></span>|<span data-ttu-id="2f630-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2f630-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f630-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f630-121">Authorization</span></span>|<span data-ttu-id="2f630-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f630-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f630-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f630-123">Accept</span></span>|<span data-ttu-id="2f630-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f630-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f630-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f630-125">Request body</span></span>
<span data-ttu-id="2f630-126">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f630-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="2f630-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f630-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="2f630-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f630-128">Property</span></span>|<span data-ttu-id="2f630-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2f630-129">Type</span></span>|<span data-ttu-id="2f630-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2f630-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f630-131">id</span><span class="sxs-lookup"><span data-stu-id="2f630-131">id</span></span>|<span data-ttu-id="2f630-132">String</span><span class="sxs-lookup"><span data-stu-id="2f630-132">String</span></span>|<span data-ttu-id="2f630-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="2f630-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2f630-134">target</span><span class="sxs-lookup"><span data-stu-id="2f630-134">target</span></span>|[<span data-ttu-id="2f630-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2f630-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2f630-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="2f630-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="2f630-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f630-137">Response</span></span>
<span data-ttu-id="2f630-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f630-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f630-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2f630-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f630-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f630-140">Request</span></span>
<span data-ttu-id="2f630-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f630-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f630-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f630-142">Response</span></span>
<span data-ttu-id="2f630-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f630-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



