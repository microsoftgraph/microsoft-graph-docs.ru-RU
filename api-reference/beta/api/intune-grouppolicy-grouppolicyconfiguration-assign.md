---
title: Действие assign
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06b96d793c07ba5fd3bc776d4b389c77708c8519
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430664"
---
# <a name="assign-action"></a><span data-ttu-id="66646-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="66646-103">assign action</span></span>

> <span data-ttu-id="66646-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66646-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66646-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66646-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66646-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66646-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66646-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66646-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66646-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66646-108">Prerequisites</span></span>
<span data-ttu-id="66646-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66646-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66646-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66646-111">Permission type</span></span>|<span data-ttu-id="66646-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66646-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66646-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66646-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66646-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66646-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="66646-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66646-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66646-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66646-116">Not supported.</span></span>|
|<span data-ttu-id="66646-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66646-117">Application</span></span>|<span data-ttu-id="66646-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66646-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66646-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66646-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="66646-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66646-120">Request headers</span></span>
|<span data-ttu-id="66646-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66646-121">Header</span></span>|<span data-ttu-id="66646-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66646-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66646-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66646-123">Authorization</span></span>|<span data-ttu-id="66646-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="66646-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66646-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66646-125">Accept</span></span>|<span data-ttu-id="66646-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66646-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66646-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66646-127">Request body</span></span>
<span data-ttu-id="66646-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66646-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="66646-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="66646-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="66646-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66646-130">Property</span></span>|<span data-ttu-id="66646-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66646-131">Type</span></span>|<span data-ttu-id="66646-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66646-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66646-133">assignments</span><span class="sxs-lookup"><span data-stu-id="66646-133">assignments</span></span>|<span data-ttu-id="66646-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="66646-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="66646-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66646-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66646-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="66646-136">Response</span></span>
<span data-ttu-id="66646-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="66646-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66646-138">Пример</span><span class="sxs-lookup"><span data-stu-id="66646-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="66646-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="66646-139">Request</span></span>
<span data-ttu-id="66646-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66646-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="66646-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="66646-141">Response</span></span>
<span data-ttu-id="66646-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66646-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




