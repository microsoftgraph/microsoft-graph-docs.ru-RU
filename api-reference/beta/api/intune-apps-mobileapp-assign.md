---
title: Действие assign
description: Н/Д
ms.openlocfilehash: 9a7d1fdbcfb494fa1e51f4d961498c87e936ca27
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081180"
---
# <a name="assign-action"></a><span data-ttu-id="4e39f-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="4e39f-103">assign action</span></span>

> <span data-ttu-id="4e39f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e39f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e39f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e39f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e39f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e39f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e39f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4e39f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e39f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e39f-108">Prerequisites</span></span>
<span data-ttu-id="4e39f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e39f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e39f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e39f-111">Permission type</span></span>|<span data-ttu-id="4e39f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e39f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e39f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e39f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e39f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e39f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e39f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e39f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e39f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e39f-116">Not supported.</span></span>|
|<span data-ttu-id="4e39f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e39f-117">Application</span></span>|<span data-ttu-id="4e39f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e39f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e39f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e39f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="4e39f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e39f-120">Request headers</span></span>
|<span data-ttu-id="4e39f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e39f-121">Header</span></span>|<span data-ttu-id="4e39f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e39f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e39f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e39f-123">Authorization</span></span>|<span data-ttu-id="4e39f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e39f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e39f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e39f-125">Accept</span></span>|<span data-ttu-id="4e39f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e39f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e39f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e39f-127">Request body</span></span>
<span data-ttu-id="4e39f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e39f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4e39f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4e39f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4e39f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e39f-130">Property</span></span>|<span data-ttu-id="4e39f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e39f-131">Type</span></span>|<span data-ttu-id="4e39f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e39f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e39f-133">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="4e39f-133">mobileAppAssignments</span></span>|<span data-ttu-id="4e39f-134">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4e39f-134">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="4e39f-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4e39f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e39f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e39f-136">Response</span></span>
<span data-ttu-id="4e39f-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e39f-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e39f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4e39f-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e39f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e39f-139">Request</span></span>
<span data-ttu-id="4e39f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e39f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4e39f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e39f-141">Response</span></span>
<span data-ttu-id="4e39f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4e39f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





