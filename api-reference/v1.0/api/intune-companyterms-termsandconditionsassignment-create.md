---
title: Создание объекта termsAndConditionsAssignment
description: Создание объекта termsAndConditionsAssignment.
ms.openlocfilehash: 9e113ae57c4bebce3f4bcc016ab6afadc3186e0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025881"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="3b123-103">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="3b123-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="3b123-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b123-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b123-105">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3b123-105">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b123-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3b123-106">Prerequisites</span></span>
<span data-ttu-id="3b123-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b123-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b123-109">Permission type</span></span>|<span data-ttu-id="3b123-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b123-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b123-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b123-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b123-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b123-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b123-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b123-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b123-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b123-114">Not supported.</span></span>|
|<span data-ttu-id="3b123-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b123-115">Application</span></span>|<span data-ttu-id="3b123-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b123-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b123-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b123-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3b123-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b123-118">Request headers</span></span>
|<span data-ttu-id="3b123-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b123-119">Header</span></span>|<span data-ttu-id="3b123-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3b123-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b123-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b123-121">Authorization</span></span>|<span data-ttu-id="3b123-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b123-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b123-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3b123-123">Accept</span></span>|<span data-ttu-id="3b123-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b123-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b123-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b123-125">Request body</span></span>
<span data-ttu-id="3b123-126">В тексте запроса добавьте представление объекта termsAndConditionsAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b123-126">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="3b123-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="3b123-127">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="3b123-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b123-128">Property</span></span>|<span data-ttu-id="3b123-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3b123-129">Type</span></span>|<span data-ttu-id="3b123-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b123-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b123-131">id</span><span class="sxs-lookup"><span data-stu-id="3b123-131">id</span></span>|<span data-ttu-id="3b123-132">String</span><span class="sxs-lookup"><span data-stu-id="3b123-132">String</span></span>|<span data-ttu-id="3b123-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="3b123-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3b123-134">target</span><span class="sxs-lookup"><span data-stu-id="3b123-134">target</span></span>|[<span data-ttu-id="3b123-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3b123-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3b123-136">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="3b123-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="3b123-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b123-137">Response</span></span>
<span data-ttu-id="3b123-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b123-138">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b123-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3b123-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b123-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b123-140">Request</span></span>
<span data-ttu-id="3b123-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b123-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b123-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b123-142">Response</span></span>
<span data-ttu-id="3b123-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3b123-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



