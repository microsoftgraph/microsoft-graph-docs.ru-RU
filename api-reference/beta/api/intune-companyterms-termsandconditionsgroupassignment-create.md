---
title: Создание termsAndConditionsGroupAssignment
description: Создание нового объекта termsAndConditionsGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d02e0f1a2e4f0a79f6baa9fec76a68c45ef3dec7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878584"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="5c74d-103">Создание termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="5c74d-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="5c74d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c74d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c74d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c74d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c74d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c74d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c74d-107">Создание нового объекта [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5c74d-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c74d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c74d-108">Prerequisites</span></span>
<span data-ttu-id="5c74d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c74d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c74d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c74d-111">Permission type</span></span>|<span data-ttu-id="5c74d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c74d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c74d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c74d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c74d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c74d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c74d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c74d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c74d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c74d-116">Not supported.</span></span>|
|<span data-ttu-id="5c74d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c74d-117">Application</span></span>|<span data-ttu-id="5c74d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c74d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c74d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c74d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="5c74d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c74d-120">Request headers</span></span>
|<span data-ttu-id="5c74d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c74d-121">Header</span></span>|<span data-ttu-id="5c74d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5c74d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c74d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c74d-123">Authorization</span></span>|<span data-ttu-id="5c74d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c74d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c74d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c74d-125">Accept</span></span>|<span data-ttu-id="5c74d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c74d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c74d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c74d-127">Request body</span></span>
<span data-ttu-id="5c74d-128">В тексте запроса укажите представление JSON для объекта termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="5c74d-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="5c74d-129">В следующей таблице показаны свойства, которые необходимы для создания termsAndConditionsGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="5c74d-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="5c74d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c74d-130">Property</span></span>|<span data-ttu-id="5c74d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5c74d-131">Type</span></span>|<span data-ttu-id="5c74d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5c74d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c74d-133">id</span><span class="sxs-lookup"><span data-stu-id="5c74d-133">id</span></span>|<span data-ttu-id="5c74d-134">String</span><span class="sxs-lookup"><span data-stu-id="5c74d-134">String</span></span>|<span data-ttu-id="5c74d-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="5c74d-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5c74d-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="5c74d-136">targetGroupId</span></span>|<span data-ttu-id="5c74d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5c74d-137">String</span></span>|<span data-ttu-id="5c74d-138">Уникальный идентификатор группы, которая назначена политика T & C.</span><span class="sxs-lookup"><span data-stu-id="5c74d-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5c74d-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c74d-139">Response</span></span>
<span data-ttu-id="5c74d-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5c74d-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c74d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5c74d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c74d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c74d-142">Request</span></span>
<span data-ttu-id="5c74d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c74d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="5c74d-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c74d-144">Response</span></span>
<span data-ttu-id="5c74d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c74d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





