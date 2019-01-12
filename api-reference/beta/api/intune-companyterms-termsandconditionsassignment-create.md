---
title: Создание объекта termsAndConditionsAssignment
description: Создание объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 704aa0a3f86c3b65b3f2882af21010c46c02f1b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976137"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="e7c3a-103">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e7c3a-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="e7c3a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7c3a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7c3a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7c3a-107">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e7c3a-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7c3a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7c3a-108">Prerequisites</span></span>
<span data-ttu-id="e7c3a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7c3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7c3a-111">Permission type</span></span>|<span data-ttu-id="e7c3a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7c3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7c3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c3a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c3a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7c3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7c3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-116">Not supported.</span></span>|
|<span data-ttu-id="e7c3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7c3a-117">Application</span></span>|<span data-ttu-id="e7c3a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7c3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e7c3a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7c3a-120">Request headers</span></span>
|<span data-ttu-id="e7c3a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7c3a-121">Header</span></span>|<span data-ttu-id="e7c3a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e7c3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c3a-123">Authorization</span></span>|<span data-ttu-id="e7c3a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7c3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e7c3a-125">Accept</span></span>|<span data-ttu-id="e7c3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c3a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7c3a-127">Request body</span></span>
<span data-ttu-id="e7c3a-128">В тексте запроса добавьте представление объекта termsAndConditionsAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="e7c3a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="e7c3a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7c3a-130">Property</span></span>|<span data-ttu-id="e7c3a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7c3a-131">Type</span></span>|<span data-ttu-id="e7c3a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7c3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c3a-133">id</span><span class="sxs-lookup"><span data-stu-id="e7c3a-133">id</span></span>|<span data-ttu-id="e7c3a-134">String</span><span class="sxs-lookup"><span data-stu-id="e7c3a-134">String</span></span>|<span data-ttu-id="e7c3a-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e7c3a-136">target</span><span class="sxs-lookup"><span data-stu-id="e7c3a-136">target</span></span>|[<span data-ttu-id="e7c3a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e7c3a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e7c3a-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="e7c3a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7c3a-139">Response</span></span>
<span data-ttu-id="e7c3a-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c3a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e7c3a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7c3a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7c3a-142">Request</span></span>
<span data-ttu-id="e7c3a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7c3a-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7c3a-144">Response</span></span>
<span data-ttu-id="e7c3a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7c3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





