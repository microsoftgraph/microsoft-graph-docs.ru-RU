---
title: Delete mobileAppContent
description: Удаляет объект mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e034cb3de2cbaabad9d1dc76f2becb6dda815c3e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420915"
---
# <a name="delete-mobileappcontent"></a><span data-ttu-id="e6afa-103">Delete mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e6afa-103">Delete mobileAppContent</span></span>

> <span data-ttu-id="e6afa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6afa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6afa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6afa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6afa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6afa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6afa-107">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e6afa-107">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6afa-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e6afa-108">Prerequisites</span></span>
<span data-ttu-id="e6afa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6afa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6afa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6afa-111">Permission type</span></span>|<span data-ttu-id="e6afa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6afa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6afa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6afa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6afa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6afa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6afa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6afa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6afa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6afa-116">Not supported.</span></span>|
|<span data-ttu-id="e6afa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6afa-117">Application</span></span>|<span data-ttu-id="e6afa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6afa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6afa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6afa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="e6afa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6afa-120">Request headers</span></span>
|<span data-ttu-id="e6afa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6afa-121">Header</span></span>|<span data-ttu-id="e6afa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e6afa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6afa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6afa-123">Authorization</span></span>|<span data-ttu-id="e6afa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6afa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6afa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6afa-125">Accept</span></span>|<span data-ttu-id="e6afa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6afa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6afa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6afa-127">Request body</span></span>
<span data-ttu-id="e6afa-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6afa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6afa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6afa-129">Response</span></span>
<span data-ttu-id="e6afa-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6afa-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6afa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e6afa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6afa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6afa-132">Request</span></span>
<span data-ttu-id="e6afa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6afa-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="e6afa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6afa-134">Response</span></span>
<span data-ttu-id="e6afa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e6afa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




