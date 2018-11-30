---
title: Перечисление объектов notificationMessageTemplate
description: Список свойств и связей объектов notificationMessageTemplate.
ms.openlocfilehash: 699f22298f9f444f67587ddaaa63709575817ee4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075995"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="e60ee-103">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="e60ee-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="e60ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e60ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e60ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e60ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e60ee-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e60ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e60ee-107">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e60ee-107">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e60ee-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e60ee-108">Prerequisites</span></span>
<span data-ttu-id="e60ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e60ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e60ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e60ee-111">Permission type</span></span>|<span data-ttu-id="e60ee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e60ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e60ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e60ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e60ee-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e60ee-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e60ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e60ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e60ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e60ee-116">Not supported.</span></span>|
|<span data-ttu-id="e60ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e60ee-117">Application</span></span>|<span data-ttu-id="e60ee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e60ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e60ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e60ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="e60ee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e60ee-120">Request headers</span></span>
|<span data-ttu-id="e60ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e60ee-121">Header</span></span>|<span data-ttu-id="e60ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e60ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e60ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e60ee-123">Authorization</span></span>|<span data-ttu-id="e60ee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e60ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e60ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e60ee-125">Accept</span></span>|<span data-ttu-id="e60ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e60ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e60ee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e60ee-127">Request body</span></span>
<span data-ttu-id="e60ee-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e60ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e60ee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e60ee-129">Response</span></span>
<span data-ttu-id="e60ee-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e60ee-130">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e60ee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e60ee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e60ee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e60ee-132">Request</span></span>
<span data-ttu-id="e60ee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e60ee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="e60ee-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e60ee-134">Response</span></span>
<span data-ttu-id="e60ee-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e60ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```





