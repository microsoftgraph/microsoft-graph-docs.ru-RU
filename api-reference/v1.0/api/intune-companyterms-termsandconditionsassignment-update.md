---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 84213c90925882492442671b4702082b7385a25c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911786"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="9dae7-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9dae7-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="9dae7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9dae7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dae7-105">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9dae7-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9dae7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9dae7-106">Prerequisites</span></span>
<span data-ttu-id="9dae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dae7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dae7-109">Permission type</span></span>|<span data-ttu-id="9dae7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dae7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dae7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dae7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9dae7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dae7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9dae7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dae7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dae7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dae7-114">Not supported.</span></span>|
|<span data-ttu-id="9dae7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dae7-115">Application</span></span>|<span data-ttu-id="9dae7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dae7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dae7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dae7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9dae7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dae7-118">Request headers</span></span>
|<span data-ttu-id="9dae7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dae7-119">Header</span></span>|<span data-ttu-id="9dae7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9dae7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dae7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dae7-121">Authorization</span></span>|<span data-ttu-id="9dae7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9dae7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dae7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9dae7-123">Accept</span></span>|<span data-ttu-id="9dae7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9dae7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dae7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dae7-125">Request body</span></span>
<span data-ttu-id="9dae7-126">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dae7-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="9dae7-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9dae7-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="9dae7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dae7-128">Property</span></span>|<span data-ttu-id="9dae7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9dae7-129">Type</span></span>|<span data-ttu-id="9dae7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9dae7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dae7-131">id</span><span class="sxs-lookup"><span data-stu-id="9dae7-131">id</span></span>|<span data-ttu-id="9dae7-132">String</span><span class="sxs-lookup"><span data-stu-id="9dae7-132">String</span></span>|<span data-ttu-id="9dae7-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9dae7-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9dae7-134">target</span><span class="sxs-lookup"><span data-stu-id="9dae7-134">target</span></span>|[<span data-ttu-id="9dae7-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9dae7-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9dae7-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="9dae7-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="9dae7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dae7-137">Response</span></span>
<span data-ttu-id="9dae7-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9dae7-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dae7-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9dae7-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9dae7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dae7-140">Request</span></span>
<span data-ttu-id="9dae7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dae7-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9dae7-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="9dae7-142">Response</span></span>
<span data-ttu-id="9dae7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9dae7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



