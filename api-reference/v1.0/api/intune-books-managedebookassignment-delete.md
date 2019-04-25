---
title: Удаление объекта managedEBookAssignment
description: Удаляет объект managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9f1806206ec1bca7556af364cfa75583770b83c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524895"
---
# <a name="delete-managedebookassignment"></a><span data-ttu-id="ba768-103">Удаление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ba768-103">Delete managedEBookAssignment</span></span>

> <span data-ttu-id="ba768-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba768-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba768-105">Удаляет объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ba768-105">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba768-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba768-106">Prerequisites</span></span>
<span data-ttu-id="ba768-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba768-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba768-109">Permission type</span></span>|<span data-ttu-id="ba768-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba768-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba768-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba768-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba768-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba768-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba768-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba768-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba768-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba768-114">Not supported.</span></span>|
|<span data-ttu-id="ba768-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba768-115">Application</span></span>|<span data-ttu-id="ba768-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba768-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba768-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba768-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ba768-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba768-118">Request headers</span></span>
|<span data-ttu-id="ba768-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba768-119">Header</span></span>|<span data-ttu-id="ba768-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ba768-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba768-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba768-121">Authorization</span></span>|<span data-ttu-id="ba768-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba768-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba768-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ba768-123">Accept</span></span>|<span data-ttu-id="ba768-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ba768-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba768-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba768-125">Request body</span></span>
<span data-ttu-id="ba768-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba768-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba768-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba768-127">Response</span></span>
<span data-ttu-id="ba768-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba768-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ba768-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ba768-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba768-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba768-130">Request</span></span>
<span data-ttu-id="ba768-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba768-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ba768-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba768-132">Response</span></span>
<span data-ttu-id="ba768-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba768-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



