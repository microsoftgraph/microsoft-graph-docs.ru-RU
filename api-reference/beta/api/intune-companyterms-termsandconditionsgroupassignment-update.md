---
title: Update termsAndConditionsGroupAssignment
description: Обновление свойств объекта termsAndConditionsGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 160091cfa2d9d5add4bab8ed3bd16301b90f4268
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132844"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="09bc7-103">Update termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="09bc7-103">Update termsAndConditionsGroupAssignment</span></span>

<span data-ttu-id="09bc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09bc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09bc7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09bc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09bc7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09bc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09bc7-107">Обновление свойств объекта [termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="09bc7-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09bc7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09bc7-108">Prerequisites</span></span>
<span data-ttu-id="09bc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09bc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09bc7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09bc7-111">Permission type</span></span>|<span data-ttu-id="09bc7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09bc7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09bc7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09bc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09bc7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bc7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="09bc7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09bc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09bc7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09bc7-116">Not supported.</span></span>|
|<span data-ttu-id="09bc7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="09bc7-117">Application</span></span>|<span data-ttu-id="09bc7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bc7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09bc7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09bc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="09bc7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09bc7-120">Request headers</span></span>
|<span data-ttu-id="09bc7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09bc7-121">Header</span></span>|<span data-ttu-id="09bc7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09bc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09bc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09bc7-123">Authorization</span></span>|<span data-ttu-id="09bc7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09bc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09bc7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09bc7-125">Accept</span></span>|<span data-ttu-id="09bc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09bc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09bc7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09bc7-127">Request body</span></span>
<span data-ttu-id="09bc7-128">В теле запроса поставляем представление JSON для объекта [termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="09bc7-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="09bc7-129">В следующей таблице показаны свойства, необходимые при создании [терминовAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="09bc7-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="09bc7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="09bc7-130">Property</span></span>|<span data-ttu-id="09bc7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="09bc7-131">Type</span></span>|<span data-ttu-id="09bc7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="09bc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09bc7-133">id</span><span class="sxs-lookup"><span data-stu-id="09bc7-133">id</span></span>|<span data-ttu-id="09bc7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="09bc7-134">String</span></span>|<span data-ttu-id="09bc7-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="09bc7-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="09bc7-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="09bc7-136">targetGroupId</span></span>|<span data-ttu-id="09bc7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="09bc7-137">String</span></span>|<span data-ttu-id="09bc7-138">Уникальный идентификатор группы, для&C.</span><span class="sxs-lookup"><span data-stu-id="09bc7-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="09bc7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="09bc7-139">Response</span></span>
<span data-ttu-id="09bc7-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="09bc7-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09bc7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="09bc7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="09bc7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="09bc7-142">Request</span></span>
<span data-ttu-id="09bc7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09bc7-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="09bc7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="09bc7-144">Response</span></span>
<span data-ttu-id="09bc7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09bc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




