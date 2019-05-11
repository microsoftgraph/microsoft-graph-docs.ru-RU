---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29b3eed34506609561777175f358f56ad6f3b6f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908083"
---
# <a name="assign-action"></a><span data-ttu-id="52f82-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="52f82-103">assign action</span></span>

> <span data-ttu-id="52f82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52f82-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52f82-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="52f82-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52f82-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="52f82-107">Prerequisites</span></span>
<span data-ttu-id="52f82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52f82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52f82-110">Permission type</span></span>|<span data-ttu-id="52f82-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52f82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52f82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52f82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52f82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52f82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52f82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52f82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f82-115">Not supported.</span></span>|
|<span data-ttu-id="52f82-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52f82-116">Application</span></span>|<span data-ttu-id="52f82-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52f82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="52f82-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f82-119">Request headers</span></span>
|<span data-ttu-id="52f82-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52f82-120">Header</span></span>|<span data-ttu-id="52f82-121">Значение</span><span class="sxs-lookup"><span data-stu-id="52f82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52f82-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52f82-122">Authorization</span></span>|<span data-ttu-id="52f82-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52f82-124">Accept</span><span class="sxs-lookup"><span data-stu-id="52f82-124">Accept</span></span>|<span data-ttu-id="52f82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52f82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52f82-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f82-126">Request body</span></span>
<span data-ttu-id="52f82-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52f82-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="52f82-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="52f82-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="52f82-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="52f82-129">Property</span></span>|<span data-ttu-id="52f82-130">Тип</span><span class="sxs-lookup"><span data-stu-id="52f82-130">Type</span></span>|<span data-ttu-id="52f82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="52f82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f82-132">assignments</span><span class="sxs-lookup"><span data-stu-id="52f82-132">assignments</span></span>|<span data-ttu-id="52f82-133">Коллекция [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52f82-133">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="52f82-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="52f82-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="52f82-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="52f82-135">Response</span></span>
<span data-ttu-id="52f82-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52f82-136">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52f82-137">Пример</span><span class="sxs-lookup"><span data-stu-id="52f82-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="52f82-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f82-138">Request</span></span>
<span data-ttu-id="52f82-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52f82-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52f82-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f82-140">Response</span></span>
<span data-ttu-id="52f82-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52f82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




