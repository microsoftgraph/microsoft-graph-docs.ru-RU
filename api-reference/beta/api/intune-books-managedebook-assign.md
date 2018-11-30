---
title: Действие assign
description: Н/Д
ms.openlocfilehash: c43999cfe48beacc7d14fd28039e558703cf1160
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080313"
---
# <a name="assign-action"></a><span data-ttu-id="7cc59-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="7cc59-103">assign action</span></span>

> <span data-ttu-id="7cc59-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7cc59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cc59-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cc59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cc59-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7cc59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cc59-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7cc59-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cc59-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7cc59-108">Prerequisites</span></span>
<span data-ttu-id="7cc59-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cc59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cc59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cc59-111">Permission type</span></span>|<span data-ttu-id="7cc59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cc59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cc59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cc59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cc59-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cc59-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cc59-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cc59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cc59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cc59-116">Not supported.</span></span>|
|<span data-ttu-id="7cc59-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cc59-117">Application</span></span>|<span data-ttu-id="7cc59-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cc59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cc59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cc59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7cc59-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cc59-120">Request headers</span></span>
|<span data-ttu-id="7cc59-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cc59-121">Header</span></span>|<span data-ttu-id="7cc59-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7cc59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cc59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cc59-123">Authorization</span></span>|<span data-ttu-id="7cc59-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7cc59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cc59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7cc59-125">Accept</span></span>|<span data-ttu-id="7cc59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cc59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cc59-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cc59-127">Request body</span></span>
<span data-ttu-id="7cc59-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cc59-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7cc59-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7cc59-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7cc59-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cc59-130">Property</span></span>|<span data-ttu-id="7cc59-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7cc59-131">Type</span></span>|<span data-ttu-id="7cc59-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7cc59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cc59-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="7cc59-133">managedEBookAssignments</span></span>|<span data-ttu-id="7cc59-134">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7cc59-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="7cc59-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7cc59-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7cc59-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cc59-136">Response</span></span>
<span data-ttu-id="7cc59-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7cc59-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7cc59-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7cc59-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cc59-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cc59-139">Request</span></span>
<span data-ttu-id="7cc59-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cc59-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

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

### <a name="response"></a><span data-ttu-id="7cc59-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cc59-141">Response</span></span>
<span data-ttu-id="7cc59-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7cc59-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





