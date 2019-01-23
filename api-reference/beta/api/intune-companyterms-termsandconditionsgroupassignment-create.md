---
title: Создание termsAndConditionsGroupAssignment
description: Создание нового объекта termsAndConditionsGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1d5d9576e886530bd4cf8af345390e9b9170a80
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417121"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="c440d-103">Создание termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="c440d-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="c440d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c440d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c440d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c440d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c440d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c440d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c440d-107">Создание нового объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c440d-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c440d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c440d-108">Prerequisites</span></span>
<span data-ttu-id="c440d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c440d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c440d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c440d-111">Permission type</span></span>|<span data-ttu-id="c440d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c440d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c440d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c440d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c440d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c440d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c440d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c440d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c440d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c440d-116">Not supported.</span></span>|
|<span data-ttu-id="c440d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c440d-117">Application</span></span>|<span data-ttu-id="c440d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c440d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c440d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c440d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c440d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c440d-120">Request headers</span></span>
|<span data-ttu-id="c440d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c440d-121">Header</span></span>|<span data-ttu-id="c440d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c440d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c440d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c440d-123">Authorization</span></span>|<span data-ttu-id="c440d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c440d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c440d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c440d-125">Accept</span></span>|<span data-ttu-id="c440d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c440d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c440d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c440d-127">Request body</span></span>
<span data-ttu-id="c440d-128">В тексте запроса укажите представление JSON для объекта termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="c440d-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="c440d-129">В следующей таблице показаны свойства, которые необходимы для создания termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="c440d-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="c440d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c440d-130">Property</span></span>|<span data-ttu-id="c440d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c440d-131">Type</span></span>|<span data-ttu-id="c440d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c440d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c440d-133">id</span><span class="sxs-lookup"><span data-stu-id="c440d-133">id</span></span>|<span data-ttu-id="c440d-134">String</span><span class="sxs-lookup"><span data-stu-id="c440d-134">String</span></span>|<span data-ttu-id="c440d-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="c440d-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c440d-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="c440d-136">targetGroupId</span></span>|<span data-ttu-id="c440d-137">String</span><span class="sxs-lookup"><span data-stu-id="c440d-137">String</span></span>|<span data-ttu-id="c440d-138">Уникальный идентификатор группы, которая назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="c440d-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="c440d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c440d-139">Response</span></span>
<span data-ttu-id="c440d-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c440d-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c440d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c440d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c440d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c440d-142">Request</span></span>
<span data-ttu-id="c440d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c440d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="c440d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c440d-144">Response</span></span>
<span data-ttu-id="c440d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c440d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




