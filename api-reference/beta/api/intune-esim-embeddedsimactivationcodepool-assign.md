---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c6b1c15bcd23ba21ac4097d424a3a817660d0b7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943630"
---
# <a name="assign-action"></a><span data-ttu-id="38aee-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="38aee-103">assign action</span></span>

> <span data-ttu-id="38aee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38aee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38aee-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38aee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38aee-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="38aee-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38aee-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38aee-107">Prerequisites</span></span>
<span data-ttu-id="38aee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38aee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38aee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38aee-110">Permission type</span></span>|<span data-ttu-id="38aee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38aee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38aee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38aee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38aee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38aee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38aee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38aee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38aee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38aee-115">Not supported.</span></span>|
|<span data-ttu-id="38aee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38aee-116">Application</span></span>|<span data-ttu-id="38aee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38aee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38aee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38aee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="38aee-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38aee-119">Request headers</span></span>
|<span data-ttu-id="38aee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38aee-120">Header</span></span>|<span data-ttu-id="38aee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="38aee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38aee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38aee-122">Authorization</span></span>|<span data-ttu-id="38aee-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38aee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38aee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="38aee-124">Accept</span></span>|<span data-ttu-id="38aee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38aee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38aee-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38aee-126">Request body</span></span>
<span data-ttu-id="38aee-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38aee-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="38aee-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="38aee-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="38aee-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="38aee-129">Property</span></span>|<span data-ttu-id="38aee-130">Тип</span><span class="sxs-lookup"><span data-stu-id="38aee-130">Type</span></span>|<span data-ttu-id="38aee-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38aee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38aee-132">assignments</span><span class="sxs-lookup"><span data-stu-id="38aee-132">assignments</span></span>|<span data-ttu-id="38aee-133">Коллекция [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="38aee-133">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="38aee-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="38aee-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="38aee-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="38aee-135">Response</span></span>
<span data-ttu-id="38aee-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38aee-136">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38aee-137">Пример</span><span class="sxs-lookup"><span data-stu-id="38aee-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="38aee-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="38aee-138">Request</span></span>
<span data-ttu-id="38aee-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38aee-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38aee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="38aee-140">Response</span></span>
<span data-ttu-id="38aee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38aee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





