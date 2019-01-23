---
title: Действие assign
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: af3952b78c3a3ff00a9b4d43938508f338feea19
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414587"
---
# <a name="assign-action"></a><span data-ttu-id="4addd-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="4addd-103">assign action</span></span>

> <span data-ttu-id="4addd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4addd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4addd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4addd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4addd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4addd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4addd-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4addd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4addd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4addd-108">Prerequisites</span></span>
<span data-ttu-id="4addd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4addd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4addd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4addd-111">Permission type</span></span>|<span data-ttu-id="4addd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4addd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4addd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4addd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4addd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4addd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4addd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4addd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4addd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4addd-116">Not supported.</span></span>|
|<span data-ttu-id="4addd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4addd-117">Application</span></span>|<span data-ttu-id="4addd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4addd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4addd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4addd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4addd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4addd-120">Request headers</span></span>
|<span data-ttu-id="4addd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4addd-121">Header</span></span>|<span data-ttu-id="4addd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4addd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4addd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4addd-123">Authorization</span></span>|<span data-ttu-id="4addd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4addd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4addd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4addd-125">Accept</span></span>|<span data-ttu-id="4addd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4addd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4addd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4addd-127">Request body</span></span>
<span data-ttu-id="4addd-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4addd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4addd-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4addd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4addd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4addd-130">Property</span></span>|<span data-ttu-id="4addd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4addd-131">Type</span></span>|<span data-ttu-id="4addd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4addd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4addd-133">assignments</span><span class="sxs-lookup"><span data-stu-id="4addd-133">assignments</span></span>|<span data-ttu-id="4addd-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4addd-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="4addd-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4addd-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4addd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4addd-136">Response</span></span>
<span data-ttu-id="4addd-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4addd-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4addd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4addd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4addd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4addd-139">Request</span></span>
<span data-ttu-id="4addd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4addd-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4addd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4addd-141">Response</span></span>
<span data-ttu-id="4addd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4addd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




