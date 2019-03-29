---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36339bb07430eb1f688e7ae0c00761cabfd74323
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969976"
---
# <a name="assign-action"></a><span data-ttu-id="d5d54-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="d5d54-103">assign action</span></span>

> <span data-ttu-id="d5d54-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5d54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5d54-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5d54-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5d54-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5d54-106">Prerequisites</span></span>
<span data-ttu-id="d5d54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5d54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5d54-109">Permission type</span></span>|<span data-ttu-id="d5d54-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5d54-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5d54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5d54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5d54-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d54-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5d54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5d54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5d54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5d54-114">Not supported.</span></span>|
|<span data-ttu-id="d5d54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5d54-115">Application</span></span>|<span data-ttu-id="d5d54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5d54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5d54-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5d54-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d5d54-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5d54-118">Request headers</span></span>
|<span data-ttu-id="d5d54-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5d54-119">Header</span></span>|<span data-ttu-id="d5d54-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d5d54-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5d54-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5d54-121">Authorization</span></span>|<span data-ttu-id="d5d54-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5d54-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5d54-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d5d54-123">Accept</span></span>|<span data-ttu-id="d5d54-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d5d54-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5d54-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5d54-125">Request body</span></span>
<span data-ttu-id="d5d54-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5d54-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d5d54-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d5d54-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d5d54-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5d54-128">Property</span></span>|<span data-ttu-id="d5d54-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d5d54-129">Type</span></span>|<span data-ttu-id="d5d54-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d5d54-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d54-131">assignments</span><span class="sxs-lookup"><span data-stu-id="d5d54-131">assignments</span></span>|<span data-ttu-id="d5d54-132">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d5d54-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="d5d54-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d5d54-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5d54-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5d54-134">Response</span></span>
<span data-ttu-id="d5d54-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5d54-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5d54-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d5d54-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5d54-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5d54-137">Request</span></span>
<span data-ttu-id="d5d54-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5d54-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d5d54-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5d54-139">Response</span></span>
<span data-ttu-id="d5d54-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5d54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



