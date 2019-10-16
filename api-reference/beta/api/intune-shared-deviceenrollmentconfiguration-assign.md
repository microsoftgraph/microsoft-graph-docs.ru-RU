---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 941b06cb2104956df25872b04383cc865bbeec4c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536163"
---
# <a name="assign-action"></a><span data-ttu-id="0b73d-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="0b73d-103">assign action</span></span>

> <span data-ttu-id="0b73d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b73d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b73d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b73d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b73d-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b73d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b73d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b73d-107">Prerequisites</span></span>
<span data-ttu-id="0b73d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b73d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b73d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b73d-110">Permission type</span></span>|<span data-ttu-id="0b73d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b73d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b73d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b73d-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0b73d-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="0b73d-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0b73d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b73d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0b73d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b73d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b73d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b73d-116">Not supported.</span></span>|
|<span data-ttu-id="0b73d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b73d-117">Application</span></span>||
| <span data-ttu-id="0b73d-118">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="0b73d-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0b73d-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b73d-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b73d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b73d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0b73d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b73d-121">Request headers</span></span>
|<span data-ttu-id="0b73d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b73d-122">Header</span></span>|<span data-ttu-id="0b73d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0b73d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b73d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b73d-124">Authorization</span></span>|<span data-ttu-id="0b73d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b73d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b73d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0b73d-126">Accept</span></span>|<span data-ttu-id="0b73d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0b73d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b73d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b73d-128">Request body</span></span>
<span data-ttu-id="0b73d-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b73d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0b73d-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0b73d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0b73d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b73d-131">Property</span></span>|<span data-ttu-id="0b73d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0b73d-132">Type</span></span>|<span data-ttu-id="0b73d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0b73d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b73d-134">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="0b73d-134">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="0b73d-135">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0b73d-135">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0b73d-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b73d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0b73d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b73d-137">Response</span></span>
<span data-ttu-id="0b73d-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b73d-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b73d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0b73d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b73d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b73d-140">Request</span></span>
<span data-ttu-id="0b73d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b73d-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

Content-type: application/json
Content-length: 304

{
  "enrollmentConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0b73d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b73d-142">Response</span></span>
<span data-ttu-id="0b73d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b73d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






