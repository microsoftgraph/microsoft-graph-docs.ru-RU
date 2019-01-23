---
title: Действие assign
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 008d16fa6af0adff90606b1b88c3e98097b43b60
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420950"
---
# <a name="assign-action"></a><span data-ttu-id="1122a-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="1122a-103">assign action</span></span>

> <span data-ttu-id="1122a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1122a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1122a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1122a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1122a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1122a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1122a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1122a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1122a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1122a-108">Prerequisites</span></span>
<span data-ttu-id="1122a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1122a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1122a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1122a-111">Permission type</span></span>|<span data-ttu-id="1122a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1122a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1122a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1122a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1122a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1122a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1122a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1122a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1122a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1122a-116">Not supported.</span></span>|
|<span data-ttu-id="1122a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1122a-117">Application</span></span>|<span data-ttu-id="1122a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1122a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1122a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1122a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="1122a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1122a-120">Request headers</span></span>
|<span data-ttu-id="1122a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1122a-121">Header</span></span>|<span data-ttu-id="1122a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1122a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1122a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1122a-123">Authorization</span></span>|<span data-ttu-id="1122a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1122a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1122a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1122a-125">Accept</span></span>|<span data-ttu-id="1122a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1122a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1122a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1122a-127">Request body</span></span>
<span data-ttu-id="1122a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1122a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1122a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="1122a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1122a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1122a-130">Property</span></span>|<span data-ttu-id="1122a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1122a-131">Type</span></span>|<span data-ttu-id="1122a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1122a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1122a-133">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="1122a-133">mobileAppAssignments</span></span>|<span data-ttu-id="1122a-134">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1122a-134">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="1122a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1122a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1122a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1122a-136">Response</span></span>
<span data-ttu-id="1122a-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1122a-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1122a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1122a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1122a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1122a-139">Request</span></span>
<span data-ttu-id="1122a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1122a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1122a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1122a-141">Response</span></span>
<span data-ttu-id="1122a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1122a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




