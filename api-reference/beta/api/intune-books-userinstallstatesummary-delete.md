---
title: Удаление объекта userInstallStateSummary
description: Удаляет объект userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a570d86e7e54b69abea2e90d3eaa4f467eac1fc1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39931075"
---
# <a name="delete-userinstallstatesummary"></a><span data-ttu-id="aa909-103">Удаление объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa909-103">Delete userInstallStateSummary</span></span>

> <span data-ttu-id="aa909-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa909-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa909-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa909-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa909-106">Удаляет объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="aa909-106">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa909-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aa909-107">Prerequisites</span></span>
<span data-ttu-id="aa909-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa909-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa909-110">Permission type</span></span>|<span data-ttu-id="aa909-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa909-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa909-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa909-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa909-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa909-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aa909-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa909-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa909-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa909-115">Not supported.</span></span>|
|<span data-ttu-id="aa909-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa909-116">Application</span></span>|<span data-ttu-id="aa909-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa909-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa909-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa909-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="aa909-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa909-119">Request headers</span></span>
|<span data-ttu-id="aa909-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa909-120">Header</span></span>|<span data-ttu-id="aa909-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aa909-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa909-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa909-122">Authorization</span></span>|<span data-ttu-id="aa909-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa909-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa909-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aa909-124">Accept</span></span>|<span data-ttu-id="aa909-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa909-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa909-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa909-126">Request body</span></span>
<span data-ttu-id="aa909-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa909-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa909-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa909-128">Response</span></span>
<span data-ttu-id="aa909-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aa909-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa909-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aa909-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa909-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa909-131">Request</span></span>
<span data-ttu-id="aa909-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa909-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="aa909-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa909-133">Response</span></span>
<span data-ttu-id="aa909-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa909-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





