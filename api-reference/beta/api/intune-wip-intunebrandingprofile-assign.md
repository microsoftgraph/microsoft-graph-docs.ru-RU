---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da399b05962eee48bc6b8290f914117a98e146ec
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178600"
---
# <a name="assign-action"></a><span data-ttu-id="a4582-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="a4582-103">assign action</span></span>

<span data-ttu-id="a4582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4582-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4582-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4582-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4582-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4582-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a4582-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4582-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a4582-108">Prerequisites</span></span>
<span data-ttu-id="a4582-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4582-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4582-111">Permission type</span></span>|<span data-ttu-id="a4582-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4582-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4582-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4582-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4582-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4582-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4582-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4582-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4582-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4582-116">Not supported.</span></span>|
|<span data-ttu-id="a4582-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4582-117">Application</span></span>|<span data-ttu-id="a4582-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4582-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4582-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4582-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a4582-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4582-120">Request headers</span></span>
|<span data-ttu-id="a4582-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4582-121">Header</span></span>|<span data-ttu-id="a4582-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4582-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4582-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4582-123">Authorization</span></span>|<span data-ttu-id="a4582-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4582-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4582-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4582-125">Accept</span></span>|<span data-ttu-id="a4582-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4582-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4582-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4582-127">Request body</span></span>
<span data-ttu-id="a4582-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4582-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a4582-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a4582-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a4582-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4582-130">Property</span></span>|<span data-ttu-id="a4582-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4582-131">Type</span></span>|<span data-ttu-id="a4582-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4582-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4582-133">assignments</span><span class="sxs-lookup"><span data-stu-id="a4582-133">assignments</span></span>|<span data-ttu-id="a4582-134">Коллекция [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a4582-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="a4582-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4582-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a4582-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4582-136">Response</span></span>
<span data-ttu-id="a4582-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4582-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4582-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a4582-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4582-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4582-139">Request</span></span>
<span data-ttu-id="a4582-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4582-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 267

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a4582-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4582-141">Response</span></span>
<span data-ttu-id="a4582-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4582-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



