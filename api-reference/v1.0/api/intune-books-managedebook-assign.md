---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94c50cf4e3f880f61f1e392d9166c6dfe7a6f5ac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978628"
---
# <a name="assign-action"></a><span data-ttu-id="5e6bf-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="5e6bf-103">assign action</span></span>

> <span data-ttu-id="5e6bf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e6bf-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e6bf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e6bf-106">Prerequisites</span></span>
<span data-ttu-id="5e6bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e6bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e6bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e6bf-109">Permission type</span></span>|<span data-ttu-id="5e6bf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e6bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e6bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e6bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e6bf-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e6bf-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e6bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e6bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e6bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-114">Not supported.</span></span>|
|<span data-ttu-id="5e6bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e6bf-115">Application</span></span>|<span data-ttu-id="5e6bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e6bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e6bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5e6bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e6bf-118">Request headers</span></span>
|<span data-ttu-id="5e6bf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e6bf-119">Header</span></span>|<span data-ttu-id="5e6bf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5e6bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e6bf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e6bf-121">Authorization</span></span>|<span data-ttu-id="5e6bf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e6bf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5e6bf-123">Accept</span></span>|<span data-ttu-id="5e6bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5e6bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e6bf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e6bf-125">Request body</span></span>
<span data-ttu-id="5e6bf-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5e6bf-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5e6bf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e6bf-128">Property</span></span>|<span data-ttu-id="5e6bf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5e6bf-129">Type</span></span>|<span data-ttu-id="5e6bf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5e6bf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e6bf-131">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="5e6bf-131">managedEBookAssignments</span></span>|<span data-ttu-id="5e6bf-132">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5e6bf-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5e6bf-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5e6bf-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5e6bf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e6bf-134">Response</span></span>
<span data-ttu-id="5e6bf-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e6bf-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5e6bf-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e6bf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e6bf-137">Request</span></span>
<span data-ttu-id="5e6bf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 318

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5e6bf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e6bf-139">Response</span></span>
<span data-ttu-id="5e6bf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e6bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



