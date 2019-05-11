---
title: Обновление Термсандкондитионсграупассигнмент
description: Обновление свойств объекта Термсандкондитионсграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6ee50c5b6781a78d16fc8ee05b8d9d9a53cad28
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933713"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="b7f6e-103">Обновление Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="b7f6e-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="b7f6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f6e-106">Обновление свойств объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b7f6e-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7f6e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b7f6e-107">Prerequisites</span></span>
<span data-ttu-id="b7f6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7f6e-110">Permission type</span></span>|<span data-ttu-id="b7f6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f6e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f6e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7f6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-115">Not supported.</span></span>|
|<span data-ttu-id="b7f6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7f6e-116">Application</span></span>|<span data-ttu-id="b7f6e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7f6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b7f6e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7f6e-119">Request headers</span></span>
|<span data-ttu-id="b7f6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7f6e-120">Header</span></span>|<span data-ttu-id="b7f6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7f6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f6e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7f6e-122">Authorization</span></span>|<span data-ttu-id="b7f6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7f6e-124">Accept</span></span>|<span data-ttu-id="b7f6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f6e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7f6e-126">Request body</span></span>
<span data-ttu-id="b7f6e-127">В тексте запроса добавьте представление объекта [Термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="b7f6e-128">В следующей таблице приведены свойства, необходимые при создании [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b7f6e-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="b7f6e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7f6e-129">Property</span></span>|<span data-ttu-id="b7f6e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7f6e-130">Type</span></span>|<span data-ttu-id="b7f6e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7f6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f6e-132">id</span><span class="sxs-lookup"><span data-stu-id="b7f6e-132">id</span></span>|<span data-ttu-id="b7f6e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b7f6e-133">String</span></span>|<span data-ttu-id="b7f6e-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b7f6e-135">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="b7f6e-135">targetGroupId</span></span>|<span data-ttu-id="b7f6e-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b7f6e-136">String</span></span>|<span data-ttu-id="b7f6e-137">Уникальный идентификатор группы, которой назначена политика Т_амп_к.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="b7f6e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f6e-138">Response</span></span>
<span data-ttu-id="b7f6e-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f6e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b7f6e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7f6e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7f6e-141">Request</span></span>
<span data-ttu-id="b7f6e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="b7f6e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f6e-143">Response</span></span>
<span data-ttu-id="b7f6e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7f6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




