---
title: Действие assign
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 88b6b7eef26e0187bacf2ee647c95452a1642cba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316109"
---
# <a name="assign-action"></a><span data-ttu-id="fcc6f-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="fcc6f-103">assign action</span></span>

> <span data-ttu-id="fcc6f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcc6f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcc6f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcc6f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcc6f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcc6f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fcc6f-108">Prerequisites</span></span>
<span data-ttu-id="fcc6f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcc6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcc6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcc6f-111">Permission type</span></span>|<span data-ttu-id="fcc6f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcc6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcc6f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcc6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcc6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcc6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fcc6f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcc6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcc6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-116">Not supported.</span></span>|
|<span data-ttu-id="fcc6f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcc6f-117">Application</span></span>|<span data-ttu-id="fcc6f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcc6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcc6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="fcc6f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcc6f-120">Request headers</span></span>
|<span data-ttu-id="fcc6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcc6f-121">Header</span></span>|<span data-ttu-id="fcc6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcc6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcc6f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcc6f-123">Authorization</span></span>|<span data-ttu-id="fcc6f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fcc6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcc6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcc6f-125">Accept</span></span>|<span data-ttu-id="fcc6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcc6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcc6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcc6f-127">Request body</span></span>
<span data-ttu-id="fcc6f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fcc6f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fcc6f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcc6f-130">Property</span></span>|<span data-ttu-id="fcc6f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc6f-131">Type</span></span>|<span data-ttu-id="fcc6f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc6f-133">assignments</span><span class="sxs-lookup"><span data-stu-id="fcc6f-133">assignments</span></span>|<span data-ttu-id="fcc6f-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fcc6f-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="fcc6f-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcc6f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fcc6f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcc6f-136">Response</span></span>
<span data-ttu-id="fcc6f-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcc6f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fcc6f-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcc6f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcc6f-139">Request</span></span>
<span data-ttu-id="fcc6f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fcc6f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcc6f-141">Response</span></span>
<span data-ttu-id="fcc6f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fcc6f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





