---
title: Перечисление объектов managedEBookAssignment
description: Список свойств и связей объектов managedEBookAssignment.
author: tfitzmac
ms.openlocfilehash: 43625693f6510eb632f4c361cebab07066ae058f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340581"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="abfba-103">Перечисление объектов managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="abfba-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="abfba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abfba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abfba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abfba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abfba-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abfba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abfba-107">Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abfba-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abfba-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="abfba-108">Prerequisites</span></span>
<span data-ttu-id="abfba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abfba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abfba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abfba-111">Permission type</span></span>|<span data-ttu-id="abfba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abfba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abfba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abfba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abfba-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abfba-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abfba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abfba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abfba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abfba-116">Not supported.</span></span>|
|<span data-ttu-id="abfba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abfba-117">Application</span></span>|<span data-ttu-id="abfba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abfba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abfba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abfba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="abfba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abfba-120">Request headers</span></span>
|<span data-ttu-id="abfba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abfba-121">Header</span></span>|<span data-ttu-id="abfba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="abfba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abfba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abfba-123">Authorization</span></span>|<span data-ttu-id="abfba-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="abfba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abfba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="abfba-125">Accept</span></span>|<span data-ttu-id="abfba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abfba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abfba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abfba-127">Request body</span></span>
<span data-ttu-id="abfba-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abfba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abfba-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="abfba-129">Response</span></span>
<span data-ttu-id="abfba-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abfba-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abfba-131">Пример</span><span class="sxs-lookup"><span data-stu-id="abfba-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="abfba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="abfba-132">Request</span></span>
<span data-ttu-id="abfba-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abfba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="abfba-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="abfba-134">Response</span></span>
<span data-ttu-id="abfba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="abfba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
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





