---
title: Создание Термсандкондитионсграупассигнмент
description: Создание нового объекта Термсандкондитионсграупассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebb289d651037d830bb9d4c58f21672154c5d257
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760076"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="ea5fc-103">Создание Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="ea5fc-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="ea5fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea5fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea5fc-106">Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ea5fc-106">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea5fc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea5fc-107">Prerequisites</span></span>
<span data-ttu-id="ea5fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea5fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea5fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea5fc-110">Permission type</span></span>|<span data-ttu-id="ea5fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea5fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea5fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea5fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea5fc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5fc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ea5fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea5fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea5fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-115">Not supported.</span></span>|
|<span data-ttu-id="ea5fc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea5fc-116">Application</span></span>|<span data-ttu-id="ea5fc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5fc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea5fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea5fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ea5fc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea5fc-119">Request headers</span></span>
|<span data-ttu-id="ea5fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea5fc-120">Header</span></span>|<span data-ttu-id="ea5fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea5fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea5fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea5fc-122">Authorization</span></span>|<span data-ttu-id="ea5fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea5fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea5fc-124">Accept</span></span>|<span data-ttu-id="ea5fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea5fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea5fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea5fc-126">Request body</span></span>
<span data-ttu-id="ea5fc-127">В тексте запроса добавьте представление объекта Термсандкондитионсграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-127">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="ea5fc-128">В следующей таблице приведены свойства, необходимые при создании Термсандкондитионсграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-128">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="ea5fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea5fc-129">Property</span></span>|<span data-ttu-id="ea5fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ea5fc-130">Type</span></span>|<span data-ttu-id="ea5fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ea5fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea5fc-132">id</span><span class="sxs-lookup"><span data-stu-id="ea5fc-132">id</span></span>|<span data-ttu-id="ea5fc-133">String</span><span class="sxs-lookup"><span data-stu-id="ea5fc-133">String</span></span>|<span data-ttu-id="ea5fc-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ea5fc-135">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="ea5fc-135">targetGroupId</span></span>|<span data-ttu-id="ea5fc-136">String</span><span class="sxs-lookup"><span data-stu-id="ea5fc-136">String</span></span>|<span data-ttu-id="ea5fc-137">Уникальный идентификатор группы, которой назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ea5fc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea5fc-138">Response</span></span>
<span data-ttu-id="ea5fc-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea5fc-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ea5fc-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea5fc-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea5fc-141">Request</span></span>
<span data-ttu-id="ea5fc-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="ea5fc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea5fc-143">Response</span></span>
<span data-ttu-id="ea5fc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea5fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




