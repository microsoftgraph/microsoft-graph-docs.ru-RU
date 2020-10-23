---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0aed96fe451411d999063008c40e599060058d8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48716084"
---
# <a name="assign-action"></a><span data-ttu-id="f9c8b-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="f9c8b-103">assign action</span></span>

<span data-ttu-id="f9c8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9c8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9c8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9c8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9c8b-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9c8b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f9c8b-108">Prerequisites</span></span>
<span data-ttu-id="f9c8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c8b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c8b-111">Permission type</span></span>|<span data-ttu-id="f9c8b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9c8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9c8b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9c8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9c8b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c8b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9c8b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9c8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9c8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-116">Not supported.</span></span>|
|<span data-ttu-id="f9c8b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9c8b-117">Application</span></span>|<span data-ttu-id="f9c8b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c8b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9c8b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9c8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f9c8b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9c8b-120">Request headers</span></span>
|<span data-ttu-id="f9c8b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9c8b-121">Header</span></span>|<span data-ttu-id="f9c8b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9c8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9c8b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9c8b-123">Authorization</span></span>|<span data-ttu-id="f9c8b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9c8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9c8b-125">Accept</span></span>|<span data-ttu-id="f9c8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9c8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c8b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9c8b-127">Request body</span></span>
<span data-ttu-id="f9c8b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f9c8b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f9c8b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9c8b-130">Property</span></span>|<span data-ttu-id="f9c8b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9c8b-131">Type</span></span>|<span data-ttu-id="f9c8b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9c8b-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="f9c8b-133">managedEBookAssignments</span></span>|<span data-ttu-id="f9c8b-134">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f9c8b-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="f9c8b-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f9c8b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f9c8b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9c8b-136">Response</span></span>
<span data-ttu-id="f9c8b-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9c8b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f9c8b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9c8b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9c8b-139">Request</span></span>
<span data-ttu-id="f9c8b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 487

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f9c8b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c8b-141">Response</span></span>
<span data-ttu-id="f9c8b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9c8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





