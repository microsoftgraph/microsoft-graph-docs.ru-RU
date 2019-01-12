---
title: Обновление termsAndConditionsGroupAssignment
description: Обновление свойства объекта termsAndConditionsGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f93efc985db56f12ac6cf01840a525915dd8a724
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929510"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="33493-103">Обновление termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="33493-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="33493-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33493-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33493-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33493-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33493-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="33493-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33493-107">Обновление свойства объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="33493-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33493-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33493-108">Prerequisites</span></span>
<span data-ttu-id="33493-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33493-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33493-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33493-111">Permission type</span></span>|<span data-ttu-id="33493-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33493-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33493-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33493-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33493-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33493-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="33493-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33493-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33493-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33493-116">Not supported.</span></span>|
|<span data-ttu-id="33493-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33493-117">Application</span></span>|<span data-ttu-id="33493-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33493-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33493-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33493-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="33493-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33493-120">Request headers</span></span>
|<span data-ttu-id="33493-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33493-121">Header</span></span>|<span data-ttu-id="33493-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33493-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33493-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33493-123">Authorization</span></span>|<span data-ttu-id="33493-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="33493-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33493-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33493-125">Accept</span></span>|<span data-ttu-id="33493-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33493-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33493-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33493-127">Request body</span></span>
<span data-ttu-id="33493-128">В тексте запроса укажите представление JSON для объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="33493-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="33493-129">В следующей таблице показаны свойства, которые необходимы для создания [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="33493-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="33493-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="33493-130">Property</span></span>|<span data-ttu-id="33493-131">Тип</span><span class="sxs-lookup"><span data-stu-id="33493-131">Type</span></span>|<span data-ttu-id="33493-132">Описание</span><span class="sxs-lookup"><span data-stu-id="33493-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33493-133">id</span><span class="sxs-lookup"><span data-stu-id="33493-133">id</span></span>|<span data-ttu-id="33493-134">String</span><span class="sxs-lookup"><span data-stu-id="33493-134">String</span></span>|<span data-ttu-id="33493-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="33493-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="33493-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="33493-136">targetGroupId</span></span>|<span data-ttu-id="33493-137">String</span><span class="sxs-lookup"><span data-stu-id="33493-137">String</span></span>|<span data-ttu-id="33493-138">Уникальный идентификатор группы, которая назначена политика T & C.</span><span class="sxs-lookup"><span data-stu-id="33493-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="33493-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="33493-139">Response</span></span>
<span data-ttu-id="33493-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="33493-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33493-141">Пример</span><span class="sxs-lookup"><span data-stu-id="33493-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="33493-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="33493-142">Request</span></span>
<span data-ttu-id="33493-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33493-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="33493-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="33493-144">Response</span></span>
<span data-ttu-id="33493-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="33493-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```





