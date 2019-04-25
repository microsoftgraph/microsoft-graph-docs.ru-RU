---
title: Удаление Мобилеапптраублешутинжевент
description: Описывает метод Delete Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41c9383524e29ff897ea255555ab663476c36659
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527149"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="d113c-103">Удаление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="d113c-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="d113c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d113c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d113c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d113c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d113c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d113c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d113c-107">Удаляет объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d113c-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d113c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d113c-108">Prerequisites</span></span>
<span data-ttu-id="d113c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d113c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d113c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d113c-111">Permission type</span></span>|<span data-ttu-id="d113c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d113c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d113c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d113c-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="d113c-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d113c-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="d113c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d113c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d113c-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d113c-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="d113c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d113c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d113c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d113c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d113c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d113c-119">Not supported.</span></span>|
|<span data-ttu-id="d113c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d113c-120">Application</span></span>|<span data-ttu-id="d113c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d113c-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d113c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d113c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="d113c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d113c-123">Request headers</span></span>
|<span data-ttu-id="d113c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d113c-124">Header</span></span>|<span data-ttu-id="d113c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="d113c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d113c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d113c-126">Authorization</span></span>|<span data-ttu-id="d113c-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d113c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d113c-128">Accept</span><span class="sxs-lookup"><span data-stu-id="d113c-128">Accept</span></span>|<span data-ttu-id="d113c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d113c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d113c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d113c-130">Request body</span></span>
<span data-ttu-id="d113c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d113c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d113c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d113c-132">Response</span></span>
<span data-ttu-id="d113c-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d113c-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d113c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d113c-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d113c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d113c-135">Request</span></span>
<span data-ttu-id="d113c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d113c-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="d113c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d113c-137">Response</span></span>
<span data-ttu-id="d113c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d113c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




