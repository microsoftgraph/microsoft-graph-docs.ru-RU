---
title: Обновление Термсандкондитионсграупассигнмент
description: Обновление свойств объекта Термсандкондитионсграупассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c7b18dda513d373cc1a7420ad94d63c0e176e22a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760048"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="ad084-103">Обновление Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="ad084-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="ad084-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad084-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad084-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad084-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad084-106">Обновление свойств объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ad084-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad084-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad084-107">Prerequisites</span></span>
<span data-ttu-id="ad084-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad084-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad084-110">Permission type</span></span>|<span data-ttu-id="ad084-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad084-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad084-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad084-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad084-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad084-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ad084-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad084-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad084-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad084-115">Not supported.</span></span>|
|<span data-ttu-id="ad084-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad084-116">Application</span></span>|<span data-ttu-id="ad084-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad084-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad084-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad084-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ad084-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad084-119">Request headers</span></span>
|<span data-ttu-id="ad084-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad084-120">Header</span></span>|<span data-ttu-id="ad084-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ad084-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad084-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad084-122">Authorization</span></span>|<span data-ttu-id="ad084-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad084-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad084-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ad084-124">Accept</span></span>|<span data-ttu-id="ad084-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad084-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad084-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad084-126">Request body</span></span>
<span data-ttu-id="ad084-127">В тексте запроса добавьте представление объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad084-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="ad084-128">В следующей таблице приведены свойства, необходимые при создании [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad084-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="ad084-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad084-129">Property</span></span>|<span data-ttu-id="ad084-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ad084-130">Type</span></span>|<span data-ttu-id="ad084-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ad084-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad084-132">id</span><span class="sxs-lookup"><span data-stu-id="ad084-132">id</span></span>|<span data-ttu-id="ad084-133">String</span><span class="sxs-lookup"><span data-stu-id="ad084-133">String</span></span>|<span data-ttu-id="ad084-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="ad084-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ad084-135">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="ad084-135">targetGroupId</span></span>|<span data-ttu-id="ad084-136">String</span><span class="sxs-lookup"><span data-stu-id="ad084-136">String</span></span>|<span data-ttu-id="ad084-137">Уникальный идентификатор группы, которой назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="ad084-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ad084-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad084-138">Response</span></span>
<span data-ttu-id="ad084-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad084-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad084-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ad084-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad084-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad084-141">Request</span></span>
<span data-ttu-id="ad084-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad084-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="ad084-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad084-143">Response</span></span>
<span data-ttu-id="ad084-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad084-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




