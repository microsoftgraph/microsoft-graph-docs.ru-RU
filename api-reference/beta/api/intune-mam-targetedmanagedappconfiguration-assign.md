---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1312f1a32a4162115d6ed7427dd134593d6ca455
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152383"
---
# <a name="assign-action"></a><span data-ttu-id="020ef-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="020ef-103">assign action</span></span>

> <span data-ttu-id="020ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="020ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="020ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="020ef-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="020ef-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="020ef-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="020ef-107">Prerequisites</span></span>
<span data-ttu-id="020ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="020ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="020ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="020ef-110">Permission type</span></span>|<span data-ttu-id="020ef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="020ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="020ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="020ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="020ef-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="020ef-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="020ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="020ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="020ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020ef-115">Not supported.</span></span>|
|<span data-ttu-id="020ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="020ef-116">Application</span></span>|<span data-ttu-id="020ef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="020ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="020ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="020ef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="020ef-119">Request headers</span></span>
|<span data-ttu-id="020ef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="020ef-120">Header</span></span>|<span data-ttu-id="020ef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="020ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="020ef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="020ef-122">Authorization</span></span>|<span data-ttu-id="020ef-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="020ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="020ef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="020ef-124">Accept</span></span>|<span data-ttu-id="020ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="020ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="020ef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="020ef-126">Request body</span></span>
<span data-ttu-id="020ef-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="020ef-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="020ef-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="020ef-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="020ef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="020ef-129">Property</span></span>|<span data-ttu-id="020ef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="020ef-130">Type</span></span>|<span data-ttu-id="020ef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="020ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="020ef-132">assignments</span><span class="sxs-lookup"><span data-stu-id="020ef-132">assignments</span></span>|<span data-ttu-id="020ef-133">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="020ef-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="020ef-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="020ef-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="020ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="020ef-135">Response</span></span>
<span data-ttu-id="020ef-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="020ef-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="020ef-137">Пример</span><span class="sxs-lookup"><span data-stu-id="020ef-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="020ef-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="020ef-138">Request</span></span>
<span data-ttu-id="020ef-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="020ef-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="020ef-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="020ef-140">Response</span></span>
<span data-ttu-id="020ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="020ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




