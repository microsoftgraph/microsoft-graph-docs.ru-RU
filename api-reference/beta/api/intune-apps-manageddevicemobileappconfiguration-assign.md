---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 019abecc0f9d7560f907652166f8e2ba54cfa2c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974751"
---
# <a name="assign-action"></a><span data-ttu-id="20726-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="20726-103">assign action</span></span>

> <span data-ttu-id="20726-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20726-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20726-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20726-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20726-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="20726-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20726-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20726-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20726-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="20726-108">Prerequisites</span></span>
<span data-ttu-id="20726-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20726-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20726-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20726-111">Permission type</span></span>|<span data-ttu-id="20726-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20726-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20726-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20726-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20726-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20726-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20726-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20726-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20726-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20726-116">Not supported.</span></span>|
|<span data-ttu-id="20726-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20726-117">Application</span></span>|<span data-ttu-id="20726-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20726-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20726-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20726-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="20726-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20726-120">Request headers</span></span>
|<span data-ttu-id="20726-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20726-121">Header</span></span>|<span data-ttu-id="20726-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20726-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20726-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20726-123">Authorization</span></span>|<span data-ttu-id="20726-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20726-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20726-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20726-125">Accept</span></span>|<span data-ttu-id="20726-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20726-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20726-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20726-127">Request body</span></span>
<span data-ttu-id="20726-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20726-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="20726-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="20726-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="20726-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20726-130">Property</span></span>|<span data-ttu-id="20726-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20726-131">Type</span></span>|<span data-ttu-id="20726-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20726-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20726-133">assignments</span><span class="sxs-lookup"><span data-stu-id="20726-133">assignments</span></span>|<span data-ttu-id="20726-134">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="20726-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="20726-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20726-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="20726-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20726-136">Response</span></span>
<span data-ttu-id="20726-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="20726-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="20726-138">Пример</span><span class="sxs-lookup"><span data-stu-id="20726-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="20726-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="20726-139">Request</span></span>
<span data-ttu-id="20726-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20726-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 293

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="20726-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="20726-141">Response</span></span>
<span data-ttu-id="20726-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20726-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





