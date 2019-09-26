---
title: Создание Термсандкондитионсграупассигнмент
description: Создание нового объекта Термсандкондитионсграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c055f2a8d5d29da58ace22fd7a9f8722cef2510
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170422"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="23c49-103">Создание Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="23c49-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="23c49-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23c49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23c49-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23c49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23c49-106">Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="23c49-106">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23c49-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23c49-107">Prerequisites</span></span>
<span data-ttu-id="23c49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23c49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23c49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23c49-110">Permission type</span></span>|<span data-ttu-id="23c49-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23c49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23c49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23c49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23c49-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23c49-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23c49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23c49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23c49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23c49-115">Not supported.</span></span>|
|<span data-ttu-id="23c49-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23c49-116">Application</span></span>|<span data-ttu-id="23c49-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23c49-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23c49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23c49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="23c49-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23c49-119">Request headers</span></span>
|<span data-ttu-id="23c49-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23c49-120">Header</span></span>|<span data-ttu-id="23c49-121">Значение</span><span class="sxs-lookup"><span data-stu-id="23c49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23c49-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23c49-122">Authorization</span></span>|<span data-ttu-id="23c49-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23c49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23c49-124">Accept</span><span class="sxs-lookup"><span data-stu-id="23c49-124">Accept</span></span>|<span data-ttu-id="23c49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23c49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23c49-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23c49-126">Request body</span></span>
<span data-ttu-id="23c49-127">В тексте запроса добавьте представление объекта Термсандкондитионсграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23c49-127">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="23c49-128">В следующей таблице приведены свойства, необходимые при создании Термсандкондитионсграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="23c49-128">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="23c49-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="23c49-129">Property</span></span>|<span data-ttu-id="23c49-130">Тип</span><span class="sxs-lookup"><span data-stu-id="23c49-130">Type</span></span>|<span data-ttu-id="23c49-131">Описание</span><span class="sxs-lookup"><span data-stu-id="23c49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23c49-132">id</span><span class="sxs-lookup"><span data-stu-id="23c49-132">id</span></span>|<span data-ttu-id="23c49-133">String</span><span class="sxs-lookup"><span data-stu-id="23c49-133">String</span></span>|<span data-ttu-id="23c49-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="23c49-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="23c49-135">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="23c49-135">targetGroupId</span></span>|<span data-ttu-id="23c49-136">String.</span><span class="sxs-lookup"><span data-stu-id="23c49-136">String</span></span>|<span data-ttu-id="23c49-137">Уникальный идентификатор группы, которой назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="23c49-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="23c49-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="23c49-138">Response</span></span>
<span data-ttu-id="23c49-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23c49-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23c49-140">Пример</span><span class="sxs-lookup"><span data-stu-id="23c49-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="23c49-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="23c49-141">Request</span></span>
<span data-ttu-id="23c49-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23c49-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="23c49-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="23c49-143">Response</span></span>
<span data-ttu-id="23c49-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23c49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




