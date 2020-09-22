---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9dda89ef5498b2077fc60a82077190dcf2d12c8e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074463"
---
# <a name="assign-action"></a><span data-ttu-id="7c725-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="7c725-103">assign action</span></span>

<span data-ttu-id="7c725-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c725-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c725-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c725-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c725-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c725-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c725-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c725-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c725-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c725-108">Prerequisites</span></span>
<span data-ttu-id="7c725-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c725-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c725-111">Permission type</span></span>|<span data-ttu-id="7c725-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c725-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c725-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c725-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7c725-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7c725-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7c725-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c725-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c725-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c725-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c725-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c725-117">Not supported.</span></span>|
|<span data-ttu-id="7c725-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c725-118">Application</span></span>||
| <span data-ttu-id="7c725-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7c725-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7c725-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c725-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c725-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c725-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7c725-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c725-122">Request headers</span></span>
|<span data-ttu-id="7c725-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c725-123">Header</span></span>|<span data-ttu-id="7c725-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7c725-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c725-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c725-125">Authorization</span></span>|<span data-ttu-id="7c725-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c725-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c725-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7c725-127">Accept</span></span>|<span data-ttu-id="7c725-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7c725-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c725-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c725-129">Request body</span></span>
<span data-ttu-id="7c725-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c725-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7c725-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7c725-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7c725-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c725-132">Property</span></span>|<span data-ttu-id="7c725-133">Тип</span><span class="sxs-lookup"><span data-stu-id="7c725-133">Type</span></span>|<span data-ttu-id="7c725-134">Описание</span><span class="sxs-lookup"><span data-stu-id="7c725-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c725-135">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="7c725-135">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="7c725-136">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c725-136">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7c725-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c725-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c725-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c725-138">Response</span></span>
<span data-ttu-id="7c725-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c725-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c725-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7c725-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c725-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c725-141">Request</span></span>
<span data-ttu-id="7c725-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c725-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c725-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c725-143">Response</span></span>
<span data-ttu-id="7c725-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c725-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









