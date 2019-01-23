---
title: Действие assign
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74e8e85a35429d2cd57843af62578cd676fc5898
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396128"
---
# <a name="assign-action"></a><span data-ttu-id="097bc-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="097bc-103">assign action</span></span>

> <span data-ttu-id="097bc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="097bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="097bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="097bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="097bc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="097bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="097bc-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="097bc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="097bc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="097bc-108">Prerequisites</span></span>
<span data-ttu-id="097bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="097bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="097bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="097bc-111">Permission type</span></span>|<span data-ttu-id="097bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="097bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="097bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="097bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="097bc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="097bc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="097bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="097bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="097bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="097bc-116">Not supported.</span></span>|
|<span data-ttu-id="097bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="097bc-117">Application</span></span>|<span data-ttu-id="097bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="097bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="097bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="097bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="097bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="097bc-120">Request headers</span></span>
|<span data-ttu-id="097bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="097bc-121">Header</span></span>|<span data-ttu-id="097bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="097bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="097bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="097bc-123">Authorization</span></span>|<span data-ttu-id="097bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="097bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="097bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="097bc-125">Accept</span></span>|<span data-ttu-id="097bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="097bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="097bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="097bc-127">Request body</span></span>
<span data-ttu-id="097bc-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="097bc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="097bc-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="097bc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="097bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="097bc-130">Property</span></span>|<span data-ttu-id="097bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="097bc-131">Type</span></span>|<span data-ttu-id="097bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="097bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="097bc-133">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="097bc-133">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="097bc-134">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="097bc-134">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="097bc-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="097bc-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="097bc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="097bc-136">Response</span></span>
<span data-ttu-id="097bc-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="097bc-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="097bc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="097bc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="097bc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="097bc-139">Request</span></span>
<span data-ttu-id="097bc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="097bc-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="097bc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="097bc-141">Response</span></span>
<span data-ttu-id="097bc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="097bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




