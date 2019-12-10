---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 046b50b5fe572ee3203606a387c14da9f96faa61
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940042"
---
# <a name="assign-action"></a><span data-ttu-id="80ada-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="80ada-103">assign action</span></span>

> <span data-ttu-id="80ada-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80ada-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80ada-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80ada-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80ada-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="80ada-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80ada-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="80ada-107">Prerequisites</span></span>
<span data-ttu-id="80ada-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ada-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80ada-110">Permission type</span></span>|<span data-ttu-id="80ada-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80ada-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80ada-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80ada-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="80ada-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="80ada-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="80ada-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ada-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80ada-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80ada-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80ada-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80ada-116">Not supported.</span></span>|
|<span data-ttu-id="80ada-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80ada-117">Application</span></span>||
| <span data-ttu-id="80ada-118">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="80ada-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="80ada-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ada-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80ada-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80ada-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="80ada-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80ada-121">Request headers</span></span>
|<span data-ttu-id="80ada-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80ada-122">Header</span></span>|<span data-ttu-id="80ada-123">Значение</span><span class="sxs-lookup"><span data-stu-id="80ada-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80ada-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80ada-124">Authorization</span></span>|<span data-ttu-id="80ada-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80ada-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80ada-126">Accept</span><span class="sxs-lookup"><span data-stu-id="80ada-126">Accept</span></span>|<span data-ttu-id="80ada-127">application/json</span><span class="sxs-lookup"><span data-stu-id="80ada-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ada-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80ada-128">Request body</span></span>
<span data-ttu-id="80ada-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80ada-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="80ada-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="80ada-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="80ada-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="80ada-131">Property</span></span>|<span data-ttu-id="80ada-132">Тип</span><span class="sxs-lookup"><span data-stu-id="80ada-132">Type</span></span>|<span data-ttu-id="80ada-133">Описание</span><span class="sxs-lookup"><span data-stu-id="80ada-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80ada-134">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="80ada-134">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="80ada-135">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="80ada-135">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="80ada-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="80ada-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="80ada-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="80ada-137">Response</span></span>
<span data-ttu-id="80ada-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80ada-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80ada-139">Пример</span><span class="sxs-lookup"><span data-stu-id="80ada-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="80ada-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="80ada-140">Request</span></span>
<span data-ttu-id="80ada-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80ada-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80ada-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="80ada-142">Response</span></span>
<span data-ttu-id="80ada-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80ada-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








