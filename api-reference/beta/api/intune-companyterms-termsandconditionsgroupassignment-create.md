---
title: Создание Термсандкондитионсграупассигнмент
description: Создание нового объекта Термсандкондитионсграупассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c390ed0d3d5fce21cc69adfe513169833d8f4a43
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787514"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="bf1c6-103">Создание Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="bf1c6-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="bf1c6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf1c6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf1c6-106">Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bf1c6-106">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf1c6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf1c6-107">Prerequisites</span></span>
<span data-ttu-id="bf1c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf1c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf1c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf1c6-110">Permission type</span></span>|<span data-ttu-id="bf1c6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf1c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf1c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf1c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf1c6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf1c6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf1c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf1c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf1c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-115">Not supported.</span></span>|
|<span data-ttu-id="bf1c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf1c6-116">Application</span></span>|<span data-ttu-id="bf1c6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf1c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf1c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="bf1c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf1c6-119">Request headers</span></span>
|<span data-ttu-id="bf1c6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf1c6-120">Header</span></span>|<span data-ttu-id="bf1c6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf1c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf1c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf1c6-122">Authorization</span></span>|<span data-ttu-id="bf1c6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf1c6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf1c6-124">Accept</span></span>|<span data-ttu-id="bf1c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf1c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf1c6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf1c6-126">Request body</span></span>
<span data-ttu-id="bf1c6-127">В тексте запроса добавьте представление объекта Термсандкондитионсграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-127">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="bf1c6-128">В следующей таблице приведены свойства, необходимые при создании Термсандкондитионсграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-128">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="bf1c6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf1c6-129">Property</span></span>|<span data-ttu-id="bf1c6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf1c6-130">Type</span></span>|<span data-ttu-id="bf1c6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf1c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf1c6-132">id</span><span class="sxs-lookup"><span data-stu-id="bf1c6-132">id</span></span>|<span data-ttu-id="bf1c6-133">String</span><span class="sxs-lookup"><span data-stu-id="bf1c6-133">String</span></span>|<span data-ttu-id="bf1c6-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="bf1c6-135">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="bf1c6-135">targetGroupId</span></span>|<span data-ttu-id="bf1c6-136">String</span><span class="sxs-lookup"><span data-stu-id="bf1c6-136">String</span></span>|<span data-ttu-id="bf1c6-137">Уникальный идентификатор группы, которой назначена политика Т_амп_к.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="bf1c6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf1c6-138">Response</span></span>
<span data-ttu-id="bf1c6-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf1c6-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bf1c6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf1c6-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf1c6-141">Request</span></span>
<span data-ttu-id="bf1c6-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="bf1c6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf1c6-143">Response</span></span>
<span data-ttu-id="bf1c6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf1c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





