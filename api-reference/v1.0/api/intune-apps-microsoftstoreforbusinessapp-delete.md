---
title: Удаление объекта microsoftStoreForBusinessApp
description: Удаляет объект microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12204a16d9a7ee34c3b4dae37f84ea91a0fb904f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251939"
---
# <a name="delete-microsoftstoreforbusinessapp"></a><span data-ttu-id="8c834-103">Удаление объекта microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="8c834-103">Delete microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="8c834-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c834-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c834-105">Удаляет объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c834-105">Deletes a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c834-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c834-106">Prerequisites</span></span>
<span data-ttu-id="8c834-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8c834-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c834-109">Permission type</span></span>|<span data-ttu-id="8c834-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c834-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c834-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c834-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c834-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c834-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c834-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c834-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c834-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c834-114">Not supported.</span></span>|
|<span data-ttu-id="8c834-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c834-115">Application</span></span>|<span data-ttu-id="8c834-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c834-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c834-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c834-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8c834-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c834-118">Request headers</span></span>
|<span data-ttu-id="8c834-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c834-119">Header</span></span>|<span data-ttu-id="8c834-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8c834-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c834-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c834-121">Authorization</span></span>|<span data-ttu-id="8c834-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8c834-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c834-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8c834-123">Accept</span></span>|<span data-ttu-id="8c834-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c834-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c834-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c834-125">Request body</span></span>
<span data-ttu-id="8c834-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c834-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c834-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c834-127">Response</span></span>
<span data-ttu-id="8c834-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c834-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c834-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8c834-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c834-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c834-130">Request</span></span>
<span data-ttu-id="8c834-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c834-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8c834-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="8c834-132">Response</span></span>
<span data-ttu-id="8c834-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8c834-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



