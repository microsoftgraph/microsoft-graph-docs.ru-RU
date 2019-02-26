---
title: Удаление объекта iosVppEBookAssignment
description: Удаляет объект iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8364981b676c73b7d1610612bc104bce3237b116
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252009"
---
# <a name="delete-iosvppebookassignment"></a><span data-ttu-id="3d404-103">Удаление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="3d404-103">Delete iosVppEBookAssignment</span></span>

> <span data-ttu-id="3d404-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d404-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d404-105">Удаляет объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3d404-105">Deletes a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d404-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d404-106">Prerequisites</span></span>
<span data-ttu-id="3d404-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d404-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d404-109">Permission type</span></span>|<span data-ttu-id="3d404-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d404-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d404-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d404-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d404-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d404-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d404-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d404-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d404-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d404-114">Not supported.</span></span>|
|<span data-ttu-id="3d404-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d404-115">Application</span></span>|<span data-ttu-id="3d404-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d404-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d404-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d404-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3d404-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d404-118">Request headers</span></span>
|<span data-ttu-id="3d404-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d404-119">Header</span></span>|<span data-ttu-id="3d404-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3d404-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d404-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d404-121">Authorization</span></span>|<span data-ttu-id="3d404-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3d404-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d404-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3d404-123">Accept</span></span>|<span data-ttu-id="3d404-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d404-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d404-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d404-125">Request body</span></span>
<span data-ttu-id="3d404-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d404-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d404-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d404-127">Response</span></span>
<span data-ttu-id="3d404-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d404-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d404-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3d404-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d404-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d404-130">Request</span></span>
<span data-ttu-id="3d404-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d404-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3d404-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="3d404-132">Response</span></span>
<span data-ttu-id="3d404-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3d404-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



