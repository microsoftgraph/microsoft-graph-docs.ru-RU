---
title: Создание Термсандкондитионсграупассигнмент
description: Создание нового объекта Термсандкондитионсграупассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e0602405de0ad794f200cdcd2dd376c051bb56e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436547"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="65a76-103">Создание Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="65a76-103">Create termsAndConditionsGroupAssignment</span></span>

<span data-ttu-id="65a76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65a76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65a76-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65a76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65a76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65a76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65a76-107">Создание нового объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="65a76-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65a76-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65a76-108">Prerequisites</span></span>
<span data-ttu-id="65a76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65a76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65a76-111">Permission type</span></span>|<span data-ttu-id="65a76-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65a76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65a76-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65a76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65a76-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a76-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65a76-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65a76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65a76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65a76-116">Not supported.</span></span>|
|<span data-ttu-id="65a76-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65a76-117">Application</span></span>|<span data-ttu-id="65a76-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a76-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65a76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65a76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="65a76-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="65a76-120">Request headers</span></span>
|<span data-ttu-id="65a76-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65a76-121">Header</span></span>|<span data-ttu-id="65a76-122">Значение</span><span class="sxs-lookup"><span data-stu-id="65a76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65a76-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65a76-123">Authorization</span></span>|<span data-ttu-id="65a76-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65a76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65a76-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65a76-125">Accept</span></span>|<span data-ttu-id="65a76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65a76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65a76-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65a76-127">Request body</span></span>
<span data-ttu-id="65a76-128">В тексте запроса добавьте представление объекта Термсандкондитионсграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65a76-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="65a76-129">В следующей таблице приведены свойства, необходимые при создании Термсандкондитионсграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="65a76-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="65a76-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="65a76-130">Property</span></span>|<span data-ttu-id="65a76-131">Тип</span><span class="sxs-lookup"><span data-stu-id="65a76-131">Type</span></span>|<span data-ttu-id="65a76-132">Описание</span><span class="sxs-lookup"><span data-stu-id="65a76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a76-133">id</span><span class="sxs-lookup"><span data-stu-id="65a76-133">id</span></span>|<span data-ttu-id="65a76-134">String</span><span class="sxs-lookup"><span data-stu-id="65a76-134">String</span></span>|<span data-ttu-id="65a76-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="65a76-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="65a76-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="65a76-136">targetGroupId</span></span>|<span data-ttu-id="65a76-137">String</span><span class="sxs-lookup"><span data-stu-id="65a76-137">String</span></span>|<span data-ttu-id="65a76-138">Уникальный идентификатор группы, которой назначена политика T&C.</span><span class="sxs-lookup"><span data-stu-id="65a76-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="65a76-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="65a76-139">Response</span></span>
<span data-ttu-id="65a76-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65a76-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a76-141">Пример</span><span class="sxs-lookup"><span data-stu-id="65a76-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="65a76-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="65a76-142">Request</span></span>
<span data-ttu-id="65a76-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65a76-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="65a76-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="65a76-144">Response</span></span>
<span data-ttu-id="65a76-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65a76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



